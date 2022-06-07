> ## Classificação da idade (true e false)

```
Algoritmo "classificaIdade"
// Lógica de Programação
// Professor   : Marcos Monteiro 
// Descrição   : Classifica idade como
//verdadeiro e falso de acordo com as condições
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 24/05/2022
Var
nome: caractere
idade: inteiro

Inicio

   escreval("Digite seu nome: ")
   leia(nome)
   escreval("Digite sua idade: ")
   leia(idade)
   
   escreval("Nome: ", nome)
   escreval("Idade: ", idade)
   escreval("Idade maior que 18: ", idade > 18)
   escreval("Idade diferente que 25: ", idade = 25)
   escreval("Idade diferente que 25 e nome igual a Marcos: ", (idade = 25) e (nome <> "Marcos"))
   escreval("Idade diferente que 25 ou nome é igual a Marcos: ", (idade <> 25) ou (nome = "Marcos"))
   escreval("Idade dividida por 2 é igual a zero: ", idade % 2 = 0)
Fimalgoritmo

```