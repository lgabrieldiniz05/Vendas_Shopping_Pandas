# Análise de dados com Pandas
<h2>Fala pessoal abaixo um pouco do meu estudo com a biblioteca Pandas</h2>
<h3>Imprimindo nosso DataFrame</h3>
<h4>primeiro começamos importando a biblioteca PANDAS para isso iremos utlizar a seguinte linha de código .</h4>
<h5><i>import pandas as pd</i></h5>
<h4>em seguinda atribuimos o nosso arquivo xlsx a uma variável dentro do nosso código</h4>
<h5><i>tabela_vendas = pd.read_excel('Vendas.xlsx')</i></h5>
<h4>Para visualizar o nosso Dataframe podemos utilizar os comandos print ou display</h4>
<h5><i>display(tabela_vendas)</i></h5>
![image](https://user-images.githubusercontent.com/90981124/150871931-d48eb915-dcba-4fee-97e7-cecf321f9140.png)
<h3>Localizando um objeto</h3>
<h4>Para filtrar nossa pesquisa utilizamos o .loc[<i>'Objeto Desejado'</i>] atribuindo o resultado a variável vendas_norteshopping e utilizando o comando display para imprimir nosso novo Dataframe na tale</h4>
<h5><i>vendas_norteshopping = tabela_vendas.loc[tabela_vendas['ID Loja'] == 'Norte Shopping']</i></h5>
<h4>E imprimimos utilizando o comando</h4>
<h5>display(vendas_norteshopping)</i></h5>
![image](https://user-images.githubusercontent.com/90981124/150872008-402619cb-60a9-413d-8a2c-bf6210540b1d.png)
<h3>Reduzindo o número de colunas</h3>
<h4>Para diminuir o número de colunas do nosso Dataframe criamos uma nova variável e atribuimos a ela o seguindo código:</h4>
<h5><i>vendas_norteshipping_dois = tabela_vendas.loc[tabela_vendas['ID Loja'] == 'Norte Shopping', 
['ID Loja', 'Produto','Valor Unitário']]</i></h5>
<h4>E imprimimos utilizando o comando</h4>
<h5><i>display(vendas_norteshipping_dois)</i></h5>
![image](https://user-images.githubusercontent.com/90981124/150872050-a5854f84-7e41-491f-a7c8-4daf482f9f90.png)
<h3>Filtrando Por Colunda</h3>
<h4>Para filtar por coluna é mais simples criamos uma nova variável atribuindo o seguinde comando:</h4>
<h5><i>produto_valor = tabela_vendas[['Produto', 'Valor Unitário']]</i></h5>
<h4>E imprimimos utilizando</h4>
<h5><i>display(produto_valor)</i></h5>
![image](https://user-images.githubusercontent.com/90981124/150872116-716ee88f-616e-4a66-94f0-b78bdee11958.png)
