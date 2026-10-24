# Projeto de Lógica de Programação — Adivinha o Animal

Projeto desenvolvido para a disciplina de **Lógica de Programação (Sebrae)**.

O programa é um "Akinator simplificado": o usuário pensa em um animal de uma lista
pré-definida e o algoritmo, por meio de até **6 perguntas de Sim/Não**, descobre qual
animal foi escolhido.

## Objetivo

Aplicar as estruturas de controle **sequencial**, **decisão** e **laço de repetição**
na construção de um algoritmo de identificação de animais.

## Animais possíveis (15)

Leão · Baleia · Tartaruga · Cavalo · Avestruz · Crocodilo · Homem · Pinguim ·
Cobra · Macaco · Pato · Iguana · Morcego · Águia · Panda

## Perguntas utilizadas (6)

1. É mamífero?
2. É quadrúpede?
3. É carnívoro?
4. É herbívoro?
5. **Voa?** *(extra)*
6. **É aquático?** *(extra)*

Além disso, há duas perguntas de desempate usadas apenas quando necessário:

- **"É bípede (anda sobre duas patas)?"** → diferencia **Homem × Macaco**
- **"Tem casco (carapaça)?"** → diferencia **Iguana × Tartaruga**

##  Tabela Verdade

| Animal | Mamífero? | Quadrúpede? | Carnívoro? | Herbívoro? | Voa? | Aquático? |
|--------|:---:|:---:|:---:|:---:|:---:|:---:|
| Leão | Sim | Sim | Sim | Não | Não | Não |
| Cavalo | Sim | Sim | Não | Sim | Não | Não |
| Homem | Sim | Não | Não | Não | Não | Não |
| Macaco | Sim | Não | Não | Não | Não | Não |
| Morcego | Sim | Não | Sim | Não | Sim | Não |
| Baleia | Sim | Não | Sim | Não | Não | Sim |
| Iguana | Não | Sim | Não | Sim | Não | Não |
| Avestruz | Não | Não | Não | Sim | Não | Não |
| Pinguim | Não | Não | Sim | Não | Não | Sim |
| Pato | Não | Não | Não | Sim | Sim | Sim |
| Águia | Não | Não | Sim | Não | Sim | Não |
| Tartaruga | Não | Sim | Não | Sim | Não | Sim |
| Crocodilo | Não | Sim | Sim | Não | Não | Sim |
| Panda | Sim | Sim | Não | Sim | Não | Não |
| Cobra | Não | Não | Sim | Não | Não | Não |

##  Tecnologias

- **Linguagem:** C++ (C++11 ou superior)
- **Compilador sugerido:** g++ / Visual Studio / Code::Blocks






