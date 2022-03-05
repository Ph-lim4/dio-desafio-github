## Tratamento de exceções
### O que são exceções?
 - Exceção é um evento que interrompe o fluxo normal do processamento de uma classe.
 - Uso correto de exceções tortna o produto mais robusto e confiável. 
 - O tratamento de exceções ajuda o programa a continuar.
 - Importante: Incorpore o tratamento de exceções desde o começo do código.
 - Pode ser dificil implementar o tratamento de exceções posteriormente.

 #### Tipos:
  - **Error:** Usado pela JVM que serve para indicar se existe algum problema de recuro no programa, tornando a execução impossivel de continuar.
  - **Unchecked (Runtime):** Exceptions que PODEM ser evitados se forem tratados e analisados pelo desenvolvedor.
  - **Checked Exception:** Exceptions que DEVEM ser evitados e tratados pelo desenvolvedor para o programa funcionar.

 #### Como tratar?
 - **try, catch, finally:** Cada uma dessas palavras, juntas, definem blocos para o tratamento de exceções.
 - **throws:** Declara que um método pode lançar uma ou várias exceções.
 - **throw:** Lança explicitamente uma exception.