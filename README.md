# Rocket NEAT AI

Um jogo de simulação de foguetes controlados por Inteligência Artificial usando o algoritmo NEAT (NeuroEvolution of Augmenting Topologies).

![Screenshot do Jogo](https://github.com/user-attachments/assets/0fdafa89-9c2e-47c2-ab85-2e1468480beb)
![Screenshot do Jogo](https://github.com/user-attachments/assets/d985d39c-a08a-4d91-9c64-a5fd6e42b927)

## 📋 Sobre o Projeto

Este é um simulador de foguetes onde uma população de foguetes aprende a navegar através de evolução neural. Cada foguete é controlado por uma rede neural que evolui ao longo das gerações usando o algoritmo NEAT.

### Características Principais

- Simulação física realista de foguetes com gravidade e empuxo
- Implementação do algoritmo NEAT para evolução das redes neurais
- Visualização em tempo real da rede neural do melhor foguete
- Sistema de partículas para efeitos visuais dos motores
- Interface gráfica com estatísticas em tempo real

## 🚀 Tecnologias Utilizadas

- C++
- SDL2 (Simple DirectMedia Layer)
- NEAT (NeuroEvolution of Augmenting Topologies)

## 🎮 Como Funciona

### Rede Neural
- 11 neurônios de entrada (inputs)
- Até 10 neurônios ocultos (hidden layer)
- 2 neurônios de saída (outputs)

### Inputs da Rede Neural
1. Distância relativa X até o alvo
2. Distância relativa Y até o alvo
3. Velocidade X do foguete
4. Velocidade Y do foguete
5. Orientação atual (sin)
6. Orientação atual (cos)
7. Diferença angular até o alvo
8. Distância absoluta até o alvo

### Outputs da Rede Neural
1. Controle de empuxo (0 ou 1)
2. Controle de rotação (-1 a 1)

## 🛠️ Instalação

### Pré-requisitos
- CMake
- SDL2
- SDL2_image
- SDL2_ttf

### Compilação
bash
mkdir build
cd build
cmake ..
make

## 🎯 Como Usar

1. Execute o programa compilado
2. Observe os foguetes aprendendo através das gerações
3. O melhor foguete de cada geração é destacado
4. A visualização da rede neural do melhor foguete é mostrada no canto superior direito

## 📊 Estatísticas Mostradas

- Geração Atual
- Melhor Aptidão (Fitness)
- Coletáveis Obtidos
- Tempo Restante da Geração

## 🤖 Parâmetros de Evolução

- Tamanho da População: 100 foguetes
- Tempo por Geração: 10 segundos
- Taxa de Mutação: 40%
- Elite da População: 20%

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

