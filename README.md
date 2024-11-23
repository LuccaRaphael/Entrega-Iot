# TáLigado - Monitoramento de Emissões e Consumo Energético com IoT e Machine Learning

## Descrição do Projeto
O **TáLigado** é uma solução inovadora para promover a eficiência energética e a sustentabilidade ambiental nas empresas. Focando na medição e controle das emissões de gases de efeito estufa, especialmente CO₂, o sistema combina tecnologias de Internet das Coisas (IoT), e visualização de dados em tempo real para oferecer insights e permitir ações corretivas rápidas.

<img src="Imagens\Logo.jpeg" alt="Logo" width="200">

### Funcionalidades Principais:
- **Monitoramento em tempo real** do consumo de energia e emissões de CO₂.
- **Alertas em tempo real** para emissões críticas.
- **Visualização de dados** através de um **dashboard no Node-RED**.
- **Recomendações personalizadas** para eficiência operacional.

---

## Problema Resolvido
Empresas enfrentam desafios significativos para monitorar e gerenciar o consumo de energia e as emissões de dióxido de carbono (CO₂). A ausência de dados em tempo real e ferramentas de análise dificultam identificar padrões de desperdício e atender às regulamentações ambientais. O **TáLigado** resolve esse problema integrando monitoramento avançado e insights preditivos.

---

## Tecnologias Utilizadas
- **IoT**: Captura de dados de sensores para medições precisas.
- **Node-RED**: Fluxos visuais para automação e integração.
- **Dashboard do Node-RED**: Visualização de dados em tempo real.
- **WiFi e MQTT**: Comunicação em tempo real.
- **LCD e LEDs**: Exibição local de informações e alertas visuais.
- **Wokwi**: Simulação para testes.

---

## Tópicos MQTT Monitorados
O sistema utiliza os seguintes tópicos MQTT para coletar e monitorar dados em tempo real:
- **`gasMonitor/niveis`**: Nível de perigo (%).
- **`gasMonitor/ppm`**: Concentração de gás em PPM.
- **`energyMonitor/consumo`**: Consumo de energia elétrica.
- **`environmentMonitor/attention`**: Monitoramento de atenção ambiental.

---

## Como Replicar e Testar

### Pré-requisitos
- **Hardware**:
  - ESP32.
  - Display LCD I2C.
  - Sensores de gases.
  - Potenciômetro (simula consumo energético).
  - LEDs (indicadores de estado).
  - Buzzer (alerta sonoro).
- **Software**:
  - Node-RED instalado localmente ou em um servidor.
  - Ambiente de simulação.
  - Broker MQTT público (como HiveMQ).

### Instruções:
1. **Simulação no Wokwi**:
   - Acesse o projeto: [Wokwi Link](<https://wokwi.com/projects/415224506759678977>).
   - Configure os sensores e os parâmetros no ambiente de simulação.
   - Execute o código para visualizar os resultados no LCD e LEDs.

   ### Projeto no Wokwi
   <img src="Imagens\wokwi.PNG" alt="Wokwi">

2. **Node-RED**:
   - Importe o fluxo disponível na pasta Fluxo/fluxos.json.
   - Configure os tópicos MQTT para comunicação.
   - Configure o **dashboard do Node-RED** com nós como:
     - **Gauge**: Para visualização de níveis de gás, atenção e consumo de energia.
   - Visualize os dados no painel do Node-RED.

   ### Fluxo no Node-RED
   <img src="Imagens\FluxoNode.PNG" alt="FluxoNode">

   ### Dashboard
   <img src="Imagens\dashboard.PNG" alt="Dashboard">

3. **Execução no Hardware**:
   - Conecte o hardware conforme o esquema.
   - Compile o código no ESP32.
   - Monitore o display LCD e os LEDs para alertas.

4. **Vídeo Demonstrativo**:
   - Vídeo Demonstativo Pedido na Entrega: [Link do Vídeo](<https://youtu.be/JK0bfrEOSxk>).
   - Pitch do projeto: [Link do Vídeo](<https://youtu.be/Gih1BJ_ZiNk>).





