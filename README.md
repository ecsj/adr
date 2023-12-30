# Exemplo de um ADR - Architecture Decision Records 

# Uso do RabbitMQ para a fila de mensagens

## Status
Aceito

## Contexto
Necessitamos de um sistema de mensagens assíncronas para comunicação entre microsserviços em nossa arquitetura distribuída. As mensagens precisam ser confiáveis, persistentes e suportar uma alta taxa de transferência.

## Decisão
Optamos por usar o RabbitMQ como nosso serviço de mensagens, devido à sua confiabilidade, suporte a filas persistentes, escalabilidade e documentação abrangente. Ele se integra bem com nossas tecnologias existentes e oferece a flexibilidade necessária para lidar com futuros aumentos de carga.

## Consequências
- Positivas:
  - Melhora na escalabilidade e confiabilidade da comunicação entre microsserviços.
  - Suporte a filas persistentes assegura que mensagens não serão perdidas em caso de falhas.
  - Facilidade de integração com nossas tecnologias existentes.
- Negativas:
  - Pode haver um tempo de aprendizado para a equipe que não está familiarizada com RabbitMQ.
  - Requer monitoramento e manutenção para garantir o desempenho e a disponibilidade adequados.
