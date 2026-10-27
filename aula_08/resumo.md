# Aula 08 — Projeto React

A aula revisa fundamentos de JavaScript e apresenta conceitos essenciais do React para organizar interfaces em componentes reutilizáveis e atualizá-las conforme os dados.

## Revisão de JavaScript

Foram retomados variáveis (`const` e `let`), tipos de dados, operadores, condicionais, repetições, funções, arrays e objetos. Também foi revisada a manipulação do DOM: selecionar elementos, responder a eventos e alterar conteúdo. No React, em vez de modificar a página manualmente, descrevemos a interface com base nos dados e deixamos o React coordenar as atualizações.

## Conceitos fundamentais do React

- **JSX:** extensão de sintaxe que permite escrever estruturas semelhantes a HTML no JavaScript. Expressões são inseridas entre chaves, como `{nome}`. Em JSX, use `className` no lugar de `class`, `htmlFor` no lugar de `for` e feche elementos sem conteúdo, como `<img />`.
- **Componentes:** funções com nomes iniciados em letra maiúscula que retornam elementos React. Dividir a tela em componentes menores facilita a leitura, a organização e a reutilização.
- **Props:** dados enviados de um componente pai para um componente filho. Permitem manter uma estrutura reutilizável e variar seu conteúdo; o filho recebe esses valores e os apresenta.
- **DOM e atualizações:** o DOM representa a estrutura da página no navegador. O React usa descrições da interface e um processo de renderização e reconciliação para identificar e aplicar as mudanças necessárias, sem exigir que o desenvolvedor atualize cada elemento manualmente.
- **Listas e `key`:** o método `map()` transforma cada item de um array em elementos de interface. Cada item deve receber uma `key` estável — normalmente seu identificador — para que o React possa reconhecê-lo quando a lista muda. `filter()` pode selecionar os dados antes da renderização.
- **Renderização condicional:** permite mostrar interfaces diferentes conforme props, dados ou estado. Pode ser feita com `if` e `return` para caminhos distintos, ou com o operador ternário para alternar conteúdo de forma simples.

```jsx
function ListaResultados({ resultados, carregando }) {
  if (carregando) return <p>Carregando...</p>;
  if (resultados.length === 0) return <p>Nenhum resultado encontrado.</p>;

  return (
    <ul>
      {resultados.map((resultado) => (
        <li key={resultado.id}>{resultado.nome}</li>
      ))}
    </ul>
  );
}
```

## Atividade proposta

Desenvolver uma aplicação React que reúna JSX, componentes, props, listas com chaves e renderização condicional. O projeto deve ser publicado em um repositório público no GitHub, acompanhado de um README que descreva a aplicação, suas funcionalidades e os conceitos utilizados.
