# Análise de dados com Pandas
<h2>Fala pessoal abaixo um pouco do meu estudo com a biblioteca Pandas</h2>
<h3>Imprimindo nosso DataFrame</h3>
<h4>primeiro começamos importando a biblioteca PANDAS para isso iremos utlizar a seguinte linha de código .</h4>
<h5><i>import pandas as pd</i></h5>
<h4>em seguinda atribuimos o nosso arquivo xlsx a uma variável dentro do nosso código</h4>
<h5><i>tabela_vendas = pd.read_excel('Vendas.xlsx')</i></h5>
<h4>Para visualizar o nosso Dataframe podemos utilizar os comandos print ou display</h4>
<h5><i>display(tabela_vendas)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151063456-c53751f4-59d7-43be-81d6-53e843f9686a.png" width="900px" /></div>
<h3>Localizando um objeto</h3>
<h4>Para filtrar nossa pesquisa utilizamos o .loc[<i>'Objeto Desejado'</i>] atribuindo o resultado a variável vendas_norteshopping e utilizando o comando display para imprimir nosso novo Dataframe na tala</h4>
<h5><i>vendas_norteshopping = tabela_vendas.loc[tabela_vendas['ID Loja'] == 'Norte Shopping']</i></h5>
<h4>E imprimimos utilizando o comando</h4>
<h5>display(vendas_norteshopping)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151064027-21245a3a-955c-4bb1-b247-748a89ffeefd.png" width="900px" /></div>
<h3>Reduzindo o número de colunas</h3>
<h4>Para diminuir o número de colunas do nosso Dataframe criamos uma nova variável e atribuimos a ela o seguindo código:</h4>
<h5><i>vendas_norteshipping_dois = tabela_vendas.loc[tabela_vendas['ID Loja'] == 'Norte Shopping', 
['ID Loja', 'Produto','Valor Unitário']]</i></h5>
<h4>E imprimimos utilizando o comando</h4>
<h5><i>display(vendas_norteshipping_dois)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151064118-35663c5d-6f9f-4d1a-b1fe-8b734b789b17.png" width="900px" /></div>
<h3>Filtrando Por Coluna</h3>
<h4>Para filtar por coluna é mais simples criamos uma nova variável atribuindo o seguinde comando:</h4>
<h5><i>produto_valor = tabela_vendas[['Produto', 'Valor Unitário']]</i></h5>
<h4>E imprimimos utilizando</h4>
<h5><i>display(produto_valor)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151064190-d1abc121-1bde-46f8-8140-c7b9f31a0413.png" width="900px" /></div>
