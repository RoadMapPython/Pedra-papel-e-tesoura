# Primeira Live do Projeto RoadMap Python

Criação de um jogo(Pedra, Papel e Tesoura) em python

<h2>Faala Dev!!!</h2>



Seja bem vindo ao nosso primeiro passo nessa viagem buscando mais conhecimentos de Python. Um prazer imenso ter você aqui com a gente nesse primeiro passo rumo a uma jornada incrível.

Nesse primeiro momento realizaremos a criação de um jogo de Pedra, Papel e Tesoura ou o mundialmente conhecido <b>Jokenpô</b>.

Além desse texto, temos também um pequeno trecho da nossa live realizada ao vivo na Twitch! Disponibilizamos ele no canal do YouTube!


<h3>Passo a passo do nosso jogo "Pedra, Papel e Tesoura"</h3>


#Em um primeiro momento necessitamos realizar a importação das bibliotecas
from random import randint #Biblioteca responsável por fornecer números aleatórios com o randint
from time import sleep     #Biblioteca responsável por fornecer pausas estratégicas no jogo com o sleep


 //Iniciamos um Laço para realizar uma partida melhor de 3 
 
 
for i in range(3):
    possibilidades=("Pedra","Papel","Tesoura")
 
 
   //Realiza de maneira aleatória a escolha da máquina representadas por 0 e 1
    maquina = randint(0,2)

    print("<>"*15)
    print("0 - Pedra \n "+"1 - Papel \n " + "2 - Tesoura ")
    Jogador=int(input("Qual voce deseja?"))
    print("<>"*15)
    print("JO")
    sleep(3)      //Realiza um "freeze" de 3 segundos antes de continuar a execução do código
                  //Utilizaremos o sleep, a cada momento que quisermos espaçar um período de tempo 
                  //entre uma mensagem e outra, criando um clima de tensão até a resposta do confronto
    print("KEN")
    sleep(3)      
    print("PO")
    sleep(3)
    print("Computador Jogou {}".format(possibilidades[maquina]))
    print(" Voce      Jogou {}".format(possibilidades[Jogador]))
    
    
    Agora que o computador foi capaz de realizar uma escolha e o usuário também fez sua escolha de opção de jogada, precisamos mostrar o resultado!

Mas como comparar a jogada do computador e do usuário? Para isso, utilizaremos um recurso presente em linguagens de programação ou não, as estruturas condicionais: se e senão. Como usamos essas estruturas em nossa fala? Usamos para delimitar cenários de verdadeiros e falsos. Exemplo:

Se eu ganhar na Mega Sena, viajarei o mundo!! Senão, fico em casa mesmo...
Nesse caso, a condição está girando em torno de "GANHAR NA MEGA SENA". Sendo este cenário verdadeiro, uma ação será realizada. Sendo falso, outra ação será realizada.

Em Python, conseguimos expressar a mesma ideia com as estruturas abaixo:

. if (no português, SE)
. elif (no português, SE SENÃO)
. else (no português, SENÃO)

//Caso a máquina escolha a opção Pedra, entraremos em uma cadeia de opções.
//Logo, precisamos nos adptar a cada cenário possível.

 if maquina==0:
    #pedra
        if Jogador ==0:
          print ("Empate")

        elif Jogador==1:
          print ("Jogador Venceu") 

        elif Jogador==2:
          print("Computador Venceu")


    elif maquina==1:
      #Papel
          if Jogador==0:
            print("Computador Venceu") 
          elif Jogador==1:
            print("Empate")
          elif Jogador==2:
            print("Jogador Venceu")

    elif maquina==2:
      #Tesoura
          if Jogador==0:
            print("Jogador Venceu")
          elif Jogador==1:
            print("Computador Venceu")
          elif Jogador==2:
            print("Empate")

    else:
       print("Movimento Inválido") 


#Jogo Completo# 


from random import randint
from time import sleep 

for i in range(3):
    possibilidades=("Pedra","Papel","Tesoura")
    maquina = randint(0,2)

    print("<>"*15)
    print("0 - Pedra \n "+"1 - Papel \n " + "2 - Tesoura ")
    Jogador=int(input("Qual voce deseja?"))
    print("<>"*15)
    print("JO")
    sleep(3)
    print("KEN")
    sleep(3)
    print("PO")
    sleep(3)
    print("Computador Jogou {}".format(possibilidades[maquina]))
    print(" Voce      Jogou {}".format(possibilidades[Jogador]))

    if maquina==0:
    #pedra
        if Jogador ==0:
          print ("Empate")

        elif Jogador==1:
          print ("Jogador Venceu") 

        elif Jogador==2:
          print("Computador Venceu")


    elif maquina==1:
      #Papel
          if Jogador==0:
            print("Computador Venceu") 
          elif Jogador==1:
            print("Empate")
          elif Jogador==2:
            print("Jogador Venceu")

    elif maquina==2:
      #Tesoura
          if Jogador==0:
            print("Jogador Venceu")
          elif Jogador==1:
            print("Computador Venceu")
          elif Jogador==2:
            print("Empate")

    else:
       print("Movimento Inválido") 


print("\n")
print("\n")
print("\n")


Chegamos ao final do nosso primeiro passo rumo a uma jornada incrível com Python.

Que tal continuarmos melhorando esse código à medida que aprendemos mais sobre Python? Pensamos em adicionar interface gráfica a esse jogo em próximos encontros! O que acham? Mais ideias? Sugiram pra gente em nossas próximas lives!

Esperamos vocês lá.

Bons estudos!!!!!!!!

Autor: Emanoel Faria (GitHub : @Whoefa)


Referências : 

Curso em Video : https://www.youtube.com/watch?v=S9uPNppGsGo&list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6


