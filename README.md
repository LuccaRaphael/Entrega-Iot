# TáLigado - Monitoramento de Emissões e Consumo Energético com IoT e Machine Learning

## 📋 Descrição do Projeto
O **TáLigado** é uma solução inovadora para promover a eficiência energética e a sustentabilidade ambiental nas empresas. Focando na medição e controle das emissões de gases de efeito estufa, especialmente CO₂, o sistema combina tecnologias de Internet das Coisas (IoT), e visualização de dados em tempo real para oferecer insights e permitir ações corretivas rápidas.

### Funcionalidades Principais:
- **Monitoramento em tempo real** do consumo de energia e emissões de CO₂.
- **Alertas em tempo real** para emissões críticas.
- **Geração de relatórios detalhados** para conformidade regulatória e metas de sustentabilidade.
- **Recomendações personalizadas** para eficiência operacional.

---

## 📖 Problema Resolvido
Empresas enfrentam desafios significativos para monitorar e gerenciar o consumo de energia e as emissões de dióxido de carbono (CO₂). A ausência de dados em tempo real e ferramentas de análise dificultam identificar padrões de desperdício e atender às regulamentações ambientais. O **TáLigado** resolve esse problema integrando monitoramento avançado e insights preditivos.

---

## 🛠 Tecnologias Utilizadas
- **IoT**: Captura de dados de sensores para medições precisas.
- **Node-RED**: Fluxos visuais para automação e integração.
- **WiFi e MQTT**: Comunicação em tempo real.
- **LCD e LEDs**: Exibição local de informações e alertas visuais.
- **Wokwi**: Simulação para testes.

---

## 🚀 Como Replicar e Testar

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

3. **Node-RED**:
   - Importe o fluxo disponível na pasta `Fluxo/fluxos.json`.
   - Configure os tópicos MQTT para comunicação.
   - Visualize os dados no painel do Node-RED.

   ### Fluxo no Node-RED
    ![Node-RED Flow](Imagens\FluxoNode.PNG)

4. **Execução no Hardware**:
   - Conecte o hardware conforme o esquema.
   - Compile o código no ESP32.
   - Monitore o display LCD e os LEDs para alertas.

5. **Vídeo Demonstrativo**:
   - Assista o vídeo: [Link do Vídeo](<https://youtu.be/dc5UFIitvjs>).



