---
title: Algoritmos de Ordenação
subtitle:

# Summary for listings and search engines
summary: Estudo sobre os algoritmos de ordenação.

# Link this post with a project
projects: []

# Date published
date: "2022-08-25T12:00:00Z"

# Date updated
lastmod: "2022-08-25T12:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Allow visitors to make improvements to the page?
# Requires a repository to be configured in `params.yaml`
editable: true

authors:
- admin

tags: ["teoria", "computação", "algoritmo", "ordenação"]

categories: ["computação"]

---
Ordenação é um problema que surge com frequência e oferece um solo fértil para a apresentação de muitas técnicas de projeto e ferramentas de análise padronizadas. Sendo uma operação fundamental da ciência da computação e, por isso, há um grande número de bons algoritmos de ordenação à nossa disposição. O melhor algoritmo para determinada aplicação depende --- entre outros fatos --- do número de itens a ordenar, do grau de ordenação já apresentado por esses itens, das possíveis restrições aos valores dos itens, da arquitetura do computador e do tipo de dispositivo de armazenamento que será utilizado. Estudares um conjunto de algoritmos de ordenação e iremos implementá-los na linguagem de programação C.

### Ordenação por Inserção
O algoritmo de ordenação por inserção é eficiente para ordenar um número pequeno de elementos. A ordenação por inserção funciona da maneira como muitas pessoas ordenam as cartas em um jogo de baralho. Iniciamos com a mão esquerda vazia e as cartas viradas para baixo, na mesa. Em seguida, retiramos uma carta de cada vez da mesa e a inserimos na posição correta na mão esquerda. Para encontrar a posição correta para uma carta, nós a comparamos com cada uma das cartas que já estão na mão, da direita para a esquerda. Em todas as vezes, as cartas que seguramos na mão esquerda são ordenadas, e essas cartas eram as que estavam na parte superior da pilha sobre a mesa.

Como visto na definição de [algoritmos]({{< ref "/blog/algoritmo" >}} "Algoritmos") temos como entrada e saída:

**Entrada:** Uma sequência de {{< math >}}$ n ${{< /math >}} números {{< math >}}$\langle a_1, a_2, \dots, a_n \rangle${{< /math >}}.

**Saída:** Uma permutação (reordenada) {{< math >}}$\langle a'_1, a'_2, \dots, a'_n \rangle${{< /math >}} da sequência de entrada, tal que {{< math >}}$ a'_1 \leq a'_2 \leq \dotsc \leq a'_n ${{< /math >}}.

Os números que desejamos ordenar também são conhecidos como **_chaves_**. Embora conceitualmente estejamos ordenando uma sequência, a entrada é dada na forma de um arranjo com {{< math >}}$ n ${{< /math >}} elementos.

Implementação em C:
```c
void ordenacao_insercao(int* vetor, int tamanho_vetor) {
    int i, j, chave;

    for(i = 1; i < tamanho_vetor; i++) { 
        chave = vetor[i]; 
        j = i - 1;

        while(j >= 0 && vetor[j] > chave) { 
            vetor[j + 1] = vetor[j];
            j--;
        }

        vetor[j + 1] = chave;
    } 
}
```
O algoritmo recebe como entrada um vetor e o tamanho do vetor. O algoritmo ordena os números da entrada no lugar da seguinte forma: reorganiza os números dentro do vetor, com no máximo um número constante deles armazenado fora do vetor em qualquer instante. O vetor conterá a sequência de saída ordenada quando terminar.