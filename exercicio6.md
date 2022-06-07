> ## Calculando e imprimindo IMC

```
Algoritmo "IMC"
// Lógica de Programação
// Professor   : Marcos Monteiro
// Disciplina   : [Lógica de Programação]
//Calcular o IMC e imprimir os dados e resultado.

Var
   peso, altura, imc:real
   nome:caractere

Inicio
   escreval("Digite seu nome: ")
   leia(nome)
   escreval("Digite seu peso: ")
   leia(peso)
   escreval("Digite sua altura: ")
   leia(altura)

   imc <- peso/(altura * altura)

   escreval("Nome: ", nome, " Altura: ", altura, "mts", " Peso: ", peso, "kg", " IMC: ", imc)
Fimalgoritmo
```