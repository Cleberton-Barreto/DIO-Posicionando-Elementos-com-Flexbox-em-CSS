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

* **display**
* **flex-direction**
* **flex-wrap**
* **flex-flow**
* **justify-content**
* **align-items**
* **align-content**



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

- **align-self -** 



### Fundamentos // parte 1 - Flex Container 

**Display Flex** - 