# Reposity-Luis-Henrique
Algoritmo "Eleitorado"

Var

obrigatorio, facultativo, nao_obrigatorio : inteiro
eleitor, i : inteiro
continuar_contagem : caracter

Inicio

      escreval("Informe a idade do eleitor")
      leia(eleitor)

//inicializacao das variaveis que usei para contar os tipos de eleitores.
obrigatorio <- 0
facultativo <- 0
nao_obrigatorio <- 0
i <- 0

enquanto (continuar_contagem <> "nao") faca


     se (eleitor >= 18) e (eleitor <=69) entao

     obrigatorio <- obrigatorio + 1

                 senao
                 se (eleitor >= 16) ou (eleitor = 17) ou (eleitor >= 70) entao

                 facultativo <- facultativo + 1

     senao (eleitor < 16 ) entao

     nao_obrigatorio <- nao_obrigatorio + 1

                      fimse
                 fimse


                escreval("Informe a idade do eleitor")
                leia(eleitor)
                
i <- i+1

     //A cada 10 eleitores o algoritmo perguntara se deseja continuar a contagem
    se (i = 10) entao

       escreval("Deseja continuar a contagem de eleitor")
       leia(continuar_contagem)
       
                               fimse

             //Usei esta estrutura SE, para reninciar a variavel "I", na qual contava a quantidade de eleitores.
             se ( i = 10) entao
             i<- 0
             fimse

                  fimenquanto

           // Quando for finalizado a contagem, sera mostrado uma tabela com a contagem de eleitores
           escreval("Eleitor obrigado a votar ", obrigatorio)
           escreval("Eleitor facultativo ", facultativo)
           escreval("Eleitor nao obrigatorio ", nao_obrigatorio)

Fimalgoritmo
