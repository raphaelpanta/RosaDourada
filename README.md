Versão em Português Brasileiro

A Brazilian Portuguese translation of GildedRose Kata [Original - In english](https://github.com/NotMyself/GildedRose)

##Rosa Dourada Kata de Refatoração

Olá e bem-vindo ao time Rosa Dourada. Como você sabe, somos uma
pequena pousada uma expendida localização em uma proeminente
cidade dirigida por um amigável administrador de pousadas chamado
Alisson. Nós, também, compramos e vendemos somente as mais excelentes
mercadorias. Infelizmente, nossas mercadorias estão em constante
degradação em qualidade ao passo em que se aproximam de seus prazos
de venda. Nós temos um sistema em produção que atualiza nosso inventário
para nós. Ele foi desenvolvido por um tipo sem-noção chamado Leeroy, o
qual seguiu adiante em novas aventuras. Sua tarefa é adicionar novos
recursos em nosso sistema para podermos dar início à venda de uma nova
categoria de itens. Em primeiro lugar, uma introdução a nosso sistema:

- Todos os itens tem um valor PrazoDeVenda o qual denota o número de dias que nós temos para vender aquele item
- Todos os itens tem um valor de Qualidade o qual denota o quanto valioso o item é
- Ao final de cada dia o sistema decrementa ambos os valores para cada item

Bem simples, certo? Bem, agora é que a coisa se torna ainda mais interessante:

- Após o prazo de venda passar, sua Qualidade será degradado duas vezes mais rápido
- A Qualidade de um item nunca deve ser negativa.
- "Queijo Brie Envelhecido" na verdade tem acréscimo de Qualidade quanto mais envelhecido ficar
- A Qualidade de um item não pode ser mais que 50
- "Sulfuras", sendo um item lendário, nunca pode ser vendido ou decrementado em Qualidade
- "Passes para os bastidores", como "Queijo Brie Envelhecido", aumenta em Qualidade ao passo que seu PrazoDeVenda se aproxima; Qualidade aumenta em 2 quando tem 10 ou menos dias de prazo e por 3 quando faltam 5 ou menos dias porém a Qualidade cai para 0 após o dia do Show.

Nós, recentemente contratamos um fornecedor de itens de invocação. Isto requer uma atualização
em nosso sistema:

- Itens "Invocáveis" degradam em Qualidade duas vezes mais rápido que os itens normais

Sinta-se livre para fazer quaisquer mudanças para o método AtualizarQualidade
e adicionar qualquer código novo desde de que tudo continue a trabalhar corretamente. Todavia,
não altere a classe Item ou suas propriedades pois ela pertence ao goblin lá no canto que entrará
em modo instantâneo de raiva e descarregara de uma vez em você pois, ele não acredita em código de
propriedade compartilhada (você pode fazer o método AtualizarQualidade e as propriedades
de Item static caso queira, nós iremos te dar cobertura para você).

Apenas para deixar claro, um item não pode ter sua Qualidade aumentada acima de 50,
porém "Sulfuras" é um item lendário e sua Qualidade é 80 e nunca se altera.

##Dando Início

Clone este repositório. Execute build.bat no Powershell. Se você ver uma saída similar
ao seguinte screenshot, você estará pronto para dar início as suas refatorações.

![alt text](images/build_output.png "Saída com a Build em bom estado")

##Quem, O que e O Porquê?
Quem: [@TerryHughes](https://twitter.com/TerryHughes), [@NotMyself](https://twitter.com/NotMyself)

O que e o Porquê : [Refatore isto: O Kata Gilded Rose](http://iamnotmyself.com/2011/02/13/refactor-this-the-gilded-rose-kata/)

Tradução: Raphael Pantaleão - www.github.com/raphaelpanta
