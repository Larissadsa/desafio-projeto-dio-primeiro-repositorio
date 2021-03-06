# Anotações Flexbox :pencil:

**Flex container** - É a tag que envolve os itens, será nela que iremos aplicar a propriedade "display: flex". Transforma todos os seus itens filhos em flex itens.

**Flex item** - São os elementos filhos diretos do Flex container, e também podem se tornar Flex container.

### Propriedades flex container:

**Display: flex;**

Torna a tag um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos desta tag tornam-se em flex items.

**Flex-direction**

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

- row (padrão): à direção do texto, esquerda para direita.

- row-reverse: sentido oposto à direção do texto.

- column: ordenação de cima para baixo, em coluna única.

- column-reverse: ordenação inversa, de baixo para cima.

  

**Flex-wrap**

É a propriedade que define se os itens devem ou não quebrar a linha. Por padrão eles não quebram linhas, isso faz com que os flex items sejam compactados além do limite do conteúdo.

- nowrap: é o padrão, não permite a quebra de linha.

- wrap: permite a quebra de linha assim que um dos flex items não puder mais ser compactado.

- wrap-reverse: mesma lógica do wrap, porém na direção contrária.

  

**Flex flow**

É um atalho para as propriedades **flex-direction** e **flex-wrap**. Porém seu uso não é tão comum, visto que quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.



**Justify-content**

Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamentos entre eles. obs: caso seus itens estejam ocupando 100% de todo o container, ela não se aplica.

- flex-start: início do container.
- flex-end: final do container.
- center: ao centro do container
- space-between: cria um espaçamento igual entre os elementos.
- space-around: os espaçamentos do meio são duas vezes maiores que o inicial e final.



**Align-items**

Trata do alinhamento dos flex-items de acordo com o eixo do container. O alinhamento é diferente para quando os itens estão em colunas ou linhas.

Permite o alinhamento central no eixo vertical.

- center: alinhamento dos itens ao centro.
- stretch: padrão, os flex-items crescem igualmente.
- flex-start: alinhamento dos itens no início.
- flex-end: alinhamento dos itens no final.
- baseline: alinhamento de acordo com a linha base da tipografia dos itens.



**Align-content**

É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.  Precisamos que:

- O container utilize quebra de linhas;
- A altura do container seja maior que a soma das linhas dos itens.

Tipos de alinhamento:

- center: alinhamento ao centro.
- stretch: é o padrão e os flex itens crescem igualmente.
- flex-start: alinhamento dos itens no início.
- flex-end: alinhamento dos itens no final.
- space-between: cria um espaçamento igual entre os elementos.
- space-around: os espaçamentos do  meio são duas vezes maiores que o inicial e final.



### Propriedades flex items:

**Flex-grow**

Define a proporcionalidade  de crescimentos dos itens, respeitando o tamanho de seus conteúdos internos. Obs: não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.



**Flex-basis**

É a propriedade que estabelece o tamanho inicial do irem antes da distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

- auto: caso o item não tenha tamanho, este será proporcional ao conteúdo do irem.
- px, %, em,...: são valores exatos previamente definidos.
- 0: terá relação com a definição do flex-grow.



**Flex-shrink**

É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.



**Flex**

Esta propriedade é um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis.



**Order**

Esta propriedade lidará com a ordenação dos itens.



**Align-self**

É a propriedade que estabelece o alinhamento de modo individual sobre um determinado item.

- auto: valor padrão, irá respeitar a definição de align-items do container.
- flex-start: ao início do container.
- flex-end: ao final do container.
- center: relativo ao centro de acordo com o eixo (column ou row).
- stretch: ocupa todo o espaço relativo.
- baseline: utiliza a linha base da tipografia.
