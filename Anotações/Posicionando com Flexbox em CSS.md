# Flexbox

## Parte 1

#### Display: Flex;

-  Torna uma tag um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos desta tag, tornam-se flex items.

#### Flex Direction:

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

- Eixos: Row, row-reverse, column e column-reverse.

#### Flex-Wrap

É a propriedade que define se os itens devem ou não quebrar a linha. Por padrão eles não quebram linhas, isso faz com que os flex items sejam compactados além do limite do conteúdo.

- nowrap = padrão, não permite quebra.
- wrap = permite quebra quando não puder mais ser compactado
- wrap-reverse = permite quebra na direção contrária da linha, acima.

#### Flex-Flow

É um atalho para as propriedades flex-direction e flez-wrap. Seu uso não é tão comun, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

#### Justify Content

Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles. *OBS*: caso seus itens estejam ocupando 100% de todo o container, ela não se aplica.

​	Variações:

 - Flex-start: início do container.
 - Flex-end: final do container.
 - Center: ao centro do container.
 - space-between: cria um espaçamento igual entre os elementos.
 - space-around: espaçamentos do meio são 2x maiores que o inicial e final.

#### Align Items

Trata do alinhamento dos flex items de acordo com o eixo do container. Alinhamento é diferente quando itens estão em colunas ou linhas. Permite o alinhamento central no eixo vertical.

Tipos:

	- Center: ao centro.
	- Stretch: padrão, os flex items cresçam igualmente.
	- Flex-star: ao ínicio.
	- Flex-end: ao final.
	- Baseline: a linha base da tipografia dos items.

#### Align Content

É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.

Precisamos :

- O container utilize quebra de linhas;
- A altura do container seja maior que a soma das linhas dos items

Tipos:

- Flex-start: início do container.
 - Flex-end: final do container.
 - Center: ao centro do container.
 - space-between: cria um espaçamento igual entre os elementos.
 - space-around: espaçamentos do meio são 2x maiores que o inicial e final.

## Parte 2

#### Flex Grow

Define a proporcionalidade de crescimentos dos itens, respeitando o tamanho de seus conteúdos internos. **OBS:** Não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container. 

#### Flex Basis

É a propriedade que estabelece o tamanho inicial do item antes das distribuições de espaço restante dentro dele, usando como base o conteúdo interno disposto.

Valores possíveis: 

- auto: caso o item não tenha tamanho, este será proporcional ao conteúdo do item.
- px, %, em, ...: são valores exatos previamente definidos.
- 0(zero): terá relação com a definição do flex-grow.

#### Flex Shrink

É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.

#### Flex

É um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis. *EX*: flex: **1 0 auto** .

#### Order

É para ordenação do itens.

#### Align Self

Estabelece o alinhamento de modo individual sobre um determinado item.

Valores possíveis:

 - Auto: valor padrão, irá respeitar a definição de align-items do container.
 - Center: relativo ao centro de acordo com o eixo.
 - Stretch: ocupa todo o espaço relativo.
 - Flex-star: ao ínicio.
 - Flex-end: ao final.
 - Baseline: utiliza a linha base da tipografia dos items.