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



