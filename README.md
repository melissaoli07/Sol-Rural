# DISRUPTIVE ARCHITECTURES: IOT, IOB & GENERATIVE IA
# Grupo Sol Rural - Projeto: Energia Agrovoltaica 
Luiza Nunes de Jesus - RM99768  
Melissa de Oliveira Pecoraro - RM98698  
Pamella Schimalesky Engholm- RM551600  
Roberto Menezes Dos Santos - RM552520
## Indíce
1. [Visão Geral](#visão-geral)
2. [Tecnologias Utilizadas](3tecnologias-utilizadas)
3. [Pré-requisitos](#pré-requisitos)
4. [Configuração do Hardware](#configuração-do-hardware)
5. [Configuração do Software]
Como Executar
Testando a Solução
### 1. Visão Geral
O projeto "Energia Agrovoltaica" propõe uma solução inovadora para os desafios de escassez de energia e água no semiárido do Nordeste do Brasil. Esta região enfrenta dificuldades econômicas e sociais, com a escassez de recursos essenciais impactando diretamente a agricultura local. O objetivo do projeto é utilizar energia solar, uma fonte limpa e acessível, para promover o desenvolvimento sustentável em comunidades agrícolas, principalmente nas regiões do Sertão, onde a falta de energia elétrica e água potável é um obstáculo contínuo. A proposta envolve a criação de uma plataforma inteligente de monitoramento e controle de geração de energia solar, utilizando IoT para otimizar a utilização de energia solar e aumentar a eficiência das atividades agrícolas.

O sistema consiste em:

- **Monitoramento de luminosidade** (simulação de painel solar).  
- **Indicação visual da energia gerada usando LEDs** (verde e vermelho).  
- **Dashboard online para acompanhamento em tempo real.**

### 2. Tecnologias Utilizadas
**Hardware:**

- ESP32 (para funcionalidades Wi-Fi).
- Sensor LDR (Light Dependent Resistor).
- LEDs (verde e vermelho).

**Software:**

- Simluador Wokwi.  
- Node-red

### 3. Pré-requisitos
Antes de começar, você precisa ter o seguinte instalado:

- Wokwi ou outro simulador.
- Node-red instalado.

### 4. Configuração do Hardware

- Monte o circuito básico de acordo com a imagem:
- ![Circuito](imagens/readme.png)


Conecte o sensor LDR ao pino analógico do Arduino (ex.: A0).
Ligue o LED verde ao pino digital D2 e o LED vermelho ao D3.
Use resistores apropriados para proteger os LEDs e o sensor.
Esquema de Conexão:

Alimente o Arduino:
Conecte o Arduino ao computador via cabo USB para carregar o código e testar.

5. Configuração do Software
Arduino IDE:

Faça o download do código fornecido no repositório (arquivo energia_agrovoltaica.ino).
Carregue o código no Arduino conectado ao computador.
Backend (Python):

Instale as dependências:
bash
Copiar código
pip install -r requirements.txt
Execute o backend localmente:
bash
Copiar código
python app.py
O backend deve rodar no endereço http://localhost:5000.
Frontend (Dashboard):

Navegue até o diretório do frontend:
bash
Copiar código
cd frontend
Instale as dependências:
bash
Copiar código
npm install
Inicie o servidor de desenvolvimento:
bash
Copiar código
npm start
Acesse o dashboard em http://localhost:3000.
6. Como Executar
Certifique-se de que o hardware está montado corretamente e o código Arduino foi carregado.
Inicie o backend Python para gerenciar os dados do sensor.
Acesse o dashboard no navegador para visualizar os dados em tempo real.
Ajuste a intensidade de luz no sensor (por exemplo, usando uma lanterna) para testar o comportamento do sistema.
7. Testando a Solução
Teste o circuito físico:

Use uma fonte de luz (ex.: lanterna) para variar a intensidade no LDR.
Verifique se o LED verde acende com alta intensidade e o LED vermelho com baixa intensidade.
Teste o dashboard:

Acesse o dashboard enquanto muda a intensidade da luz no LDR.
Verifique se os gráficos atualizam em tempo real.
Certifique-se de que alertas ou mensagens refletem corretamente o status da energia.
Valide a comunicação:

Teste se os dados capturados pelo sensor são enviados para o backend e exibidos no frontend.




