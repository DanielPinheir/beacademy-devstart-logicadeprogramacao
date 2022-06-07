> ## Area e perimetro Quadrado e Triangulo

```
Algoritmo "areaEperimetro"
// Lógica de Programação
// Professor   : Marcos Monteiro 
// Descrição   : Programa que calcula área e o perímetro
// do q-quadrado ou t-triangulo
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 24/05/2022
Var
lado, altura, area, perimetro: real
figura: inteiro

Inicio
      escreval("Escolha a figura ('1' para Quadrado ou '2' para Triângulo):")
      leia(figura)
      enquanto (figura <> 1) e (figura <> 2) faca
      escreval("Figura inválida!!Digite '1' para Quadrado ou '2' para Triângulo:")
      leia(figura)
      fimenquanto
      escolha figura
           caso 1
                area := -1
                perimetro := -1
           caso 2
                area := 1
                perimetro := 1
           outrocaso
                area := 0
                perimetro := 0
      fimescolha
      se (area = 0) e (perimetro = 0) entao
           escreval("Operação inválida!! Escolha 'q' ou 't'!!")
      senao
           se  (area = -1) e (perimetro = -1) entao
             escreval("Digite o lado do quadrado: ")
             leia(lado)
             area <- lado * lado
             perimetro <- lado * 4
             escreval("Area do quadrado: ", area, "cm2")
             escreval("Perimetro do quadrado: ", perimetro, "cm")
             
             senao
                  se (area = 1) e (perimetro = 1) entao
                     escreval("Digite a altura do triângulo: ")
                     leia(altura)
                     escreval("Digite o lado do triângulo: ")
                     leia(lado)
                     area <- (lado * altura)/2
                     perimetro <- lado * 3
                     escreval("Area do triângulo: ", area, "cm2")
                     escreval("Perimetro do triângulo: ", perimetro, "cm")
                  fimse
             fimse
      fimse
Fimalgoritmo

```
