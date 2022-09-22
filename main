import os #bliblioteca de comandos no sistema operacional#
import random #bliblioteca de sorteio de palavras#

# bem vindo #

nome = input("Digite seu nome: ") #input para digitar nome#
print (f'Ola seja bem vindo {nome}! Vamos começar a jogar?') #imprime a frase com o nome#
input('\nPressione enter para começar') #comando para iniciar#

# jogo #

lista_de_palavras = ['gato','cachorro','tigre','elefante'] #lista de opc#
palavra_selecionada = random.choice (lista_de_palavras).upper() #sorteando palavra da lista#
tamanho_palavra = len(palavra_selecionada) #tamanho da palavra#
palavra_codificada = ['_']*tamanho_palavra #substituindo letra por _#
quantidade_de_erros = 0 #variavel de erros#

while '_' in palavra_codificada and quantidade_de_erros < 6: #limitando erro#
    print (f'\nSua palavra tem {tamanho_palavra} letras, o tema é animais') 
    print (f'Erros: {quantidade_de_erros} de 6')
    
    for letra in palavra_codificada:
        print(letra , end = ' ')
    print()

    letra_escolhida = input("Digite uma letra: ").upper() #letra que escolhe#
    acertou = False 
    for i in range(len(palavra_selecionada)): #ler cada letra na palavra#
        if letra_escolhida == palavra_selecionada[i]: #verificar se a letra digitada tem na palavra"
            palavra_codificada [i] = letra_escolhida #substituir letra#
            acertou = True
    if acertou == True:
        print("\nParabens! Acertou.")
    else:
        print("\nErrou! Essa letra não existe nessa palavra.")
        quantidade_de_erros = quantidade_de_erros + 1

if quantidade_de_erros == 6:
    print("Você perdeu!")
else:
    print("Parabéns! Você ganhou.")

print("A palavra selecionada era: ")
print(palavra_selecionada)
