# Dashboard Pico Bússola 🌍🧭

Este projeto é um **painel interativo** desenvolvido em HTML, CSS e JavaScript puro que exibe dados de direção, sensor e estado de botão enviados por um **Raspberry Pi Pico W**. Os dados são armazenados no **Firebase Realtime Database** e atualizados em tempo real na interface.

## 🔧 Funcionalidades

- Exibe uma **bússola** que gira conforme a direção recebida.
- Anima um **cata-vento** de acordo com o valor do sensor (ex: intensidade de vento).
- Mostra o estado do **botão (ligado/desligado)**.
- Atualiza os dados automaticamente a cada 2 segundos.

## 🧰 Tecnologias utilizadas

- **HTML5** – Estrutura da interface.
- **CSS3** – Estilização simples e responsiva.
- **JavaScript ES6+** – Lógica de busca e atualização dos dados.
- **Firebase Realtime Database** – Backend para armazenar as leituras enviadas pelo Pico W.

## 📦 Estrutura do projeto
```
📁 projeto/
├── index.html # Página principal (Dashboard)
├── bussola.png # Imagem da bússola
├── catavento.png # Imagem do cata-vento
```
1. Clone o projeto ou salve os arquivos localmente:
```bash
git clone https://github.com/seuusuario/dashboard-pico-bussola.git
```
2. Certifique-se de que os arquivos bussola.png e catavento.png estejam na mesma pasta do index.html.
3. Abra o projeto no Visual Studio Code e inicie o servidor local com a extensão Live Server:
   - Clique com o botão direito no index.html → "Open with Live Server"
   - O navegador será aberto automaticamente com a visualização do painel
4. O painel buscará os dados mais recentes do Firebase automaticamente.
### 🔁 Atualização em tempo real
- O painel consulta o Firebase a cada 2 segundos:
- Busca a última leitura registrada (direction, sensor, botao).
- Atualiza os elementos visuais com base nos valores recebidos.

### Projetado por Antonio José Mota
