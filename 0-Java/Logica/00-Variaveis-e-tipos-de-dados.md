# Variaveis em Java.

As variáveis em Java são declaradas especificando o tipo de dado seguido pelo nome da variável.

```Java
int idade;
String nome;
double altura;
```

As variáveis podem ser inicializadas durante a declaração ou posteriormente no código.

```Java
int idade = 30;
String nome = "João";
double altura = 1.75;
```

É uma boa prática seguir as convenções de nomenclatura ao nomear variáveis em Java, como usar camelCase e escolher nomes descritivos.

```Java
int idadeDoUsuario;
String nomeCompleto;
```

# Tipos de Dados em Java.

##### Tipos Primitivos:

- Inteiros: byte, short, int, long
- Ponto Flutuante: float, double
- Booleano: boolean (true/false)
- Caractere: char

##### Tipos de Referência:

- String: Sequência de caracteres.
- Array: Coleção de elementos do mesmo tipo.
- Classes e Objetos: Instâncias de classes definidas pelo usuário.

##### Literais:

Um literal é uma representação fixa de um valor no código-fonte.

Exemplos:

- int idade = 30; (literal inteiro)
- double salario = 2500.50; (literal de ponto
- flutuante)
- char letra = 'A'; (literal caractere)
- String nome = "Maria"; (literal string)

##### Constantes:

```Java
final double PI = 3,14;
```

##### Tipos Genéricos (a partir do Java 5):

- Permitem a criação de classes, interfaces e métodos que operam com tipos específicos, mas sem especificar esses tipos até a criação da instância.

Exemplo:

```Java
ArrayList<String> listaDeStrings = new ArrayList<String>();
```

##### Java é uma linguagem fortemente tipada, o que significa que cada variável deve ser declarada com um tipo específico.

# Conversão entre tipos de Dados.

**Conversão implícita(Widening Conversion):**

Isso ocorre quando você está atribuindo um valor de um tipo de dado menor para um tipo de dado maior. Java faz isso automaticamente sem qualquer intervenção do programador.

Por exemplo:

```Java
int x = 5;
double y = x;
```

**Conversão explícita (casting):**

Isso ocorre quando você deseja converter um tipo de dado em outro tipo de dado compatível, mas de um tamanho maior ou menor, e precisa especificar a conversão explicitamente.

Por exemplo:

```Java
double x = 5.5;
int y = (int) x;
```

**Métodos de Conversão de Classes Wrapper:**

As classes wrapper em Java (por exemplo, Integer, Double, Float, etc.) fornecem métodos para converter entre tipos de dados primitivos e objetos.

Por exemplo:

```Java
String numberStr = "123";
int number = Integer.parseInt(numberStr);
```

**Métodos valueOf() e toString():**

Muitas classes fornecem métodos valueOf() e toString() para converter entre tipos de dados e strings.

Por exemplo:

```Java
int num = 123;
String numStr = String.valueOf(num);
```

**Conversão de Arrays:**

Você pode converter arrays entre tipos de dados usando iteração manual ou métodos de biblioteca, como Arrays.copyOf().

Por exemplo:

```Java
int[] intArray = {1, 2, 3, 4, 5};
double[] doubleArray = new double[intArray.length];
for (int i = 0; i < intArray.length; i++) {
    doubleArray[i] = intArray[i];
}
```
