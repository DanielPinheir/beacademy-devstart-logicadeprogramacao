> ## Calculadora Completa

```
Algoritmo "CalculadoraCompleta"
// Lógica de Programação 
// Professor   : Marcos Monteiro 
// Recebe 2 números e uma operação retornando o resultado
// e fazendo novo cálculo caso usuário deseje
Var
   numero1, numero2:real
   operacao, novoCalculo:caractere
   resultado:real

Inicio
      escreval("Digite o primeiro número: ")
      leia(numero1)
      escreval("Digite a operação: ")
      leia(operacao)
      escreval("Digite o segundo número: ")
      leia(numero2)
      escolha operacao
              caso "+"
                   resultado := numero1 + numero2
              caso "-"
                   resultado := numero1 - numero2
              caso "*"
                   resultado := numero1 * numero2
              caso "/"
                   resultado := numero1 / numero2
              outrocaso
                   resultado := -1
      fimescolha
      se (resultado = -1) entao
           escreval("Operação inválida!! Escolha + , - , * , /")
      senao
           escreval("Resultado :", resultado)
      fimse
      
      escreval(numero1, " ", operacao, " ", numero2, " = ",resultado)

      escreval("Deseja realizar um novo cálculo (S ou N)? ")
      leia(novoCalculo)

      enquanto (novoCalculo = "s") ou (novoCalculo = "S") faca
         escreval("Digite o primeiro número: ")
         leia(numero1)
         escreval("Digite a operação: ")
         leia(operacao)
         escreval("Digite o segundo número: ")
         leia(numero2)
         escolha operacao
                 caso "+"
                      resultado := numero1 + numero2
                 caso "-"
                      resultado := numero1 - numero2
                 caso "*"
                      resultado := numero1 * numero2
                 caso "/"
                      resultado := numero1 / numero2
                 outrocaso
                      resultado := -1
         fimescolha
         se (resultado = -1) entao
              escreval("Operação inválida!! Escolha + , - , * , /")
         senao
              escreval("Resultado :", resultado)
         fimse
         escreval(numero1, " ", operacao, " ", numero2, " = ",resultado)
         escreval("Deseja realizar um novo cálculo (S ou N)? ")
         leia(novoCalculo)
      fimenquanto
      escreval("Muito obrigado!!")
Fimalgoritmo
```