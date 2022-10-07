<h1>HERANÇA</h1>
1. Crie um código que apresente uma herança.

```
  public class Animal{
  public String nome;
  public Number idade;
  public String raca;
  
 public Animal(String nome, Number, idade, String raca){
      this.nome = nome;
      this.idade = idade;
      this.raca = raca;
    }
}


  public class Vaca extends Animal{
  
  public vaquinha(String nome, Number, idade, String raca){
    }
  public number nmroid;
   public boolean vacinada;
```

PARA ESTE CÓDIGO ACIMA PRECISARIAMOS DOS GETTER E SETTERS


OUTRA MANEIRA:



```
  public class Animal{
  
  public String nome;
  public Number idade;
  public String raca;
  }


public class Vaca extends Animal{
 public number nmroidentificador;
 public boolean vacinada;
  }
   ```
  
  <h1>INTERFACE</h1>
  2. Crie um código que apresente uma implementação de interface.
  
  
 Exemplo de Implementação de Interface:
 

```
public class Veiculo {
  public String tipo;
  public String classe;
}

public interface Voador {
  void voa()
}

public interface Terrestre {
  void anda()
}

public interface Navegacao {
  void navega()
}

  
public class Helicoptero extends Veiculo implements Voador {
  public String modelo;
  
  @Override
  public void voa() {
    System.out.println("o"+ modelo + " está em voo!");
  }
}
    
public class Barco extends Veiculo implements Navegacao {
  public String modelo;
  
  @Override
  public void navega() {
    System.out.println("O "+ modelo + " está navegando!");
  }
}

public class Carro extends Veiculo implements Terrestre {
  public String modelo;
  
  @Override
  public void anda() {
    System.out.println("O "+ modelo + " está andando terrestre!");
  }

```

<h1>SOBRECARGA</h1>
3. Crie um código que apresente uma sobrecarga de método.

```
public class Calculadora{

public int calcular(int a + int b){
return a+b;
}
public double calcular( double a, double b){
     return a+b;
  }
   public String calcular( String a, String b){
     return a+b;
}
public static void main(String args[]){
     Calculadora soma= new calculadora();
     System.out.println(soma.calcular(2,2));
    System.out.println(soma.calcular(3.5,7.8));
    System.out.println(soma.calcular("calcu","ludora"));
  }
```

<h1>Composição</h1>
4. Crie um código que apresente uma relação de composição.

```
public class Pessoa {
    private String nome;
    private int idade;

    public Pessoa(String nome, int idade) {
        this.nome = nome;
        this.idade = idade;
    }
}
  **Precisamos usar getters e setters**


public class Carro {
    private Pessoa dono;
    private String modelo;
    

    public Carro(String modelo, Pessoa dono) {
        this.modelo = modelo;
        this.dono = dono;
    }
}

   **Precisamos usar getters e setters**

public class Main {
    public static void main(String[] args) {
        Pessoa pessoa = new Pessoa("Guilerme", 98);
        Carro carro = new Carro("Golf turbo", pessoa);
        System.out.println(carro);
    }
}
```
OUTRA MANEIRA É:

```
public class Carro {
    private String modelo;
    private Pessoa pessoa;
    
}

public class Pessoa {
    private String nome;
    private int idade;
    }
   ```
