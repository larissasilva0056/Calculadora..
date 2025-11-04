Calculadora Científica 2.0 em C
Este projeto implementa uma calculadora científica completa em linguagem C, focada em atender aos requisitos de modularidade, cobertura funcional e qualidade de código. O projeto inclui operações básicas, funções trigonométricas, estatísticas, manipulação de matrizes e um sistema de histórico com persistência em arquivo.

Funcionalidades Principais
A calculadora oferece um menu interativo com as seguintes funcionalidades:

Operações Básicas e Científicas
Soma, Subtração, Multiplicação, Divisão

Potência (pow), Raiz Quadrada (sqrt)

Seno, Cosseno, Tangente (em graus)

Logaritmo na base 10 (log10), Logaritmo natural (ln)

Exponencial (exp), Valor Absoluto (fabs)

Máximo (max), Mínimo (min)

Fatorial (limitado a n <= 20)

MMC (Mínimo Múltiplo Comum), MDC (Máximo Divisor Comum)

Conversão de Graus para Radianos e vice-versa

Cálculo de Hipotenusa

Estatística (Uso de Arrays)
Média Aritmética

Mediana (com ordenação interna)

Desvio Padrão

Matrizes (2x2)
Soma de Matrizes 2x2

Multiplicação de Matrizes 2x2

Sistema e Histórico (Uso de Structs)
Histórico de Operações: Armazena o tipo de operação, operandos e resultado em um struct (Operacao).

Exibição do Histórico.

Bônus Implementados
O projeto inclui funcionalidades extras para a obtenção de pontos bônus:

Persistência do Histórico: O histórico de operações é salvo em um arquivo binário (historico_calculadora.bin) ao sair e é carregado automaticamente ao iniciar a calculadora.

Matrizes 3x3: Adicionadas as operações de Soma e Multiplicação para matrizes de dimensão 3x3.

Como Compilar e Executar
Para compilar e rodar a calculadora, é necessário ter um compilador C compatível com o padrão C99/C11 (como o GCC) instalado.

O código utiliza funções da biblioteca matemática (<math.h>), portanto, é crucial linkar o programa com a flag -lm.

Compilação (Linux/macOS/WSL)
Baixe o arquivo main.c (ou clone o repositório).

Abra o terminal na pasta do projeto.

Compile usando o comando:

Bash
gcc -std=c99 main.c -o calculadora -lm
O flag -lm é obrigatório para as funções matemáticas.

Execução
Execute o programa compilado:

Bash
./calculadora
Execução no GDB (Para Debug)
Para executar com o GNU Debugger, compile com a flag -g:

Bash
gcc -std=c99 main.c -o calculadora -lm -g
gdb calculadora
(gdb) run

Documentação do Código
Todas as funções do arquivo main.c estão devidamente comentadas e documentadas para explicar seus parâmetros, propósito e tratamento de exceções (divisão por zero, raiz de negativo, etc.), cumprindo o requisito de qualidade e documentação.
