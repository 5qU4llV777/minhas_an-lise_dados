# Lendo dados usando python e pandas
import pandas as pd
<br>
tabela = pd.read_csv("") <<< nome da tabela ou caminho
<br>
display(tabela) <<< se estiver usando jupyter

# Separando colunas e somando
name_count_price = tabela["User Rating Count"].sum()
<br>
print(name_count_price)

# Agrupando e somando
name_count_price = tabela[["Name", "User Rating Count", "Price"]].groupby("Name").sum()
<br>
display(name_count_price) <<< se estiver usando jupyter

# Análise final 
name_count_price = tabela[["Name", "User Rating Count", "Price", "Genres"]].groupby(["Name", "User Rating Count", "Price", "Genres"]).sum()
<br>
display(name_count_price) <<< se estiver usando jupyter


