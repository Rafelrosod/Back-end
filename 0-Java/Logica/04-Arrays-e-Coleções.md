# Declaração e inicialização de Arrays.

##### Arrays

Um array é uma estrutura de dados que armazena um conjunto fixo de elementos do mesmo tipo. Os elementos de um array são acessados por meio de um índice.

Exemplo de declaração e inicialização de um array:

```Java
int[] numbers = {1, 2, 3, 4, 5};
```

##### Principais características dos arrays:

- O tamanho de um array é fixo após a inicialização e não pode ser alterado.
- Os índices de um array começam em 0 e vão até o tamanho do array menos 1.
- Arrays podem conter elementos de qualquer tipo de dado, incluindo tipos primitivos e objetos.

# Coleções

As coleções em Java são estruturas de dados dinâmicas que podem armazenar um número variável de elementos de qualquer tipo. As coleções fornecem métodos úteis para adicionar, remover e acessar elementos de forma eficiente.

Algumas das coleções mais comuns em Java são:

##### ArrayList:

Uma implementação de lista baseada em array redimensionável.

```Java
import java.util.ArrayList;

ArrayList<Integer> numbers = new ArrayList<>();
numbers.add(1);
numbers.add(2);
// ...
```

##### LinkedList:

Uma implementação de lista duplamente encadeada.

```Java
import java.util.LinkedList;

LinkedList<String> names = new LinkedList<>();
names.add("Alice");
names.add("Bob");
// ...
```

##### HashSet:

Uma implementação de conjunto que não permite elementos duplicados.

```Java
import java.util.HashSet;

HashSet<String> uniqueNames = new HashSet<>();
uniqueNames.add("Alice");
uniqueNames.add("Bob");
// ...

```

##### HashMap:

Uma implementação de mapa que armazena pares chave-valor.

```Java
import java.util.HashMap;

HashMap<String, Integer> scores = new HashMap<>();
scores.put("Alice", 90);
scores.put("Bob", 85);
// ...

```
