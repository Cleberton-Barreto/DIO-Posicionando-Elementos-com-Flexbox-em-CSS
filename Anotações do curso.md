# Objetivos do curso :bookmark_tabs:



​	Apresentar os fundamentos e aplicações da propriedade flexbox na criação de layouts responsivos, sem a necessidade a definição de valores fixos.



### Requisitos Básicos

- Ter feito o curso de "Introdução a criação de websites com HTML5 e CSS3"
- Editor de texto
- Navegador de Internet



### Percurso

- **Aula1** Introdução ao Flexbox
- **Aula2** Fundamentos do Flexbox
- **Aula3** Projeto Integrador



### Objetivos da Aula 

1. Conhecer a estrutura básica
2. Entender a diferença entre Flex Container e Flex Item
3. Conhecer inicialmente algumas propriedades



### Suporte

​	Foi projetado como um modelo de layout unidimensional e com um método que pode oferecer distribuição de espaço entre itens em uma interface e recursos de alinhamento. Os navegadores abaixo já veem com esse suporte:

- Chrome 29.0
- Explorer 11.0
- FireFox 22.0
- Opera 48
- Safari 10



### Flex Container

​	É a tag que envolve os itens, será nela que iremos aplicar a propriedade "display: flex". Transforma todos os seus itens filhos em flex itens.

#### Propriedades relacionadas:

* **display** É o inicializador do container.
* **flex-direction** Responsável por fazer o direcionamento desses itens (horizontal ou vertical).
* **flex-wrap** Responsável pela quebra de linha.
* **flex-flow** Que é uma abreviação do direction e o wrap.
* **justify-content** Responsável por alinhar os itens do container de acordo com sua direção.
* **align-items** Responsável por alinhar os itens de acordo com o eixo do container.
* **align-content** Responsável por alinhar as linhas do container.



### Flex Item

​	São os elementos filhos diretos dos Flex Container. E também podem se tornar Flex Container.

#### Propriedades relacionadas:

- **flex-grow -** Define a proporcionalidade de crescimentos dos itens, respeitando o tamanho de seus conteúdos internos.

  OBS: não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container. 

- **flax-basis -** É a propriedade que estabelece o tamanho inicial do item antes da distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

  **Valores possíveis**

  **auto:**  caso o item não tenha tamanho, este será proporcional ao conteúdo do item.

  **px, %, em,...:** são valores exatos previamente definidos.

  **0(zero):**  terá relação com a definição do flex-grow.

- **flex-shrink -** É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.

- **flex -** Esta propriedade é um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis.

- **order -** Esta propriedade é responsável por ordenar nossos itens.

- **align-self -** É a propriedade que estabelece o alinhamento de modo individual sobre um determinado item.

  **Valores possíveis**

  **auto:** valor padrão, irá respeitar a definição de align-items do container.

  **flex-start:** ao início do container.

  **flex-end:** ao final do container.

  **center:** relativo ao centro de acordo com o eixo.

  **stretch:** ocupa todos os espaços relativos.

  **baseline:** utiliza a linha base da tipografia.


### Fundamentos  

**Objetivos da aula**

1. Conhecer e aplicar a propriedade de inicialização do flex container.

**Display: flex** Torna suas tags(h1~h6, a, p, span e etc) um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos destas tags, tornam-se flex items.



**Objetivos da aula**

1. Entender o comportamento padrão de orientação horizontal de um flex container.
2. Aprender a modificar a orientação horizontal.

**Flex-direction** É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

**Eixos** 

- **row -** É o padrão, direção de texto , da esquerda para a direita.
- **row-reverse -** Altera a direção dos nossos itens, agora da direita para a esquerda.
- **column -** Ordena de cima para baixo em um eixo vertical, colocando nossos itens em coluna única.
- **column-reverse -** Altera a direção dos nossos itens, agora ordena de baixo para cima.



**Flex-wrap** É a propriedade que define se os itens devem ou não quebrar a linha. Por padrão eles não quebram linhas, isso faz com que os flex itens sejam compactados além do limite do conteúdo.

- **nowrap -** É o padrão, não permite a quebra de linhas. Se houver muitos itens dentro de nosso container, pode ocorrer o vazamento desses itens caso nosso container seja usado além do máximo estipulado.
- **wrap -** Permite a quebra de linha, assim que um dos flex itens não puder mais ser compactado, os próximos itens passam para a linha de baixo, impedindo assim o vazamento destes.
- **wrap-reverse -** Também permite a quebra de linha, o que muda é que agora eles serão organizados de modo inverso, de baixo para cima.



**Flex-flow** É um atalho para as propriedades **flex-direction** e **flex-wrap**. Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é o nowrap.



**Justify-content** Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.

**OBS:** Caso seus itens esteja ocupando 100% de todo o container, ela não se aplica.

**As variações**

* **flex-start:** início do container.
* **flex-end:** final do container.
* **center:** ao centro do container.
* **space-between:** cria um espaçamento igual entre os elementos.
* **space-around:** os espaçamentos do meio são duas vezes maiores que o inicial e final.



**Align-items** Trata do alinhamento dos flex itens de acordo com o eixo do container. O alinhamento é diferente para quando os itens estão em colunas ou linhas. Essa propriedade permite o alinhamento central do eixo vertical.

**Tipos de alinhamento** 

* **center** Alinhamento dos itens ao centro.
* **stretch** É o padrão, e os flex itens crescem igualmente.
* **flex-start** Alinhamento dos itens no início.
* **flex-end** Alinhamento dos itens no final.
* **baseline** Alinhamento de acordo com a linha base da tipografia dos itens.