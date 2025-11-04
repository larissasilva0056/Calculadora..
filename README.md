Calculadora Científica em C
Descrição do Projeto

Este projeto é uma calculadora científica completa, desenvolvida em linguagem C, com suporte para:

Operações básicas (soma, subtração, multiplicação, divisão)
Operações avançadas (potência, raiz, logaritmo, fatorial)
Funções estatísticas (média, mediana, desvio-padrão)
Funções trigonométricas (seno, cosseno, tangente)
Operações com matrizes 2x2 e 3x3
Conversões entre graus e radianos
Armazenamento e exibição de histórico persistente (salvo em arquivo .txt)

O código é modular, bem comentado e organizado em funções, com uso de structs, arrays, e arquivos para persistência de dados.

 Funcionalidades Principais
Categoria	Funções Implementadas
Básicas	Soma, Subtração, Multiplicação, Divisão
Avançadas	Potência, Raiz quadrada, Fatorial, Logaritmo
Estatísticas	Média, Mediana, Desvio Padrão
Trigonométricas	Seno, Cosseno, Tangente
Comparação	Máximo, Mínimo
Inteiras	MDC, MMC
Conversões	Graus ↔ Radianos
Matrizes	Soma e multiplicação de matrizes 2x2 e 3x3
Extras	Histórico de operações salvo em historico.txt
 Estrutura do Código

Operacao: estrutura (struct) que armazena os dados de cada operação

Funções matemáticas separadas por tipo

Funções para manipulação de matrizes

Sistema de menu interativo com loop do...while

Histórico de operações armazenado em:

vetor historico[MAX_OPERACOES]

arquivo historico.txt (persistência entre execuções)

Como Compilar e Executar
Compilar no terminal:
gcc calculadora.c -o calculadora -lm


O parâmetro -lm é necessário para incluir a biblioteca matemática (math.h).

Executar:
./calculadora

Requisitos

Compilador C (GCC recomendado)

Sistema operacional Windows, Linux ou macOS

Biblioteca padrão math.h (já inclusa no GCC)

Histórico Persistente

Cada operação realizada é salva automaticamente no arquivo historico.txt.
Mesmo após fechar o programa, o histórico é recarregado na próxima execução.

Exemplo do arquivo:

1;Soma;5.00;2.00;7.00
2;Raiz;9.00;0.00;3.00
3;Média;4.00;6.00;5.00

Exemplo de Uso
--- Calculadora Científica ---
1. Soma
2. Subtração
3. Multiplicação
4. Divisão
...
Escolha uma opção: 1

Digite o primeiro número: 8
Digite o segundo número: 4
Resultado: 12.00

integrantes do grupo:
Pedro, Larisssa e Vitoria

