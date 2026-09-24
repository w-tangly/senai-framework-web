# 1. Introdução ao CSS (Cascading Style Sheets)
O CSS é a linguagem responsável por definir o estilo, layout, cores, fontes, margens, alinhamentos e responsividade de páginas web. Ele segue a estrutura básica:
$$\text{seletor } \{ \text{propriedade: valor;} \}$$

* **Seletor:** Indica a tag HTML ou elemento onde a regra será aplicada.
* **Propriedade:** O atributo a ser modificado (ex: `background-color`, `color`, `font-size`).
* **Valor:** A configuração desejada (ex: `#FF0000`, `16px`).

## Formas de Aplicação do CSS
1. **In-line:** Aplicado diretamente na tag HTML usando o atributo `style`. Recomendado apenas para testes rápidos ou ajustes pontuais.
2. **Interno:** Definido dentro da tag `<style>` no cabeçalho (`<head>`) do documento HTML. Ideal para páginas únicas.
3. **Externo:** Escrito em um arquivo separado com extensão `.css` e vinculado ao HTML via a tag `<link>`. **É a abordagem mais recomendada** para projetos maiores, promovendo organização e reutilização.

---

# 2. Principais Propriedades do CSS
* `color`: Define a cor do texto.
* `background-color`: Define a cor de fundo do elemento.
* `font-family`: Especifica a família da fonte tipográfica.
* `font-size`: Controla o tamanho do texto (em `px`, `rem`, `%`, etc.).
* `margin`: Controla o espaçamento *externo* (fora das bordas do elemento).
* `padding`: Controla o preenchimento *interno* (entre a borda e o conteúdo).
* `border`: Define espessura, estilo e cor da borda.
* `width` e `height`: Controlam a largura e a altura de um elemento.
* `display`: Define como o elemento é renderizado (ex: `block`, `inline`, `flex`).
* `position`: Define o método de posicionamento (`static`, `relative`, `absolute`, `fixed`).
* `text-align`: Controla o alinhamento horizontal do texto.

## Seletores Especiais: Class e ID
* **Classes (`.`):** Permitem aplicar o mesmo conjunto de estilos a múltiplos elementos, garantindo consistência visual.
* **IDs (`#`):** Utilizados para estilizar elementos únicos e específicos de uma página, permitindo também navegação por âncoras e manipulação precisa via JavaScript.

---

# 3. O Box Model (Modelo de Caixas)
O *Box Model* descreve os blocos gerados por elementos HTML na página e gerencia o dimensionamento e espaçamento através de quatro camadas principais:
1. **Content:** A área central onde aparecem textos e imagens (dimensões de largura e altura).
2. **Padding:** O espaço interno entre o conteúdo e a borda.
3. **Border:** A linha que envolve o conteúdo e o padding.
4. **Margin:** O espaço externo que separa o elemento dos demais vizinhos na página.

* **Vantagens de uso:** Facilita o controle de tamanhos, evita sobreposições, organiza visualmente a interface e ajuda na adaptação para diferentes tamanhos de tela.

---

# 4. Layouts Flexíveis com Flexbox
O **Flexbox** (*Flexible Box Layout*) é um módulo de layout unidimensional projetado para organizar itens eficientemente em linhas ou colunas, oferecendo alinhamento e distribuição automática de espaços.

## Principais Propriedades do Flexbox (Aplicadas no Container):
* `flex-direction`: Define o eixo principal (`row`, `column`, `row-reverse`, `column-reverse`).
* `justify-content`: Alinha os itens ao longo do **eixo principal** (ex: `flex-start`, `center`, `flex-end`, `space-between`, `space-around`, `space-evenly`).
* `align-items`: Alinha os itens ao longo do **eixo transversal** (ex: `flex-start`, `center`, `flex-end`, `stretch`, `baseline`).
* `flex-wrap`: Controla se os itens devem quebrar para uma nova linha (`nowrap`, `wrap`, `wrap-reverse`).
* `gap`: Define o espaçamento direto entre os itens flexíveis.

---

# 5. Layouts Responsivos
Técnica de design que adapta automaticamente o conteúdo para diferentes tamanhos de tela (smartphones, tablets e desktops), melhorando a experiência do usuário (UX) e a usabilidade.  
* **Tag essencial para responsividade mobile:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

# 6. Introdução aos Frameworks CSS
Um **framework CSS** é um conjunto pré-fabricado de recursos, padrões, classes utilitárias e componentes prontos que agilizam e padronizam o desenvolvimento de interfaces web.

## Os Três Pilares de um Framework:
1. **Layout:** Grid, Flexbox e responsividade.
2. **Estilos:** Cores, espaçamentos e tipografia.
3. **Componentes:** Botões, cards, barras de navegação (*navbars*), etc.

---

# 7. Tailwind CSS (Abordagem Utility-First)
O **Tailwind CSS** é um framework baseado no conceito **Utility-First** (utilitário em primeiro lugar). Em vez de fornecer componentes prontos fechados, ele fornece pequenas classes atômicas que possuem uma única responsabilidade específica, permitindo combiná-las diretamente no HTML para construir interfaces customizadas.

## Vantagens do Tailwind CSS:
* Reduz o tempo de desenvolvimento.
* Aumenta a flexibilidade visual sem criar arquivos CSS inchados.
* Facilita a padronização e o design responsivo (*Mobile First*).

## Exemplo Prático de Utility-First:
```html
<button class="bg-blue-600 text-white px-6 py-3 rounded-lg font-bold">
  Enviar
</button>
```
* `bg-blue-600`: Cor de fundo azul.
* `text-white`: Cor do texto branca.
* `px-6 py-3`: Padding horizontal e vertical.
* `rounded-lg`: Bordas arredondadas.
* `font-bold`: Texto em negrito.

## Formas de Importação/Uso:
1. **Play CDN (Ideal para testes rápidos):**
   ```html
   <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
   ```
2. **Tailwind CLI / PostCSS:** Integração robusta via Node.js (`npm install tailwindcss @tailwindcss/cli`) para projetos em produção e frameworks modernos (Next.js, Angular, Laravel).
3. **Tailwind CSS IntelliSense:** Extensão recomendada para editores (como VS Code) que oferece autocompletar inteligente e visualização prévia das classes utilitárias.
