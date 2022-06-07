> ## Extrato bancário

```
Algoritmo "SaldoAtual"
// Lógica de Programação 
// Professor   : Marcos Monteiro 
// Disciplina   : [Lógica de Programação]
// Criarei um programa que simula uma operação bancária (saque ou depósito)
// e retorna o saldo inicial, a operação e o saldo final ao usuário.

Var
   valorInicial:real
   operacao:caractere
   tipoOperacao:inteiro
   saldoAtual, valorDeposito, valorSaque:real

Inicio
   valorInicial <- 500.00
   escreval("Digite 1 para operação de Saque ou 2 para operação de Depósito: ")
   leia(tipoOperacao)

   enquanto (tipoOperacao <> 1) e (tipoOperacao <> 2) faca
      escreval("Operação inválida!!Digite 1 para Saque ou 2 para Depósito: ")
      leia(tipoOperacao)
   fimenquanto
   se (tipoOperacao = 1) entao
      operacao <- "Saque (-)"
      escreval("Digite valor do saque: ")
      leia(valorSaque)
      enquanto (valorSaque  > valorInicial) faca
         escreval("Saldo insuficiente para saque! Digite um valor até R$", valorInicial, ".")
         leia(valorSaque)
      fimenquanto
         saldoAtual <- valorInicial - valorSaque
         escreval("Valor inicial: R$", valorInicial)
         escreval("Operação: ", operacao)
         escreval("Valor da operação: ", valorSaque)
         escreval("Saldo: R$", saldoAtual)


    senao
       se (tipoOperacao = 2) entao
          operacao <- "Depósito (+)"
          escreval("Digite o valor do depósito: ")
          leia(valorDeposito)
          saldoAtual <- valorInicial + valorDeposito
          escreval("Valor inicial: R$", valorInicial)
          escreval("Operação: ", operacao)
          escreval("Valor da operação: ", valorDeposito)
          escreval("Saldo: R$", saldoAtual)
       fimse
   fimse
Fimalgoritmo

```
