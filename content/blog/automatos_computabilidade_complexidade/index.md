---
title: Autômatos, Computabilidade e Complexidade
subtitle:

# Summary for listings and search engines
summary: Introdução a três áreas centrais da teoria da computação.

# Link this post with a project
projects: []

# Date published
date: "2022-08-24T18:00:00Z"

# Date updated
lastmod: "2022-08-24T18:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Allow visitors to make improvements to the page?
# Requires a repository to be configured in `params.yaml`
editable: true

authors:
- admin

tags: ["teoria", "computação"]

categories: ["computação"]

---
> Quais são as capacidade e limitações fundamentais dos computadores?

Essa questão vai lá atrás nos anos 1930's quando os primeiros lógicos e matemáticos começaram a explorar o significado de computação. Os avanços tecnológicos têm aumentado enormemente nossa capacidade de computar e tem trazido essa questão do domínio da teoria para o mundo do interesse prático.

Em cada uma das três áreas --- autômatos, computabilidade e complexidade --- essa questão é interpretada diferentemente, e as respostas variam conforme a interpretação de cada área.

## Teoria da Complexidade
> O que faz alguns problemas computacionalmente difíceis e outros fáceis?

Essa é a questão central da teoria da complexidade. Notavelmente, não sabemos a resposta para ela, embora ela tenha sido intensamente pesquisada durante os últimos 35 anos.

Em uma das importantes conquistas da teoria da complexidade até agora, pesquisadores descobriram um elegante esquema para classificar problemas conforme sua dificuldade computacional. Usando esse esquema, podemos demonstrar um método para dar evidência de que certos problemas são computacionalmente difíceis, ainda que sejamos incapazes de provar que eles o são.

Temos varias opções quando deparamos com um problema que parece ser computacionalmente difícil. Primeiro, entendendo qual aspecto do problema e a raiz da dificuldade, podemos ser capazes de alterá-lo de modo que o problema seja mais facilmente solúvel. Segundo, podemos nos contentar com uma solução menos perfeita para o problema. Em certos casos encontrar soluções que apenas se aproximam da solução perfeita é relativamente fácil. Terceiro, alguns problemas são difíceis somente no pior caso, porém fáceis na maior parte do tempo. Dependendo da aplicação, você pode ficar satisfeito com um procedimento que ocasionalmente seja lento, mas usualmente roda rapidamente. Finalmente, você pode considerar tipos alternativos de computação, tais como computação aleatorizada ou métodos de meta-heurísticas que podem acelerar certas tarefas ou encontrar uma solução satisfatória.

## Teoria da Computabilidade
Durante a primeira metade do século XX, matemáticos como Kurt Gödel, Alan Turing e Alonzo Church descobriram que certos problemas não podem ser resolvidos por computadores. Um exemplo desse fenômeno é o problema de determinar se um enunciado matemático é verdadeiro ou falso. Essa tarefa é o feijão com arroz dos matemáticos. Parece uma questão natural para resolução por computador, porque ela reside estritamente no domínio da matemática. Mas nenhum algoritmo de computador pode realizar essa tarefa. 

Entre as consequências desse resultado estava o desenvolvimento de ideias concernentes a modelos teóricos de computadores, que em algum momento ajudariam a levar a construção de computadores reais.

As teorias da computabilidade e da complexidade estão intimamente relacionados. Na teoria da complexidade, o objetivo é classificar problemas como fáceis e difíceis, enquanto que na teoria da computabilidade a classificação de problemas é por meio da separação entre os que são solúveis e os que não são. A teoria da computabilidade introduz vários dos conceitos usados na teoria da complexidade.

## Teoria dos Autômatos
Teoria dos autômatos lida com as definições e propriedades de modelos matemáticos de computação. Esses modelos desempenham um papel em diversas áreas aplicadas da ciência da computação. Um modelo, chamado _aotômato finito_, é usado em processamento de texto, compiladores e projeto de hardware. Um outro modelo, chamado _gramática livre de contexto_ é usado em linguagens de programação e inteligência artificial.

Teoria dos autômatos é um excelente lugar para começar a estudar a teoria da computação. As teorias de computabilidade e complexidade requerem uma definição precisa de um _computador_. A teoria dos autômatos permite praticar com definições formais de computação pois ela introduz conceitos relevantes a outras áreas não teóricas da ciência da computação.