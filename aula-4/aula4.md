# Aplicação de Sistemas Digitais de Controle Distribuído (SDCD) no Projeto Integrador

## 1. Introdução

Os Sistemas Digitais de Controle Distribuído (SDCD) representam uma evolução dos sistemas de controle industrial, permitindo a distribuição do processamento entre diferentes dispositivos conectados por redes industriais. 

No contexto do Projeto Integrador, que envolve uma aplicação web/mobile com integração IoT para acompanhamento da fabricação de veículos, o uso de um SDCD é essencial para garantir coleta, processamento e disponibilização eficiente dos dados em tempo real.

---

## 2. Papel dos Componentes do Sistema

Considerando o fluxo proposto:

**Sensor → ESP32 → MQTT → Servidor → Aplicativo Mobile → Dashboard → Gestão da Fábrica**

### a) Sensor
Responsável por coletar dados do ambiente industrial, como:
- Temperatura
- Status da produção
- Etapas do processo de fabricação

### b) ESP32
Dispositivo embarcado que:
- Recebe dados dos sensores
- Realiza processamento inicial
- Envia informações via rede

### c) Protocolo MQTT
Protocolo de comunicação leve, ideal para IoT:
- Permite envio de dados em tempo real
- Utiliza modelo publish/subscribe
- Reduz consumo de rede

### d) Servidor
Responsável por:
- Receber dados do MQTT
- Processar e armazenar informações
- Disponibilizar dados para aplicações

### e) Aplicativo Mobile
Interface para o cliente:
- Permite acompanhar o processo de fabricação
- Exibe status do veículo em tempo real

### f) Dashboard
Ferramenta de visualização:
- Apresenta dados consolidados
- Auxilia na tomada de decisão

### g) Gestão da Fábrica
Utiliza as informações para:
- Monitoramento da produção
- Controle de processos
- Planejamento estratégico

---

## 3. Fluxo de Dados do Sistema

O fluxo de dados ocorre da seguinte forma:

1. Os sensores coletam informações do processo produtivo (ex: montagem do veículo).
2. O ESP32 recebe esses dados e os envia via protocolo MQTT.
3. O servidor recebe as informações e realiza o processamento.
4. Os dados são armazenados e disponibilizados para o aplicativo e dashboard.
5. O cliente visualiza o andamento da fabricação do veículo pelo aplicativo.
6. A gestão da fábrica acompanha os dados em tempo real através do dashboard.

Esse fluxo garante comunicação contínua e integrada entre chão de fábrica e sistemas de gestão.

---

## 4. Decisões e Ações com Base nos Dados

Com as informações disponíveis no dashboard, é possível:

- Monitorar o progresso da fabricação
- Identificar atrasos em etapas do processo
- Detectar falhas em equipamentos
- Realizar manutenção preventiva
- Ajustar processos produtivos em tempo real
- Melhorar a experiência do cliente com transparência

---

## 5. Vantagens do Sistema Distribuído

A utilização de um SDCD no projeto traz diversas vantagens:

### a) Confiabilidade
- Elimina ponto único de falha
- Sistema continua operando mesmo com falhas locais

### b) Escalabilidade
- Permite adicionar novos sensores e dispositivos facilmente

### c) Redução de cabeamento
- Comunicação via rede reduz necessidade de conexões físicas

### d) Processamento distribuído
- Cada dispositivo realiza parte do processamento

### e) Integração com TI
- Facilita conexão com sistemas corporativos (ERP, apps)

---

## 6. Conclusão

A aplicação de um Sistema Digital de Controle Distribuído no Projeto Integrador demonstra como a integração entre IoT e sistemas industriais pode transformar o processo produtivo.

O uso de sensores, dispositivos embarcados, comunicação via MQTT e aplicações digitais permite não apenas o controle eficiente da produção, mas também a entrega de valor ao cliente final, que passa a acompanhar em tempo real a fabricação do seu veículo.

Dessa forma, o SDCD se mostra uma solução estratégica, alinhada aos conceitos da Indústria 4.0 e à transformação digital das organizações.