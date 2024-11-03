# Funções.

- Em Java, o termo "função" geralmente se refere a um método que não está associado a uma classe específica (método estático).
- Funções em Java são definidas usando o modificador static, o que significa que elas podem ser chamadas sem criar uma instância da classe.
- Funções em Java não têm acesso direto a variáveis de instância (membros não estáticos) de uma classe.
  Elas são úteis para agrupar funcionalidades que não dependem do estado de um objeto específico.

Exemplo de função em Java:

```Java
public class Utils {
    public static int soma(int a, int b) {
        return a + b;
    }
}
```

# Métodos.

- Métodos em Java são blocos de código associados a uma classe específica.
- Eles podem ter acesso a variáveis de instância (membros não estáticos) e métodos de uma classe.
- Os métodos em Java podem ser definidos com vários modificadores de acesso, como **public**, **private**, **protected**, etc., que controlam sua visibilidade e acessibilidade.
- Eles são usados para representar o comportamento e as operações que os objetos da classe podem realizar.

Exemplo de método em Java:

```Java
public class Pessoa {
    private String nome;

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getNome() {
        return nome;
    }
}
```

##### Parâmetros de Métodos:

- Os parâmetros de método são variáveis ​​declaradas na assinatura do método que recebem valores quando o método é chamado.
- Eles permitem que os métodos aceitem entradas externas para processamento.
- Os parâmetros são especificados entre parênteses após o nome do método na declaração do método.

Exemplo de método com parâmetros em Java:

```Java
public class Calculadora {
    public static int soma(int a, int b) {
        return a + b;
    }
}
```

##### Retorno de Métodos:

- O retorno de método é o valor que o método envia de volta ao local onde foi chamado.
- O tipo de retorno do método é especificado na declaração do método, após os parâmetros.
- O valor de retorno é especificado usando a palavra-chave **return** seguida do valor a ser retornado.

Quando você chama um método que retorna um valor, você pode usar esse valor em uma expressão, atribuí-lo a uma variável ou fazer qualquer outra operação desejada com ele.

Exemplo de chamada de método com retorno:

```Java
int resultado = Calculadora.soma(5, 3);
System.out.println("A soma é: " + resultado);
```

# Recursão.

A recursão é um conceito em programação em que uma função ou método chama a si mesmo diretamente ou indiretamente. Em Java, você pode usar recursão para resolver problemas de forma elegante e eficiente, especialmente aqueles que podem ser divididos em subproblemas menores do mesmo tipo.

Aqui está um exemplo simples de função recursiva em Java que calcula o fatorial de um número:

```Java
public class Recursao {
    public static int fatorial(int n) {
        if (n == 0 || n == 1) {
            return 1;
        } else {
            return n * fatorial(n - 1);
        }
    }

    public static void main(String[] args) {
        int numero = 5;
        int resultado = fatorial(numero);
        System.out.println("O fatorial de " + numero + " é: " + resultado);
    }
}
```

Neste exemplo, a função fatorial() é recursiva. Ela calcula o fatorial de um número n chamando a si mesma com um argumento menor (n - 1) até que atinja o caso base (quando n é igual a 0 ou 1). Quando isso acontece, a recursão para e os valores de retorno começam a ser calculados, subindo na pilha de chamadas.

É importante ter um caso base em qualquer função recursiva para evitar que a recursão continue indefinidamente. No exemplo acima, o caso base é quando n é 0 ou 1, momento em que a função retorna 1.
