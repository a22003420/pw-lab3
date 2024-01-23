**Escola Comércio Lisboa (ECL), Programação Web, 23-24**
 
# Lab 3: *Layouts baseados em flex e grid* 

## Objetivos
* Aplicar os conceitos aprendidos de propriedades CSS, em especial flexbox e grid.

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. 
* Se tiver alguma dúvida:
    * Perguntar ao professor
    * Usar este link para apoio: https://www.w3schools.com/css/

## Pré-requisitos
* Deverá ter o VSCode instalado para editar o código HTML de forma fácil.
* Deverá ter instalado o git no seu computador.
* explore os exercícios do tutorial [Flexbox froggy](https://flexboxfroggy.com/)


# 1. Flex 
* cria uma pasta com o nome lab3.
* Irá criar uma página index.html onde explorará a propriedade <code>display:flex</code>
* crie um ficheiro CSS à parte, para estilizar esta página
* escolha uma fonte Google que goste, inclua o link para esta e utilize-a em todo o website, definindo um seletor universal <code>*</code> e propriedade <code>font-family</code> 
* especifique no style sempre <code>* {box-sizing: border-box; padding: 0; margin: 0;}</code>

### 1.1. Elemento centrado usando <code>flex</code>

* Crie um elemento div que tenha largura 100vw e altura 50vh
* atribua-lhe uma cor de fundo
* coloque dentro do div um parágrafo <code>p</code> com a palavra 'Viajar' ou outra palavra ou frase que queira e centre-a no div, usando CSS flex.
* Configure o tamanho do emoji com a propriedade font-size


### 1.2. Imagem com texto usando <code>position</code>

<img src="https://user-images.githubusercontent.com/42048382/221723524-823851af-f4c9-467c-8d6f-3e3857dbbeed.png" width="300px">

* Escolha uma imagem. Pode usar o [Unsplash](https://unsplash.com/), repositório de imagems de uso livre de onde pode usar: 
   * **imagem aleatória** de acordo com termos de pesquisa e tamanho especificado. Por exemplo, para as palavras "beach sand", 600x400, especifica-se https://source.unsplash.com/random/600×400/?beach,sand. Cada vez que refrescar a sua página terá uma imagem diferente.
   * **escolher imagem**. Escolha uma imagem (das free) clique nela e copie do URL o código (unsplash.com/photos/**xg8z_KhSorQ**). Pode especificar a dimensão que pretende (e.g., 300x200). Construa o hiperlink: https://source.unsplash.com/xg8z_KhSorQ/300x200
* Crie um elemento div com <code>position:relative</code> e contendo um elemento com a imagem <code>img</code> e um elemento parágrafo <code>p</code>.
* dimensione a imagem com largura 100%, <code>width:100%</code> por forma a ocupar toda a largura do browser.
* coloque uma frase sobre a imagem usando as propriedades <code>position:absolute</code> e especificando a posição em relação ao topo <code>top</code> e lado esquerdo <code>left</code>. Escolha uma cor para o texto que contraste bem com o fundo.
* Se tiver dúvidas, veja o [video-tutorial: posicionamento de elementos e seletores vários](https://educast.fccn.pt/vod/clips/1tmk0lmtww/html5.html?locale=en)


### 1.3. Capitais europeias usando <code>flex</code>

![image](https://user-images.githubusercontent.com/42048382/158489558-8f31368d-e15b-4a32-82c8-683ac6b2b482.png)

Usando uma flexbox (propriedade <code>display: flex</code>) crie um elemento flex que replique o layout acima. O código a implementar está em baixo, explicado a seguir:
* crie uma pasta images para a qual extraia as imagens de capitais europeias contidas no ficheiro [ZIP](https://github.com/ULHT-PW/pw23-lab3/blob/main/capitais.zip) 
* Crie um *container* flex (elemento <code>div</code> com classe *capitais*, com a propriedade <code>display: flex</code>)) e contendo um conjunto de items <code>div</code> 
* configure o container por forma a ter uma cor de fundo clara  
* os items serão um conjunto de elementos <code>div</code>. Cada um será alusivo a uma capital europeia tal como se descreve a seguir.
* cada item <code>div</code> deverá conter dois elementos <code>div</code>, um com a imagem, e outro com um parágrafo com o nome da capital. 
* configure os div dentro do container (recorrendo à composição de selectores <code>.container div</code>) por forma a terem uma borda e cantos arredondados 
* dentro de cada <code>div</code> coloque a imagem do lado esquerdo e do lado direito um parágrafo com o nome da cidade. para tal, configure ambos com a propriedade <code>display: inline-block</code>
* explore as propriedades <code>flex-flow</code> e <code>justify-content</code> e <code>align-items</code> para configurar adequadamente as imagens. Garanta espaçamento entre estas, usando a propriedade <code>margin</code>. 

![image](https://user-images.githubusercontent.com/42048382/158496390-ad99c24c-dfe8-4030-b662-244a9eaec457.png)

### 1.4. Propriedades CSS <code>flex</code>

Crie um div onde explora dentro deste as propriedades:
* crie um conjunto de círculos: crie elemento quadrado, esolha cor de fundo, e defina border-radius = sua largura... 😀). coloque uma palavra centrada, usando flex.
* aplique clip a uma imagem
* z-index
* display:hidden e hover (quando passa com o rato por cima, desaparece)

### 1.5. Cabeçalho <code>header</code> com <code>position:sticky</code>

* Crie um cabeçalho, elemento <code>header</code>, fixo com a propriedade <code>position:sticky</code>
* O <code>header</code> deverá conter:
    * <code>h1</code> com um título do lado esquerdo 
    * <code>nav</code> com 
        * links "ancora" para as várias partes da página, definindo id para cada uma das partes anteriores. 
        * link para uma das páginas da próxima secção grid.
* O <code>header</code>, configure com <code>display:flex</code>, e faça com que o titulo e nav fiquem cada um encostado a uma lado, com a propriedade <code>justify-content:space-between</code>
* Escolha uma cor de fundo <code>background</code> e do texto <code>color</code> que goste.
* estilize os hiperlinks <code>a</code> do nav com as seguintes propriedades:
    * <code>padding:20px</code> para que haja espaço à volta de cada palavra
    * remova a formatação de hiperlink do texto (sublinhado azul), com <code>text-decoration: none</code>.
    * escolha uma cor para a fonte
    * estilize o que acontece quando passa por cima do menu. PAra tal, deverá definir o selector <code>a:hover</code> com as seguintes propriedades:
        * associe uma cor de fundo, cinza claro, quando passa por cima do link com o rato
        * texto em bold, com  <code>font-weight: bold</code>


# 2. Páginas com diferentes layouts usando <code>grid</code>

* O segredo do CSS grid é:
    * dar um nome <code>grid-area</code> a cada elemento do layout  
    * no contentor grid, com a propriedade <code>displaygrid</code>, caracterizar:
        * <code>grid-template-areas</code>
        * <code>grid-template-columns</code> 
        * <code>grid-template-rows</code>.
    * Explore a combinação de unidades diferentes, fr, %, vw
* Se tiver dúvidas sobre CSS Grid, veja o [vídeo-tutorial: construindo um layout com CSS Grid](https://educast.fccn.pt/vod/clips/1qib570kz7/html5.html?locale=en) 
* Crie uma combinação de pelo menos 5 elementos semânticos HTML (header, nav, main, article, aside, footer...):
    * configure dois elementos com uma cor de fundo diferente e uma palavra a seu gosto
    * 2 com imagens de fundo, usando  <code>background-image:url(...)</code> e <code>background-size:cover</code>). 
    * um elemento <code>grid</code>
* faça 6 copias do ficheiro HTML, dando nomes diferentes.
* usando CSS grid, crie, com o mesmo conteúdo, 6 páginas com 6 layouts diferentes. Configure o CSS dentro do próprio html, no elemento style. Inspire-se nos [exemplos de layouts com 2 e 3 colunas](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Design_and_accessibility/Common_web_layouts) e invente.
* no <code>grid</code> insira 6 links (pode ser apenas um número) para cada uma das páginas, e um sexto para a página Flex. 

# 3. Submissão

1. Verifique que todos os links do seu website funcionam devidamente.
2. Crie um novo repositório GitHub público e carregue o seu laboratório 3 (Opção 1).
3. Pode enviar por e-mail para o Professor o código (Opção 2).


 # Fim ☀
 
Esperamos que tenha gostado de aplicar os conhecimentos para criar layouts com flexbox e CSS grid &#127760;!
