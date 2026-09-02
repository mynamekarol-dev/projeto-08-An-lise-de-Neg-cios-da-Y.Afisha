#  — Projeto: Análise de Negócios da Y.Afisha

## Sobre o projeto

Neste projeto, trabalhei como analista no departamento de análise da **Y.Afisha**, com o objetivo de entender melhor o comportamento dos usuários e verificar se os investimentos em marketing estavam trazendo bons resultados para a empresa.

Para isso, utilizei dados de acessos ao site, pedidos realizados pelos usuários e despesas com marketing entre **janeiro de 2017 e dezembro de 2018**.

Durante a análise, procurei entender como os usuários utilizavam o produto, quando começavam a realizar compras, quanto cada cliente gerava de receita e quanto tempo era necessário para que os investimentos em marketing fossem recuperados.

---

## Objetivos

Neste projeto, meus principais objetivos foram:

* analisar o comportamento dos usuários no site;
* identificar a quantidade de usuários por dia, semana e mês;
* analisar a duração das sessões;
* entender com que frequência os usuários retornavam;
* descobrir quanto tempo os usuários levavam para realizar a primeira compra;
* analisar a quantidade de pedidos realizados;
* calcular o tamanho médio das compras;
* calcular o LTV dos clientes;
* analisar os gastos com marketing;
* calcular o CAC por origem de anúncio;
* avaliar o retorno dos investimentos por meio do ROI;
* comparar os resultados entre dispositivos e origens de anúncios;
* identificar quais origens de marketing apresentavam melhores resultados;
* fazer recomendações sobre onde seria mais interessante investir.

---

# 1. Preparação dos dados

Primeiramente, carreguei os três conjuntos de dados que seriam utilizados na análise:

* `visits_log_us.csv`
* `orders_log_us.csv`
* `costs_us.csv`

Depois de importar os arquivos, comecei verificando a estrutura dos DataFrames, a quantidade de registros, os nomes das colunas e os tipos de dados.

Também analisei possíveis valores ausentes e inconsistências.

Como os dados possuem informações de datas e horários, converti as colunas correspondentes para o formato adequado de data e hora. Isso foi importante para conseguir calcular corretamente sessões, períodos de conversão, coortes e métricas ao longo do tempo.

Também procurei deixar os dados organizados e preparados para as etapas seguintes da análise.

---

# 2. Análise do produto

## Usuários por dia, semana e mês

Primeiramente, analisei a quantidade de usuários que acessavam o site em diferentes períodos.

Calculei o número de usuários únicos por:

* dia;
* semana;
* mês.

Essa análise me ajudou a entender como o tráfego do site se comportava ao longo do tempo e se existiam períodos com maior ou menor utilização.

---

## Número de sessões

Depois, analisei as sessões realizadas pelos usuários.

Uma pessoa poderia acessar o site mais de uma vez, então foi importante diferenciar o número de usuários do número de sessões.

Calculei a quantidade de sessões realizadas por dia para entender melhor a frequência de utilização do produto.

---

## Duração das sessões

Também calculei a duração das sessões utilizando os horários de início e fim registrados nos dados.

A partir disso, analisei quanto tempo, em média, os usuários permaneciam no site.

Também utilizei gráficos para visualizar a distribuição da duração das sessões e identificar possíveis diferenças ou comportamentos fora do padrão.

---

## Retorno dos usuários

Outra parte da análise foi verificar com que frequência os usuários voltavam ao site.

Analisei o comportamento dos usuários ao longo do tempo para entender melhor a retenção e identificar se os acessos eram apenas pontuais ou se os usuários continuavam utilizando o produto.

---

# 3. Análise das vendas

## Primeira compra e conversão

Depois de analisar o comportamento dos usuários, passei para a parte de vendas.

Meu primeiro objetivo foi descobrir **quando os usuários começavam a comprar**.

Para isso, relacionei os dados de visitas com os dados de pedidos e analisei o período entre o primeiro acesso/registro e a primeira compra.

Também organizei os usuários em grupos de acordo com o tempo necessário para realizar a conversão.

Essa análise ajudou a entender quanto tempo normalmente era necessário para um usuário se transformar em cliente.

---

## Quantidade de pedidos

Em seguida, analisei a quantidade de pedidos realizados pelos clientes durante os períodos observados.

Observei como os pedidos estavam distribuídos ao longo do tempo e também utilizei gráficos para identificar possíveis mudanças no comportamento de compra.

---

## Valor médio das compras

Também calculei o valor médio dos pedidos.

Essa métrica foi importante porque não basta analisar apenas a quantidade de clientes ou pedidos. Um cliente que realiza compras de maior valor pode representar uma receita maior para a empresa.

Por isso, comparei o volume de pedidos com a receita gerada.

---

# 4. LTV — Lifetime Value

Depois, calculei o **LTV (Lifetime Value)** para entender quanto de receita os clientes geravam para a empresa ao longo do tempo.

Para essa análise, utilizei os dados de receita dos pedidos e organizei os clientes em coortes.

A análise por coortes permitiu acompanhar o comportamento dos clientes adquiridos em diferentes períodos e comparar quanto de receita cada grupo gerava ao longo do tempo.

Também criei gráficos para visualizar a evolução do LTV.

---

# 5. Análise de marketing

## Gastos com marketing

Depois de analisar os usuários e as vendas, comecei a analisar os investimentos em marketing.

Utilizei o arquivo `costs_us.csv` para verificar quanto dinheiro foi gasto com as diferentes origens de anúncios.

Analisei os custos:

* no total;
* por origem de anúncio;
* ao longo do tempo.

Essa etapa foi importante para conseguir relacionar os gastos com os resultados obtidos nas vendas.

---

## CAC — Custo de aquisição de clientes

Em seguida, calculei o **CAC (Customer Acquisition Cost)** para cada origem de anúncio.

Essa métrica mostra quanto, em média, foi necessário gastar para adquirir um cliente.

Comparei o custo das diferentes origens com a quantidade de clientes que elas conseguiram trazer.

Dessa forma, consegui identificar quais origens tinham um custo de aquisição maior e quais conseguiam trazer clientes com um investimento menor.

---

## ROI — Retorno sobre o investimento

Por fim, analisei o **ROI (Return on Investment)** para avaliar se os investimentos realizados em marketing estavam trazendo retorno para a empresa.

Comparei os gastos de cada origem com a receita gerada pelos clientes adquiridos.

Essa foi uma das métricas mais importantes da análise, porque uma origem de anúncios pode trazer muitos usuários, mas isso não significa necessariamente que ela seja a mais lucrativa.

Por isso, considerei o ROI junto com outras métricas, como CAC e LTV.

---

# 6. Análise por dispositivo e origem de anúncio

Também comparei as principais métricas entre diferentes dispositivos e origens de anúncios.

Criei gráficos para visualizar as diferenças e entender melhor quais grupos apresentavam melhores resultados.

Analisei principalmente:

* quantidade de usuários;
* sessões;
* conversões;
* receita;
* LTV;
* CAC;
* ROI.

Além disso, observei como essas métricas mudavam ao longo do tempo.

---

# 7. Visualizações

Durante o projeto, utilizei gráficos para facilitar a interpretação dos resultados.

As visualizações me ajudaram principalmente a:

* observar a evolução dos usuários ao longo do tempo;
* comparar sessões e duração;
* analisar as conversões;
* acompanhar o LTV das coortes;
* comparar os gastos de marketing;
* visualizar o CAC por origem;
* comparar o ROI;
* identificar diferenças entre dispositivos;
* identificar quais origens de anúncios apresentavam melhores resultados.

Procurei sempre relacionar os gráficos com as métricas calculadas, para não analisar as visualizações de forma isolada.

---

# 8. Recomendações para o marketing

Depois de analisar os dados de produto, vendas e marketing, utilizei os resultados para avaliar onde os investimentos poderiam ser mais eficientes.

Para fazer as recomendações, não considerei somente a quantidade de usuários trazidos por cada origem.

Também levei em consideração principalmente:

* **LTV**, para entender quanto os clientes geravam de receita;
* **CAC**, para entender o custo de aquisição;
* **ROI**, para avaliar o retorno dos investimentos;
* conversão;
* comportamento dos clientes ao longo do tempo.

A partir dessas métricas, comparei as diferentes origens de anúncios e identifiquei aquelas que apresentavam uma relação mais interessante entre investimento e retorno.

Minha recomendação final foi baseada principalmente nas origens que conseguiram gerar clientes de maior valor sem exigir um custo de aquisição excessivo.

Os valores e comparações utilizados para chegar à recomendação final estão apresentados no notebook, junto com os gráficos e cálculos realizados.

---

# 9. Conclusão

Neste projeto, consegui analisar o caminho completo do usuário, desde o acesso ao site até a realização de uma compra.

Primeiramente, analisei como os usuários utilizavam o produto e com que frequência acessavam o site. Depois, observei o comportamento de compra e o tempo necessário para a conversão.

Em seguida, calculei métricas como **LTV, CAC e ROI** para entender não apenas quantos clientes eram adquiridos, mas também quanto eles representavam financeiramente para a empresa.

A análise de marketing foi importante para entender que o maior número de usuários nem sempre significa o melhor resultado. Para tomar uma decisão de investimento, é necessário comparar o custo para adquirir os clientes com a receita que eles geram.

Com isso, consegui utilizar os dados para identificar quais origens de anúncios apresentavam melhores resultados e formular recomendações para uma possível otimização dos investimentos de marketing.

---

# Tecnologias utilizadas

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook**

---

# Principais aprendizados

Neste projeto, aprendi a analisar um negócio olhando para diferentes etapas da jornada do cliente.

Coloquei em prática conceitos como:

* preparação e tratamento de dados;
* análise de datas;
* análise de usuários e sessões;
* conversão;
* análise de coortes;
* LTV;
* CAC;
* ROI;
* análise de investimentos em marketing;
* visualização de dados;
* interpretação de métricas;
* elaboração de recomendações baseadas em dados.

Também consegui entender melhor como diferentes métricas precisam ser analisadas em conjunto para chegar a uma conclusão mais confiável sobre o desempenho de uma estratégia de marketing.
