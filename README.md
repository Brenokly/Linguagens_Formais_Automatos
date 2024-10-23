# README do Algoritmo de Autômato 🤖

## Descrição 📜

Este programa em C++ implementa um autômato finito que aceita cadeias de entrada baseadas em um conjunto de estados e transições. Ele permite ao usuário definir os estados do autômato, as transições entre eles e testar cadeias de entrada para verificar se são aceitas pelo autômato.

## Estruturas de Dados 📊

O programa utiliza duas estruturas principais:

1. **Transicao**: Representa uma transição em um estado, contendo:
   - `pos_Estado`: O nome do estado resultante após a leitura do símbolo.
   - `valor_Lido`: O símbolo que causa a transição.

2. **Estado**: Representa um estado no autômato, contendo:
   - `nome`: O nome do estado.
   - `transicao`: Um array de transições associadas ao estado.
   - `inicial`: Um booleano que indica se o estado é inicial.
   - `final`: Um booleano que indica se o estado é final.
   - `returnPos_Estado`: Um método que retorna o próximo estado com base no símbolo lido.

## Funcionalidades ⚙️

- **Definição de Estados**: O usuário pode inserir o número de estados e nomeá-los.
- **Definição do Alfabeto**: O usuário insere os símbolos que serão usados para as transições.
- **Definição de Transições**: O programa solicita as transições de cada estado para os símbolos do alfabeto.
- **Estado Inicial**: O usuário indica qual estado é o estado inicial.
- **Estados Finais**: O usuário define quais estados são finais.
- **Testes de Cadeias**: O programa aceita cadeias de entrada e verifica se elas são aceitas pelo autômato.

## Como Usar 🛠️

1. Compile o código usando um compilador de C++ (por exemplo, `g++`).
2. Execute o programa. O usuário será solicitado a inserir os estados, símbolos, transições, estado inicial e estados finais.
3. Após a definição do autômato, insira cadeias para testar. O programa indicará se a cadeia é aceita ou não.

## Exemplo de Execução 💻

```
Insira as informações do autômato!
==================================

Quantos estados serão? 2
Qual o estado 0? q0
Qual o estado 1? q1

Quais serão os simbolos do alfabeto?
Simbolo 0: a
Simbolo 1: b

Entre com as transições de cada estado!
Para cada estado é perguntado, qual será o estado resultado da leitura do símbolo.
Você precisa responder baseado na tabela de estados que você informou.
TABELA DE ESTADOS
Estado 0: q0
Estado 1: q1
Transição do estado q0 lendo a: q1
Transição do estado q0 lendo b: q0
Transição do estado q1 lendo a: q0
Transição do estado q1 lendo b: q1

Quais é o estado inicial? q0
Agora informa quais estados são finais!
Estado final 0: q1

Agora vamos testar com entradas do seu autômato!
Caso queira parar, apenas pressione "Enter"

Cadeia: ab
Cadeia é aceita pelo autômato!
```

## Conclusão 🎓

Este algoritmo de autômato é uma ferramenta básica para entender como funcionam os autômatos finitos. Você pode expandir a funcionalidade, adicionando suporte para autômatos não determinísticos, mais símbolos, ou implementando uma interface gráfica.

## Licença 📄

Este projeto é de uso educacional. Sinta-se à vontade para modificá-lo e usá-lo para fins de aprendizado.
```
