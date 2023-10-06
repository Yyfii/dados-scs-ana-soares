# Teste de Dados (dados-scs-ana-soares)
Teste de dados SCS - Smart Creative Solutions
##
# Desafio 
#
* Será que nossos diferentes lojistas associados conseguem manter o preço do mesmo produto sem grandes discrepâncias?
  ##
    Primeiramente, para responder a esse questionamento, irei mostrar um gráfico, feito a partir da amostra de um produto e o  preço que cada lojista atribuiu:
   ![image](https://github.com/Yyfii/dados-scs-ana-soares/assets/125479516/d2fef7ba-a8c1-40eb-971f-140024d85f63)
  É possível inferir de acordo com o gráfico que há uma variação aproximadamente nos intervalos de 74 para 90 na faixa de preços de um mesmo produto, do qual foram analisados o preço de 488 pedidos de diferentes lojistas.
  
   - Total de pedidos do mesmo produto: 488
   - Faturamento do produto sem frete: R$ 43025,56
   - Faturamento de frete            : R$ 8046,04
   - Faturamento total               : R$ 51071.6

   
   Analisando também os dados de algumas outras amostras aleatórias, que receberam diferentes pedidos:
   
   ![image](https://github.com/Yyfii/dados-scs-ana-soares/assets/125479516/ec244a98-b9f4-4e60-86bf-40932b2eef17)

    Percebe-se que o produto foi vendido nove vezes pelo mesmo vendedor, entretanto com preços diferentes.
   
* Podemos dar os mesmos benefícios para todos os lojistas (sellers)? Ou existe algum que merece destaque?

  A partir da análise de dados constatou-se qual o lojista que mais recebeu pedidos, o ['id_vendedor'] == '6560211a19b47992c3666cc44a7e94c0'], com um total de 2033 pedidos.
  
  ![image](https://github.com/Yyfii/dados-scs-ana-soares/assets/125479516/d6599c44-57cb-4aaa-a601-9277570f713f)

* Existe diferença no valor do frete praticado em regiões/cidades diferentes? Ou podemos aplicar as mesmas regras de subsídio de frete para qualquer localidade?
  
   Sim, de acordo com os dados existentes e alguns testes feitos com os mesmos, é possível constatar variações nos fretes de diferentes localidades. Podemos aplicar as mesmas regras, mas não o mesmo valor, já que o frete é calculado a partir do:
    -origem e destino da entrega;
    -tamanho da embalagem;
    -peso da mercadoria;
    -prazo de envio
  
    Então o frete deve ser calculado analisando a origem e o destino, as medidas do produto e também o tempo de envio. O mercado livre por exemplo, apresenta uma variação no preço dependendo do tempo de entrega, o cliente pode escolher entre uma entrega mais rápida 
 com um preço maior ou uma entrega com o tempo normal e o preço padrão.

* Será que nosso catálogo de produtos é abrangente? Ou tem foco em categorias específicas?
   
   A partir da base de dados é possível constatar categorias que possuem mais produtos cadastrados:

    - cama_mesa_banho                3029
    - esporte_lazer                  2867
    - moveis_decoracao               2657
    - beleza_saude                   2444
    - utilidades_domesticas          2335
      ...
    - fashion_roupa_infanto_juvenil  5
    - casa_comforto                  2
    - pc_gamer                       3
    - seguros_servicos               2
    - cds_dvds_musicais              1

  É possível inferir, portanto, que o catálogo é mais focado em produtos de bem estar, comforto, saúde e beleza.
  

* Será que sempre vendemos os mesmos produtos? Ou existem sazonalidades?
  
  Existem sazonalidades, é possível destacar quais os tipos de produtos que são mais vendidos, veja a seguir:
    
  - moveis_decoracao   527 
  - casa_mesa_banho    488
    
* Será que existe um modelo preditivo para nos preparar para o futuro?
  
   O modelo preditivo  supervisionado é indicado, ele pode ser desenvolvido da seguinte forma:
  
    - Identificando o objetivo que se tem com esse modelo preditivo
    - Coletando exemplos relacionados a/ao area/dominio/negócio
    - Fazendo uma análise(descritiva inicial)
    - Selecionar os algoritmos/ferramentas de machine learning que serão utilizadas
    - Utilizar esse algoritmo/ferramenta para criar o modelo preditivo
    - Analisar esses modelos criados
    - Escolher o que se portou melhor
    - Colocar em produção
    - Monitorar como o modelo se comporta, por isso que é necessário saber o que o modelo deve fazer,supervisionado, por que ao saber como ele deveria se comportar e como ele se comporta, pode-se medir a eficácia do modelo.
 
      
* Será que o atual banco de dados vai suportar o nosso crescimento? Ou existe uma opção mais escalável?
  
   Como a atual situação do marketplace é o big data, existem sim opções, como o hadoop e também prezar pela  qualidade dos dados, dados que podem virar insights relevantes para as tomadas de decisão.

#
## Outras constatações

* A concentração dos clientes:

  - SP    41746
  - RJ    12852
  - MG    11635
  - RS     5466
  - PR     5045
  - SC     3637
  - BA     3380
  - DF     2140
  - ES     2033
  - GO     2020
  - PE     1652
  - CE     1336
  - PA      975
  - MT      907
  - MA      747
  - MS      715
  - PB      536
  - PI      495
  - RN      485
  - AL      413
  - SE      350
  - TO      280
  - RO      253S
  - AM      148
  - AC       81
  - AP       68
  - RR       46
  
* Formas de pagamentos mais utilizadas:
  
   - Cartão de crédito  76795
   - Boleto             19784
   - Voucher            5775
   - Cartão de debito   1529
   - Indefinida         3
     
* A concentração dos vendedores:

  ![image](https://github.com/Yyfii/dados-scs-ana-soares/assets/125479516/3e23dbd3-80fa-44d7-8181-2ba0250396d6)

## Fontes

FGV. Introdução à Ciência de Dados. 2023. Disponível em: https://educacao-executiva.fgv.br/cursos/online/curta-media-duracao-online/introducao-ciencia-de-dados

DESCHAMPS, Felipe. Inteligência Artificial + Machine Learning + Data Science + Deep Learning. 2020. Disponível em: https://www.youtube.com/playlist?list=PLMdYygf53DP7YZiFUtGTWJJlvynRyrna-

Programação Hashtag. Introdução ao Pandas no Python - [SAIA DO ZERO EM 1 AULA]. 2021. Disponível em: https://www.youtube.com/watch?v=C0aj3FjN5e0

Programação Hashtag. Como Trabalhar com Arquivos CSV no Python. 2022. Disponível em: https://www.youtube.com/watch?v=AnJPtKLtc7o

Programação Hashtag. Curso de Python. 2022. Disponível em: https://www.youtube.com/playlist?list=PLpdAy0tYrnKyCZsE-ifaLV1xnkXBE9n7T

Programação Hashtag. Análise Exploratória IMPRESSIONADORA em Python.2022. Disponível em: https://www.youtube.com/watch?v=4sxhE3wP3Ug

Programação Hashtag.Introdução a Análise de Dados com Python - [Primeiros Passos] .2021. Disponível em: https://www.youtube.com/watch?v=kCMaqla6GrsM

PLOTLY. Disponível em: https://plotly.com/graphing-libraries/

Teste Prático. Disponível em: https://github.com/olist/work-at-olist-data/tree/master

##
