# Estruturas Condicionais.

**if-else:**

```Java
if (condition) {
    // código a ser executado se a condição for verdadeira
} else {
    // código a ser executado se a condição for falsa
}
```

**If-else if-else:**

```Java
if (condition1) {
    // código a ser executado se a primeira condição for verdadeira
} else if (condition2) {
    // código a ser executado se a segunda condição for verdadeira
} else {
    // código a ser executado se nenhuma das condições anteriores for verdadeira
}
```

**Switch-case:**

```Java
switch (expression) {
    case value1:
        // código a ser executado se expression for igual a value1
        break;
    case value2:
        // código a ser executado se expression for igual a value2
        break;
    default:
        // código a ser executado se expression não coincidir com nenhum dos casos anteriores
}
```

**Estruturas de controle adicionais:**

**break e continue**: Usados dentro de loops ou switch-case para interromper a execução do loop ou pular para a próxima iteração.
**return**: Pode ser usado para sair de um método antes de seu término com base em uma condição.

**Operador ternário:**

```Java
variable = (condition) ? expression1 : expression2;
// Se condition for verdadeira, variable será atribuída com expression1, caso contrário, será atribuída com expression2
```

# Loops

**While:**
Executa um bloco de código repetidamente enquanto uma condição especificada for verdadeira.

```Java
int i = 0;
while (i < 5) {
    System.out.println("Número: " + i);
    i++;
}

```

**Do-While:**
Similar ao while loop, mas garante que o bloco de código seja executado pelo menos uma vez, mesmo que a condição seja inicialmente falsa.

```Java
int i = 0;
do {
    System.out.println("Número: " + i);
    i++;
} while (i < 5);
```

**For Loop**
Executa um bloco de código um número específico de vezes.

```Java
for (int i = 0; i < 5; i++) {
    System.out.println("Número: " + i);
}
```

**Enhanced For Loop (Foreach Loop):**
Usado para percorrer elementos em uma coleção (por exemplo, arrays, listas).

```Java
int[] numbers = {1, 2, 3, 4, 5};
for (int number : numbers) {
    System.out.println("Número: " + number);
}
```

Aqui, type é o tipo de elemento na coleção, variable é a variável que representa cada elemento, e collection é a coleção pela qual você está iterando.
