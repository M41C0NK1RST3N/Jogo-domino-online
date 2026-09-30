# 🁃 Dominó Online - Web App

Aplicação web completa e responsiva para jogar Dominó Tradicional (28 peças / Bucha de Ás a Seis) contra Inteligência Artificial diretamente no navegador.

---

## 🚀 Funcionalidades

- **Interface Gráfica Moderna**: Mesa estilizada em feltro, animações suaves e renderização visual precisa dos pontos das peças (0 a 6).
- **Inteligência Artificial Integrada**: Robô oponente com tomada de decisão automatizada e simulação de tempo de reflexão.
- **Validada pelas Regras Tradicionais**:
  - Distribuição inicial de 7 peças para cada jogador.
  - Monte de compra ("Dorminhoco") com 14 peças.
  - Seleção automática de quem inicia a partida com base na maior bucha/ponto.
  - Detecção automática de jogadas válidas (highlight dourado nas peças).
  - Modal para escolha de lado quando a peça encaixar em ambas as extremidades.
  - Regra de fechamento/trancamento de jogo com contagem e comparação de pontos.
- **Design Responsivo**: Adaptável para desktop, tablets e dispositivos móveis.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estruturação semântica e acessível.
- **CSS3**: Layouts Flexbox/Grid, variáveis CSS, sombras e efeitos visuais.
- **JavaScript (Vanilla / ES6)**: Motor lógico do jogo, manipulação de DOM e inteligência do oponente sem dependência de bibliotecas externas.

---

## 🎮 Como Jogar Localmente

1. Faça o download ou clone este repositório.
2. Abra o arquivo `index.html` em qualquer navegador web moderno (Google Chrome, Firefox, Edge, Safari).
3. **Controles**:
   - Clique em qualquer peça destacada em **dourado** na sua mão para jogá-la na mesa.
   - Caso a peça sirva nos dois lados, selecione a extremidade desejada na tela de escolha.
   - Use o botão **Comprar Peça** se não houver jogadas possíveis na sua mão e ainda existirem peças no monte.
   - Use o botão **Passar Vez** caso não possua jogadas e o monte esteja esgotado.

---

## 🌐 Como Publicar Online (Hospedagem Gratuita)

Você pode disponibilizar seu jogo para amigos jogarem online através do GitHub Pages, Vercel ou Netlify:

### Via GitHub Pages
1. Crie um repositório no GitHub (ex: `domino-online`).
2. Envie os arquivos `index.html` e `README.md`.
3. Acesse **Settings** > **Pages** no repositório.
4. Em **Source**, selecione a branch `main` e salve.
5. O link do seu jogo online estará disponível em poucos segundos.

### Via Netlify / Vercel
1. Conecte sua conta do GitHub na plataforma.
2. Selecione o repositório do jogo.
3. Clique em **Deploy**. A aplicação será publicada instantaneamente com um domínio HTTPS gratuito.

---

## 📜 Regras do Jogo Aplicadas

1. **Início**: O jogo embaralha as 28 peças e distribui 7 para você e 7 para o robô. As 14 restantes vão para o monte.
2. **Primeira Jogada**: O jogador que tiver a maior bucha (6x6, 5x5, etc.) inicia a partida.
3. **Turnos**: Em sua vez, você deve jogar uma peça cuja pontuação coincida com uma das extremidades livres da mesa.
4. **Vitória por Batida**: O primeiro a jogar todas as suas 7 peças vence a rodada e soma a pontuação restante da mão do adversário.
5. **Jogo Trancado**: Se ambos os jogadores não puderem jogar e o monte estiver vazio, a partida tranca. O jogador com a menor soma de pontos em mãos vence a rodada.