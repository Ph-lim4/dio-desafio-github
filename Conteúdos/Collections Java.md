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
