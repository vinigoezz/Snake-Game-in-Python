🐍 Snake Game (Python)
Uma versão moderna e customizável do clássico "Jogo da Cobrinha", desenvolvida em Python. O projeto foca em lógica de movimento em grade, manipulação de coordenadas e renderização de gráficos simples.

🎮 Como Jogar
O objetivo é comer as maçãs que aparecem aleatoriamente na tela para crescer. O jogo termina se a cobra colidir com as paredes ou com o próprio corpo.

Setas Teclado / WASD: Controlam a direção da cobra.

Pontuação: Cada maçã aumenta o tamanho da cobra e a pontuação atual.

Velocidade: A dificuldade aumenta conforme a cobra cresce (opcional).

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.x

Bibliotecas Comuns:

Pygame: Para interface gráfica e sons.

Turtle: (Caso tenha usado essa lib nativa para algo mais simples).

Random: Para geração das frutas em posições aleatórias.

🧠 Lógica do Sistema
O jogo foi estruturado seguindo conceitos fundamentais de desenvolvimento de jogos:

Representação da Cobra: Uma lista de coordenadas [(x1, y1), (x2, y2), ...], onde o primeiro elemento é a cabeça.

Movimentação: A cada frame, uma nova cabeça é adicionada na direção do movimento e a cauda é removida (a menos que ela coma uma fruta).

Detecção de Colisão: Verificação constante se a coordenada da cabeça coincide com as bordas ou com qualquer item da lista do corpo.

📂 Estrutura do Repositório
Plaintext
├── assets/
│   ├── images/        # Ícones da cobra e frutas
│   └── sounds/        # Efeito sonoro de comer e game over
├── src/
│   ├── snake.py       # Classe da cobra e lógica de movimento
│   ├── food.py        # Gerador de comida aleatória
│   └── main.py        # Loop principal e controle de FPS
├── requirements.txt   # Dependências do projeto
└── README.md
🚀 Instalação e Execução
Clone o projeto:

Bash
git clone https://github.com/seu-usuario/snake-game-python.git
cd snake-game-python
Instale as dependências:

Bash
pip install pygame
Inicie o jogo:

Bash
python src/main.py
🛠️ Customização
Você pode facilmente alterar as seguintes variáveis no código:

SCREEN_WIDTH / SCREEN_HEIGHT: Tamanho da janela.

SNAKE_SPEED: Velocidade de atualização do jogo.

GRID_SIZE: Tamanho de cada "bloco" do cenário.
