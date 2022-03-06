## Collections Java
### O que é uma Collection?
 - É um objeto que agrupa múltiplos elementos (variaveis primitivas ou objetos) dentro de uma única unidade.
 - Serve para armazenar e processar conjuntos de dados de fomar eficiente.
### Composição:
 - **Interfaces:** É um contrato que quando assumido por uma classe deve ser implementado.
 - **Implementações ou classes:** São as materializações, a codificação das interfaces.
 - **Algoritmos:** É a sequencia lógica, finita e definida de instruções que devem ser seguidas para resolver um problema.

### Hierarquia Collecions
 - (Interface)Collection >> (Interface)Set >> HashSet >> LinkedHashSet.
 - (Interface)Collection >> (Interface)Set >> >> >> TreeSet.
 - (Interface)Collection >> (Interface)List >> ArrayList.
 - (Interface)Collection >> (Interface)List >> Vector.
 - (Interface)Collection >> (Interface)List >> LinkedList.
 - (Interface)Map >> Hashtable.
 - (Interface)Map >> HashMap >> LinkedHashMap.
 - (Interface)Map >> >> >> TreeMap.
 - Object >> Arrays.
 - Object >> Collections.  

## Lists
### Coleções com interações ordenadas: Listas
Chamada da Interface List: java.util.List

 - Elementos duplicados e garante ordem de inserção.
 - "ArrayList deve ser usado onde mais operações de pesquisa são necessárias, e LinkedList deve ser usado onde mais operações de inserção e exclusão são necessárias."
 #### Comandos:
 ##
 - Criação: 
    - List< Double> notas = *new* ArrayList< Double>();
 - Adição: 
    - notas.add(7.0); 
    - notas.add(4, 8d); *Dessa forma se escolhe a posição e o dado*.
 - Substituição:
    - notas.set(notas.indexOf(5d), 6.0);
 - Conferir se há o elemento dentro da lista:
    - notas.contains(5d);
 - Verificar em uma posição especifica:
    - notas.get(2);
 - Exibir a menor e maior nota:
    - Collections.min(notas);
    - Collections.max(notas);
 - Soma dos valores:
    - Interator< Double> iterator = notas.iterator();
 - Remoção:
    - notas.remove(posição ou item)
 - Apagar toda a lista:
    - notas.clear();
 - Verificar se esta vazia:
    - notas.isEmpty();

## Set
### Coleções singulares: Set
Chamada da Interface List: java.util.Set

 - Não permite elementor duplicados.
 - Não possui índice.

 #### Comandos:
 ##
 - Criação: 
    - Set< Double> notas = new HashSet< >(Arrays.asList());
 - Conferir se há o elemento dentro da lista:
    - notas.contains(5d);
 - Exibir a menor e maior nota:
    - Collections.min(notas);
    - Collections.max(notas);
 - Soma dos valores:
    - Interator< Double> iterator = notas.iterator();
 - Remoção:
    - notas.remove(item)

## Map
### Coleção de pares: Map
Chamada da Interface List: java.util.Map

 - Elementos únicos (key) para cada valor (value).

 #### Comandos:
 ##
 - Criação: 
    - Map< String, Double> carrosPopulares = new HashMap< >(){{
    put("gol", 14.4);
    put("uno", 15.6);
    put("mobi", 16.1);
    }}
 - Substituir value:
    - carrosPopulares.put("gol", 15.2);
 - Verificar se uma key especifica existe:
    - carrosPopulare.containsKey("tucson);
 - Exibir o value de uma key:
    - carrosPopulares.get("uno");
 - Exibir keys:
    - Set < String> modelos = carrosPopulares.keySet();
 - Exibir os values:
    - Set< String> consumos = carrosPopulares.values();

## Stream
### Visão geral: Stream
Chamada da Interface List: java.util.Map

 - Elementos únicos (key) para cada valor (value).

### Classe Anônima:
É uma classe que não recebeu um nome e é tanto declarado e instanciado em uma unica instrução. Você deve considerar o uso de uma classe anônima sempre que você precisa para criar uma classe que será instanciado apenas uma vez.

### Functional Interface:
Qualquer interface com um SAM (Single Abstract Method) é uma interface funcional e sua implementação pode ser tratada como expressões lambda.
 - Comparator
 - Consumer
 - Function
 - Predicate

 ### Lambda
 Uma função lambda é uma função sem declaração, isto é, não é necessario colocar um nome, um tipo de retorno e o modificador de acesso. A ideia é que o método seja declarado no mesmo lugar em que será usado. As funções lambda em Java tem a sintaxe definida como (argumento) -> (corpo).

 ### Reference Method
 É um novo  recurso do java 8 que permite fazer referência a um método ou construtor de uma classe (de forma funcional) e assim indicar que ele deve ser utilizado num ponto específico do código, deixando-o mais simples e legível. Para utiliza-lo, basta informar uma classe ou referência seguida do símbolo "::" e o nome do método sem os parênteses no final.
 
 #### Comandos:
 ##