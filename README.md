# Power-Bi-Projeto-2

1. Gerando colunas novas (DAX)

`Custo Basico = F_acoes[Ações]*F_acoes[PreçoCompra]`

![image](https://github.com/user-attachments/assets/ffa4fa11-e5a3-485a-802f-af8a20d1a5b8)

`Valor Mercado = F_acoes[Ações]*F_acoes[PreçoCorrente]`

![image](https://github.com/user-attachments/assets/50737d08-ccae-4639-8484-f0c676289010)

`Ganho/Perda = F_acoes[Valor Mercado]-F_acoes[Custo Basico]`

![image](https://github.com/user-attachments/assets/58b22127-6421-42ea-8d89-82e3817b9687)

`Dividendos = F_acoes[PreçoCorrente]-F_acoes[PreçoCompra]`

![image](https://github.com/user-attachments/assets/197e03f5-0b5b-4f0a-a552-daad2c9924b0)

`Pct Lucro = DIVIDE(F_acoes[Valor Mercado];F_acoes[Custo Basico]-1)`

![image](https://github.com/user-attachments/assets/1f792c51-f817-4d16-ba38-97328a26beb3)

2. Medidas

* Criei duas medidas

`Valor total Corrente = SUM(F_acoes[Valor Mercado])`
`Valor Total Investido = SUM(F_acoes[Custo Basico])`

![image](https://github.com/user-attachments/assets/0b8b13bd-849c-475e-9533-dad2c6a9834b)

* Mais uma medida chamada Ganho/Perdas, aproveitando as duas medidas anteriores

`Ganho/Perdas = [Valor Total Corrente]-[Valor Total Investido]`

![image](https://github.com/user-attachments/assets/fc17529c-20b2-41ff-88d8-e626a21ec4b4)

* Outra Medida chamada retorno

`Retorno = DIVIDE([Valor Total Corrente];[Valor Total Investido]-1)`

![image](https://github.com/user-attachments/assets/97ddcb12-e11f-4265-8c51-45d6cb0bc89a)



