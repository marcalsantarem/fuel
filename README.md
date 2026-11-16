# ⛽ Calculadora de Abastecimento

Aplicação web moderna, leve e responsiva para motoristas calcularem autonomia, custos de viagem, consumo real e decidirem entre álcool ou gasolina. Funciona como **PWA (Progressive Web App)**, permitindo instalação na tela de início do smartphone e funcionamento **100% offline**, ideal para uso direto no posto de combustível.

---

## 🚀 Funcionalidades

A calculadora possui 6 modos dedicados para diferentes necessidades:

* **🚗 Autonomia:** Saiba exatamente quantos quilômetros você roda com o valor abastecido (R$), litros colocados e o custo por quilômetro rodado.
* **🗺️ Viagem:** Calcule o custo total de uma viagem considerando distância, consumo, opção de ida e volta, pedágios e divisão de custos por pessoa.
* **⛽ Encher Tanque:** Informe a capacidade do tanque e o nível atual (via slider percentual) para saber quantos litros faltam e o custo para completar.
* **⚖️ Álcool x Gasolina:** Descubra rapidamente qual combustível compensa mais financeiramente com base na relação de rendimento (padrão de 70%, totalmente ajustável) e veja a economia estimada.
* **📊 Consumo Real:** Após rodar com tanque cheio, informe a quilometragem e os litros do novo abastecimento para aferir o consumo médio real (km/L e L/100km). Inclui botões para aplicar o resultado como o novo consumo padrão de cidade ou estrada.
* **💰 Quanto Pôr:** Calcule o valor necessário a abastecer para rodar uma distância desejada, aproveitando o combustível já presente no tanque, com sugestão de arredondamento.

---

## ✨ Recursos & Destaques

* **📱 PWA & Offline:** Instalável como aplicativo nativo em Android, iOS e Desktop. Todos os recursos funcionam sem conexão com a internet através do Service Worker.
* **🌙 Tema Escuro Automático:** Adaptação suave ao tema do sistema operacional (*light/dark mode*).
* **🇧🇷 Padrão Brasileiro:** Aceita valores decimais com vírgula ou ponto (ex.: `5,89` ou `5.89`) e formata automaticamente valores em Real (`R$`) e quilômetros (`km`).
* **🔄 Sincronização Inteligente:** O preço do combustível inserido em uma aba é compartilhado automaticamente com as demais abas.
* **💾 Histórico Local:** Salva até 20 cálculos recentes com data e hora. Persistência resiliente com fallback em memória caso o `localStorage` esteja bloqueado.
* **📋 Copiar Resultado:** Botão para copiar o resumo do cálculo formatado para colar em conversas ou anotações.
* **⚙️ Consumo Customizável:** Valores padrão baseados na ficha técnica do Fiat Palio Economy Fire 1.0 (12,3 km/L na cidade e 15 km/L na estrada), com suporte a modo misto (50/50) e ajuste livre.

---

## 📲 Como Instalar como Aplicativo (PWA)

### No Android (Google Chrome / Brave / Edge):
1. Acesse o endereço da aplicação no navegador.
2. Toque no menu do navegador (três pontos) ou no banner exibido na parte inferior.
3. Selecione **"Instalar aplicativo"** ou **"Adicionar à tela inicial"**.

### No iOS / iPhone (Safari):
1. Acesse o endereço da aplicação no Safari.
2. Toque no botão de **Compartilhar** (ícone do quadrado com a seta para cima).
3. Role para baixo e selecione **"Adicionar à Tela de Início"**.

---

## 💻 Como Executar Localmente

Não é necessário instalar ferramentas, Node.js ou dependências:

1. Clone o repositório:
   ```bash
   git clone https://github.com/marcalsantarem/fuel.git
   ```
2. Abra o arquivo `index.html` em qualquer navegador:
   * No Linux/Mac: `xdg-open index.html` ou `open index.html`
   * No Windows: Dê um duplo clique em `index.html`

> **Nota para PWA:** Para testar a instalação do PWA e o Service Worker localmente, sirva os arquivos através de um servidor HTTP local simples (por exemplo: `python3 -m http.server 8000` ou extensão *Live Server* do VS Code).

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Semântico e com recursos de acessibilidade (WAI-ARIA).
* **CSS3:** Variáveis CSS (*Design Tokens*), Grid Layout, Flexbox e `@media (prefers-color-scheme: dark)`.
* **Vanilla JavaScript:** Sem dependências ou frameworks, garantindo carregamento instantâneo.
* **Service Worker & Web App Manifest:** Cache offline e suporte completo a PWA.

---

## 📄 Licença

Distribuído sob a licença MIT. Consulte o repositório para mais informações.
