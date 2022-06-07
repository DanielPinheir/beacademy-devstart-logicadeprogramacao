> ## Operações bancárias com quantidades de operações.

```
Algoritmo "QuantidadeOperacoesBancarias"
// Lógica de Programação
// Professor   : Marcos Monteiro

// Criarei um programa que simula uma operação bancária
//(saque, depósito ou tranferencia), quantidade de 
//operações a realizar e retorna o  saldo inicial, 
//a operação e o saldo final ao usuário.

Var
   valorInicial:real
   operacao, banco, agencia, conta:caractere
   tipoOperacao, numeroOperacoes, i:inteiro
   saldoAtual, valorDeposito, valorTransferencia, valorSaque:real

Inicio

   escreval ("Quantidade de operações a serem realizadas: ")
   leia(numeroOperacoes)
   valorInicial <- 500.00
   
   para i de 1 ate numeroOperacoes faca
      escreval("Digite 1 para operação de Saque ou 2 para operação de Depósito ou 3 para operação de Transferência: ")
      leia(tipoOperacao)

      enquanto (tipoOperacao <> 1) e (tipoOperacao <> 2) e (tipoOperacao <> 3) faca
         escreval("Operação inválida!!Digite 1 para Saque ou 2 para Depósito ou 3 pata Transferência: ")
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
            valorInicial <- saldoAtual
            escreval("Valor inicial: R$", valorInicial)
            escreval("Operação: ", operacao)
            escreval("Valor da operação: ", valorSaque)
            escreval("Saldo: R$", saldoAtual)
            valorInicial <- saldoAtual

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
             valorInicial <- saldoAtual
             
             senao
                se (tipoOperacao = 3) entao
                   operacao <- "Transferência (-)"
                   escreval("Digite o número do Banco: ")
                   leia(banco)
                   escreval("Digite a Agência: ")
                   leia(agencia)
                   escreval("Digite a Conta: ")
                   leia(conta)
                   escreval("Digite o valor da transferência: ")
                   leia(valorTransferencia)
                   
                   enquanto (valorTransferencia  > valorInicial) faca
                            escreval("Saldo insuficiente para saque! Digite um valor até R$", valorInicial, ".")
                            leia(valorTransferencia)
                   fimenquanto
                   
                   saldoAtual <- valorInicial - valorTransferencia
                   escreval("Número do banco: ",banco)
                   escreval("Agência: ",agencia)
                   escreval("Conta: ",conta)
                   escreval("Valor inicial: R$", valorInicial)
                   escreval("Operação: ", operacao)
                   escreval("Valor da operação: ", valorTransferencia)
                   escreval("Saldo: R$", saldoAtual)
                   valorInicial <- saldoAtual
                fimse
          fimse
      fimse
   fimpara
 fimalgoritmo