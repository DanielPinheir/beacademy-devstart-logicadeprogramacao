> ## Classificação do IMC

```
Algoritmo "ClassificacaoIMC"
// Lógica de Programação 
// Professor   : Marcos Monteiro 
// Disciplina   : [Lógica de Programação]
//Calcular o IMC e classificar de acordo com o resultado.

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

   se (imc < 19) entao
      escreval("Classificação: Abaixo do Peso.")
      senao
           se (imc >= 19) e (imc < 25) entao
           escreval("Classificação IMC de " + nome + ": Peso Normal.")
           senao
                se (imc >= 25) e (imc < 30) entao
                escreval("Classificação IMC de " + nome + ": Sobrepeso.")
                senao
                     se (imc >= 30) e (imc < 40) entao
                     escreval("Classificação IMC de " + nome + ": Obesidade Tipo I.")
                     senao
                          escreval("Classificação IMC de " + nome + ": Obesidade mórbida.")
                     fimse
                fimse
          fimse
   fimse
Fimalgoritmo
```