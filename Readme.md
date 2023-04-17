<h2>Kafka pdi</h2>

<h3>Descrição:</h3>

Uma aplicação simples feita em go para exemplificar como funciona o kafka contendo um producer e um consumer para enviar e consumir mensagens.

<h3>Rodando o projeto:</h3>

- docker-compose up -d

- acesse o container do kafka e crie o tópico de teste ou entre pelo navegador no painel do confluentic e crie manualmente comando para executar no container:
  `kafka-topics --create --bootstrap-server=localhost:9092 --topic=teste --partitions=3`

- Acesse o container da aplicação em um terminal e rode o comando: `go run cmd/consumer/main.go` para deixar o consumer consumindo as mensagem

- Acesse o container da aplicação em um terminal e rode o comando: `go run cmd/producer/main.go` para publicar a mensagem
