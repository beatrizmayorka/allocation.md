# Resumo sobre alocação de memória/listas/pilhas

### Alocação de memória

<p> Na <strong>alocação estática</strong> o tamanho do vetor é pré-definido antes da execução do programa. O compilador aloca de forma automática quanto do espaço da memória será preciso. Esse tipo de alocação tende a desperdiçar memória, pois o usuário não saberá ao certo quanto de espaço será necessário para armazenar as informações e, dessa forma, irá reservar mais memória do que seria o essencial. </p>
<p> Já na <strong>alocação dinâmica</strong>, a especificação do tamanho do vetor é feita quando o programa está em execução. Isso é feito através da leitura de um arquivo ou da informação digitada pelo usuário. Também é possível aumentar ou diminuir a quantidade de memória alocada. </p><p> Em outro âmbito, é possível explorar três funções que o C possui para tratar a alocação de memória. Abaixo estão: </p>
      <li><strong>Sizeof</strong>: é uma função utilizada para estabelecer o número de bytes para um tipo de dados. Cada compilador possui um número de bytes a ser retornado.</li>
      <li><strong>Malloc</strong>: é uma função usada para alocar um espaço de memória. Ela recebe números inteiros como argumento e esse números correspondem ao número de bytes a serem alocados. No fim, a função retornará um ponteiro do tipo void.</li>
      <li><strong>Free</strong>: serve para liberar o espaço de memória alocado.</li>

### Listas

<p> Estrutura que armazena um conjunto de elementos em sequência. Essa estrutura contém nós interligados por ponteiros, onde o ponteiro apontará para o próximo nó até que esse ponteiro seja Null, o que representará o fim da lista. A lista encadeada está associada a alocação dinâmica de memória. Então, para cada novo elemento na estrutura é alocado um espaço na memória para poder armazená-lo. Sendo assim, o espaço total de memória consumido pela estrutura será equivalente ao número de elementos armazenados nessa memória. </p>  

### Pilhas

<p> A pilha é uma forma de organizar um conjunto de elementos através de uma determinada ordem, ou seja, o último elemento do conjunto será sempre o primeiro a sair (a sigla LIFO - Last In, First Out - descreve essa estratégia). </p>
<p> O manuseio da pilha é feito através de cinco operações, dentre elas: </p>
      <li><strong>Push</strong> - empilhar</li>
      <li><strong>Pop</strong> - desempilhar</li>
      <li><strong>Top</strong> - mostra qual elemento está no topo</li>
      <li><strong>isEmpty</strong> - verifica se está vazia</li>
      <li><strong>isFull</strong> - verifica se está cheia</li>

<p> <strong>**isFull</strong> é utilizado somente com a estratégia correta.</p>

<p> Existem duas estratégias usadas para implementar uma pilha, são elas: alocação dinâmica e alocação estática. </p>
      <li><strong>Alocação estática</strong>: utilizará um vetor com tamanho fixo e limitado. Dessa forma, é será possível usufruir da operação * isFull para verificar se o vetor está completo.</li> 
      <li><strong>Alocação dinâmica</strong>: possibilita fazer o empilhamento de elementos enquanto houver memória.</li>
