# Lendo dados usando python e pandas
import pandas as pd
<br>
tabela = pd.read_csv("") <<< nome da tabela ou caminho
<br>
display(tabela) <<< se estiver usando jupyter

# Separando colunas e somando
nome da variavel de sua escolha >>>>> maisjogados = tabela["aqui nome da tabela"].sum()
<br>
print(maisjogados)

# Agrupando e somando
maisjogados = tabela[["aqui nome das tabelas"]].groupby("Name").sum()
<br>
display(maisjogados) <<< se estiver usando jupyter

# Análise final 
maisjogados = tabela[["Rank", "Name", "Platform", "Year", "Genre", "Publisher",	"NA_Sales",	"EU_Sales",	"JP_Sales", "Global_Sales"]].groupby(["Rank", "Name", "Platform", "Year", "Genre", "Publisher",	"NA_Sales",	"EU_Sales",	"JP_Sales", "Global_Sales"]).sum()
<br>
display(maisjogados) <<< se estiver usando jupyter


