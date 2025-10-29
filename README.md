# Calculadora Científica em C – Versão 2.0

## Descrição do Projeto

Este projeto implementa uma **calculadora científica modular em C**, com **20 funções matemáticas**, **arrays**, **structs para histórico de operações**, **menu interativo** e **tratamento de erros**. O objetivo é combinar operações básicas, avançadas e manipulação de matrizes, oferecendo um histórico das últimas operações realizadas.

O projeto foi desenvolvido de forma **modular**, separando funções de cálculo e de entrada/saída, garantindo legibilidade e fácil manutenção.

## Funcionalidades

### Operações básicas:
- Soma  
- Subtração  
- Multiplicação  
- Divisão (com verificação de divisão por zero)

### Operações matemáticas adicionais:
- Potência  
- Raiz quadrada  
- Fatorial  
- Média  
- Mediana  
- Desvio-padrão  
- Máximo  
- Mínimo  
- MDC e MMC  
- Logaritmo natural  
- Trigonometria: seno, cosseno e tangente  
- Conversões: graus ↔ radianos  

### Operações com matrizes 2x2:
- Soma de matrizes  
- Multiplicação de matrizes  

### Histórico de operações:
- Armazenamento das últimas N operações usando `struct Operacao`  
- Registro de tipo de operação, operandos, resultado e ID  
- Exibição completa do histórico  

## Estrutura do Código

- **Struct `Operacao`**: armazena as informações de cada operação realizada.  
- **Arrays**: usados para cálculos de média, mediana e desvio-padrão.  
- **Funções separadas**: cálculo e entrada/saída são tratados em funções diferentes, garantindo modularidade.  
- **Menu interativo**: usa `while + switch` para navegação.  
- **Validação de entradas**: tratamento de erros como divisão por zero, log de número não positivo e raiz de número negativo.

## Como Compilar e Executar

### Compilação no GDB:

```bash
gcc -Wall -Wextra -o calculadora calculadora.c -lm
```

### Rodando no GDB:

```bash
gdb ./calculadora
(gdb) run
```

## Exemplo de Uso

1. Executar o programa  
2. Escolher uma opção do menu (ex.: 1 para soma)  
3. Inserir os operandos conforme solicitado  
4. Visualizar resultado  
5. Consultar histórico das operações realizadas  

## Histórico de Operações

Cada operação realizada é armazenada em um **histórico** que contém:
- ID da operação  
- Tipo (ex.: “Soma”, “MDC”, “Seno”)  
- Operandos  
- Resultado  

Exemplo de saída do histórico:

```
[1] Soma: 5.00 e 3.00 = 8.00
[2] Raiz: 16.00 = 4.00
[3] Fatorial: 5 = 120.00
```

## Estrutura de Pastas 

```
CalculadoraC/
│
├── calculadora.c        # Código fonte completo
├── README.md            # Este arquivo
```


