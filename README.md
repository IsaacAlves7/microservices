O **ZeroMQ (ØMQ)** pode ser utilizado para implementar uma arquitetura de **Event-Driven Architecture (EDA)** em microsserviços, mas ele não é um *message broker* como RabbitMQ, Kafka ou NATS. Ele é uma biblioteca de mensageria de alta performance que fornece padrões de comunicação.

Na prática, ele suporta diversos padrões úteis para EDA:

* **Publish/Subscribe (PUB/SUB)** → um serviço publica eventos e vários consumidores os recebem.
* **Push/Pull (Pipeline)** → distribuição de tarefas entre workers.
* **Request/Reply (REQ/REP)** → comunicação síncrona entre serviços.
* **Dealer/Router** → balanceamento de carga e comunicação assíncrona mais sofisticada.

Exemplo do ZeroMQ em uma arquitetura EDA: Imagine um e-commerce:

```
+-----------------+
| Pedido Service  |
+-----------------+
        |
        | Evento: PedidoCriado
        |
      PUB
        |
        v
======================
     ZeroMQ
======================
     |        |       |
    SUB      SUB     SUB
     |        |       |
Estoque  Pagamento  Email
 Service   Service  Service
```

O serviço de pedidos publica um evento:

```json
{
  "event": "PedidoCriado",
  "pedidoId": 123,
  "cliente": "João"
}
```

Todos os microsserviços inscritos recebem esse evento e executam suas responsabilidades.

Entretanto, existe uma diferença importante, o ZeroMQ **não armazena mensagens**.

Se um consumidor estiver offline quando o evento for publicado:

* RabbitMQ → a mensagem pode ficar na fila.
* Kafka → a mensagem permanece no log.
* ZeroMQ → **a mensagem é perdida** (dependendo do padrão utilizado).

Também não possui recursos nativos como:

* filas persistentes;
* confirmação (ACK/NACK);
* retry automático;
* dead-letter queue;
* ordenação persistente;
* replay de eventos.

Tudo isso precisa ser implementado pela aplicação, caso seja necessário.

## Quando usar ZeroMQ

É uma ótima escolha quando você precisa de:

* latência extremamente baixa;
* alta taxa de mensagens;
* comunicação entre processos ou servidores;
* sistemas distribuídos HPC (High Performance Computing);
* processamento financeiro;
* jogos multiplayer;
* aplicações IoT;
* sistemas de visão computacional.

## Quando preferir RabbitMQ ou Kafka

Para microsserviços corporativos, geralmente o mais comum é:

* **RabbitMQ** quando há necessidade de filas confiáveis, ACKs e retries.
* **Kafka** quando o sistema é orientado a eventos com grande volume, retenção de eventos e possibilidade de replay.
* **ZeroMQ** quando a prioridade é desempenho e simplicidade, e a perda ocasional de mensagens é aceitável ou controlada pela própria aplicação.

Comparação rápida:

| Recurso           | ZeroMQ | RabbitMQ | Kafka |
| ----------------- | ------ | -------- | ----- |
| Broker dedicado   | ❌      | ✅        | ✅     |
| Pub/Sub           | ✅      | ✅        | ✅     |
| Persistência      | ❌      | ✅        | ✅     |
| ACK               | ❌      | ✅        | ✅     |
| Replay de eventos | ❌      | ❌        | ✅     |
| Latência          | ⭐⭐⭐⭐⭐  | ⭐⭐⭐      | ⭐⭐⭐⭐  |
| Throughput        | ⭐⭐⭐⭐⭐  | ⭐⭐⭐      | ⭐⭐⭐⭐⭐ |
| Complexidade      | Baixa  | Média    | Alta  |

Em resumo, **é perfeitamente possível construir uma arquitetura EDA com ZeroMQ**, especialmente usando o padrão **PUB/SUB**. Contudo, ele atua como uma camada de transporte de mensagens de alto desempenho, não como um broker completo. Para microsserviços que exigem alta confiabilidade, persistência e recuperação de falhas, tecnologias como RabbitMQ, Kafka ou NATS JetStream costumam ser mais adequadas.

# ZeroMQ messaging patterns

> ZeroMQ is a really beautiful hammer, </br>
> you should take it with you </br>
> and find nails. </br>
>
> -- Someone on the internet.

I know about ZMQ years ago.

I admire [Pieter Hintjens](https://en.wikipedia.org/wiki/Pieter_Hintjens), I read many of his books, and watched all his talks I can find the internet. He was such a great leader!

But I never had a project about messaging, in which I can use ZMQ.

Until I want to write a _subdoman-based http reverse proxy_ (like [ngrok](https://ngrok.com)).

I implemented it by pure TCP and socket API,
a lot of features aboud reliability need to be implemented.

Then I went back to ZMQ docs again, and found that
the _subdoman-based http reverse proxy_ I want to implement
is exactly the **[majordemo](https://zguide.zeromq.org/docs/chapter4/#Service-Oriented-Reliable-Queuing-Majordomo-Pattern)** of ZMQ's zguide.

I finally found the perfact nail!

## Development

```sh
npm install           # Install dependencies
npm run build         # Compile `src/` to `lib/`
npm run build:watch   # Watch the compilation
npm run format        # Format the code
```

## License

[GPLv3](LICENSE)
