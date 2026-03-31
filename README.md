# Slither Clone - Multiplayer Local

Este é um clone simplificado do jogo Slither.io, desenvolvido para funcionar em rede local usando Node.js, Express e WebSockets.

## Funcionalidades

- **Multiplayer em tempo real**: Vários jogadores podem se conectar simultaneamente.
- **Mecânica de Cobra**: Movimento suave baseado no mouse, crescimento ao comer e colisão.
- **Sistema de Comida**: Partículas espalhadas pelo mapa que aumentam o tamanho da cobra.
- **Leaderboard**: Ranking em tempo real dos maiores jogadores.
- **Descoberta via mDNS**: O servidor se anuncia na rede local como `snake.local`.
- **Morte Dinâmica**: Quando uma cobra morre, ela se transforma em comida para outros jogadores.

## Como Executar

1. Certifique-se de ter o **Node.js** instalado.
2. Navegue até a pasta do projeto.
3. Instale as dependências (caso ainda não tenha feito):
   ```bash
   npm install
   ```
4. Inicie o servidor:
   ```bash
   npm start
   ```
5. O jogo estará disponível em `http://localhost:3000` na sua rede local.

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução do servidor.
- **Express**: Servidor web para arquivos estáticos.
- **ws (WebSocket)**: Comunicação bidirecional de baixa latência.
- **HTML5 Canvas**: Renderização gráfica no navegador.
- **bonjour-service**: Anúncio do serviço na rede local via mDNS.
- **open**: Abertura automática do navegador.
