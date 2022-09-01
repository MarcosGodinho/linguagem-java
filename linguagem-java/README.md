# Linguagem de programação Java
Revisão sobre a linguagem Java

## Tópicos de Estudos

* [Linguagem de programação Java](01.md)
  * Paradigmas de Programação: Orientada a objetos, estruturada, imperativa, genérica, funcional, reflexiva, concorrente.
 
  * Modelo de Tipagem de dados: Primitivos: boolean, byte, char, short, int, long, float e double. Referência: Strings, Arrays Primitivos e Objetos.


  * Modelo de construção da Linguagem  
  * Estilo de código
  * Versões
    * Java 1.8
      * Default Methods em interfaces;
      * Lambda e Functional interfaces;
      * Method References;
      * Stream;
      * Nova API de Datas.
    * Java 11
      * Executar arquivo Java com um único comando;
      * Métodos java String;
      * Sintaxe da variável local para parâmetro Lambda;
      * Limitação de recurso;
      * Ler e gravar String de/para aquivos.
    * Java 18
      * API vetorial;
      * "Pattern matching for switch statements";
      * UTF-8;
      * Servidor web simples.
    * Java 19 
      * API de memória e função estrangeira;
      * Correspondência de padrões para expressões de switch;
      * Genéricos universais.

  * Conjunto de palavras reservadas: private, protected, public, abstract, class, extends, final, etc.
  * Ambiente de Desenvolvimento e Ferramentas
    * Documentação oficial: https://docs.oracle.com/en/java/
    * JDK: Java Development Kit.
    * IDEs: VSCode, IntelliJ IDEA, eclipse.
      * Como criar um projeto Java em uma IDE
  * Mercado
    * Popularidade 
      * Tiobe: 3 lugar, 12.40%
      * Survey da Stackoverflow: Loved 45.75%, Dreaded: 54.25%
      * Survey da Jetbrains: Java é a linguagem mais usadana na Coreia do Sul, China e Alemanha.
    * Vagas e salários 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
    * Áreas de aplicações da linguagem Java 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
    * Principais bibliotecas/frameworks 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
* [Hello World](02.md)
  * class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!"); 
        }
    }
  * Nome do arquivo e Extensão: HelloWorld.java
  * Nome da classe: HelloWorld
  * Método main: puclic static void main(String[] args)
  * Escrever dados no console: system.out.println("Aqui")
  * Indentação de código
  * Delimitação de uma instrução: Com o ;
  * Delimitação de bloco de instruções: Com }
  * Compilação e Execução via linha de comando
* [Tipos de Dados e operadores](03.md)
  * Tipos de Dados: Primitivos: boolean, byte, char, short, int, long, float e double. Referência: Strings, Arrays Primitivos e Objetos.
  * Declarações de variáveis: int idade = 0; (Tipo de dado, nome da variável, sinal de =, valor da variável)
  * Nomes válidos para variáveis e boas práticas: camelCase.
  * Atribuição de valores: Sinal de =
  * Operadores
    * Operadores aritméticos: Soma +, Subtração -, Multiplicação *, Divisão /, Sobra %.
    * Operadores booleanos: Maior que >, Menor que <, Igual ==, Diferente !=, Menor ou igual <=, Maior ou igual >=
  * Conversão de tipos de dados: To + tipo de dado. Exemplo: .ToInteger, .ToDouble
* [Saída de Dados](04.md)
  * Método System.out.println: Imprime algo na tela, faz quebra de linha no final.
  * Método System.out.print: Imprime mas sem quebra de linha.
  * Exibir o valor de uma variável: System.out.println()
  * Exibir o valor de um decimal: System.out.println()
* Classe Math
  * Definição: É a classe para ajudar em programas que envolvam matemática. Possui funções para fazer raiz quadrada, PI, logaritmos, etc.
  * Principais operações: Math.exp, Math.pow, Math.log, Math.sqrt.
* String
  * Concatenação de String: variavel.concat("O que deseja concatenar")
  * Principais operações sobre String: index.Of, equals, endsWith, contains, compareTo, lenght.
  * Comparação de String: compareTo, compareToIgnoreCase.
  * Diferença entre String e caracter: String é uma cadeia de caracteres.
* Entrada de Dados
  * Classe Scanner
    * Obter um valor inteiro:
    Scanner leitor = new Scanner(System.in);
    String x = leitor.nextInteger();
    * Obter um valor decimal
    Scanner leitor = new Scanner(System.in);
    String x = leitor.nextDouble();
    * Obter um valor de texto 
     Scanner leitor = new Scanner(System.in);
    String x = leitor.nextString();
* Fluxo de Controle
  * Estruturas de Decisões
    * if-else-then
    void applyBrakes() {
        if (isMoving) {
            currentSpeed--;
        } else {
            System.err.println("The bicycle has already stopped!");
        } 
    }
    * switch
    class Programa{
    public static void main (String [] args){
        int numero = 10;
        switch (numero){
            case 1:
                System.out.println("Dez");
                break;
            case 2:
                System.out.println("Numero muito grande");
                break;
        }

    }
  * Estruturas de Repetições
    * for: for(declara variável; condição; resultado)
    
    * while: while(condição){
        O que fazer enquanto for verdadeiro.
    }
    
    * do-while: do {
         O que fazer.  
    } while(condição);
    
    * Comandos break e continue: Break para um loop. Continue vai para o proximo looping, pulando caso aconteca alguma condição.
    
* Arranjos e Matrizes
  * Definição matemática: Representação de dados em linhas e colunas.
  * Declaração de arranjos: int vetor[tamanho];
  * Declaração de matrizes: vetor = new int [linhas][colunas]
  * Percorrer arranjos: for(int i = 0; i<arranjo.lenght; i++){}
  * Percorrer matrizes
    * Linha a linha
    for(int i = 0; i<arranjo.lenght; i++){
        for(int j= 0; j<arranjo.lenght; j++){
        }
    }
    * Coluna a coluna
    for(int i = 0; i<arranjo.lenght; i++){
        for(int j= 0; j<arranjo.lenght; j++){}
    }
    * Em diagonal 
  * Utilizar arranjos e matrizes como parâmetros de métodos 
  * Utilizar arranjos e matrizes como retorno de métodos 
* Tratamento de Exceções
  * Definição
  * Exceções comuns
    * Divisão por zero
    * Conversão de tipos de dados inválidos
    * Acessar uma posição inválida em um arranjo
    * Acessar uma String nula
  * Bloco para capturar uma exceção 
  * Bloco para capturar diferentes exceções 
  * Bloco finally
  * Lançar uma exceção
* Métodos estáticos
  * Estrutura de declaração de um método estático
  * Nomes válidos e boas práticas 
  * Parâmetros 
  * Retorno
  * Utilização de métodos estáticos 
    * Disponíveis na mesma classe
    * Disponíveis em outra classe/arquivo. 
  * Recursão 
* Classe
  * Definição
    * Representação de classe e objeto na UML
    * Diferença entre classe e objeto
  * Atributos
  * Métodos
  * Construtor 
  * Objeto
  * Inicialização de um objeto 
  * Utilização de um objeto
  * Comparação de objetos
  * Método toString
  * Visibilidade de atributos e métodos
    * Público
    * Privado 
  * Sobrecarga de métodos
  * Sobrecarga de construtores
* Pacotes 
  * Definição
     * Representação de pacotes na UML
  * Definição de um pacote em uma classe
  * Importando uma classe de um pacote diferente
  * Visibilidade de classes, atributos e métodos
     * Default/Pacote  
  * Pacote default
    * Importar uma classe em um pacote default 
* Escopo de classe e objeto
  * Definição 
  * Palavra reservada static 
* Herança
  * Definição
     * Representação de herança na UML
  * Criação de uma classe que realiza herança 
  * Sobreescrita de métodos
  * Polimorfismo
    * Conversão de tipos 
  * Visibilidade de atributos e métodos
     * Protegido
  * Palavra reservada super 
     * Encadeamento de construtor 
     * Encadeamento de método
* Interface
  * Definição
     * Representação de interface na UML
  * Criação de uma classe que implementa uma interface
  * Sobreescrita de métodos
  * Polimorfismo
    * Conversão de tipos 
* Classe abstrada
  * Definição
     * Representação de classe abstrata na UML
  * Criação de uma classe que extende uma classe abstrata
  * Polimorfismo
    * Conversão de tipos 
* Coleções 
  * Definição
  * List e Arraylist 
    * Aplicações
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
  * Map e HashMap
    * Aplicações 
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
* Tipo Enumerado
  *  Definição
     * Representação de tipos enumerados na UML
* Representação de tempo
  * Classe Date
  * Classe Calendar
  * API Date/Time Java 8
    * LocalDate
    * LocalTime
    * LocalDateTime
    * Period
    * Duration
    * Formação de Date/Time 
* Modificador final
  * Definição
    * Representação de final no diagrama UML 
  * Modificador final em uma variável
    * Variável  de tipo primitivo
    * Objeto 
  * Modificador final em um atributo
    * Atributo primitivo
    * Objeto 
  * Modificador final em um método
  * Modificador final em uma classe
* Objeto imutável
  * Definição
  * Aplicações
  * Como criar um objeto imutável
  * Como modificar um objeto imutável 
* Tipos Genéricos
  * Definição
     * Representação de tipos genéricos na UML
  * Criação de classes com tipos genéricos
  * Inicialização de objetos com tipos genéricos  
* Testes Unitários
  * TDD
  * JUnit
    * Adicionar JUnit no projeto Java
  * Teste assertEquals
  * Teste assertTrue/assertFalse
  * Teste assertNull/assertNull
  * Teste assertArrayEquals  
  * Teste fail
  * Teste capturar uma exception
* JDBC
  * Definição
  * Driver de conexão 
  * Como adicionar o driver de conexão no projeto Java
  * Criação de uma conexão com o banco de dados
    * Classe DataManager
    * String de conexão
      * Banco SQLite
      * Banco MySql
      * Banco Postgre 
    * Classe Connection
  * Enviar instruções SQL
    * Classe Statement
    * Classe PreparedStatment   
  * Consultar registros no banco de dados
    * Classe ResultSet
    * Obter um registro
    * Obter uma coleção de registros
  * Bloco de instruções try-with-resources
  * Captura de exceções
    * Driver não encontrado
    * Conexão inválida
    * Tabela não encontrada
    * Registro não encontrado
    * Erro ao inserir/atualizar
    * Erro ao consultar
  * Design Patterns
    * Singleton Factory para criação de conexões   
      * Representação na UML
    * DAO para manipular dados de uma tabela   
      * Representação na UML

## Listas de Exercícios

[SCHEIBEL, Glaucio. Exercícios de Programação](https://github.com/glaucioscheibel/exercicios)

[Beecrowd](https://www.beecrowd.com.br/judge/pt/)

[Leetcode](https://leetcode.com)

[HackerRank](https://www.hackerrank.com)

[Exercism](https://exercism.org/tracks/java)



## Referências Bibliográficas

FURGERI, SÉRGIO. Java 8 Ensino Didático: Desenvolvimento e Implementação de Aplicações. Saraiva Educação SA, 2018.

Schildt, Herbert. Java para iniciantes. Bookman Editora, 2015.

Finegan, Edward, and Robert Liguori. OCA Java SE 8: Guia de Estudos para o Exame 1Z0-808. Bookman Editora, 2018.

Bloch, Joshua. Java Efetivo: 3a edição. Alta Books Editora, 2019.

Martin, Robert C. Código limpo: habilidades práticas do Agile software. Alta Books, 2019.

Fowler, Martin. UML Essencial: um breve guia para linguagem padrão. Bookman editora, 2014.
