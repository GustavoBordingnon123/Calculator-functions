import math
import matplotlib.pyplot as plt
import numpy as np
from matplotlib.pyplot import *
from numpy import *
import pandas
import plotly.express as px
from sympy import *
from sympy.plotting import *

raiz_quadrada = 0
raiz_quadrada_final = 0
contador_debbugger = 0
escolha_função_2grau = 0
funcao_exponencial = 0
escolha_exponencial = 0
escolha_do_usuario = 0
flag = 0


def opção_do_usuario():
    print()
    print("calculadora rmc - gustavo bordignon e kadu")
    print("1- funções do segundo grau")
    print("2- funções exponensiais")
    print("3- matrizes")
    print("4- sair")
    opção_no_menu = int(input("olá escolha qual opção da calculadora voçê quer ultilizar: "))
    if opção_no_menu < 1 or opção_no_menu > 4:
        opção_no_menu = int(input("este numero é invalido, por favor escolha um dos numeros apontados na legenda"))
        return opção_no_menu
    return opção_no_menu
          
def opção_do_usuario_função_2grau():
    print()
    print("por favor, escolha qual tipo de conta da função de segundo grau voçê quer:")
    print()
    print("1-Calcular raizes")
    print("2- f(x) = y")
    print("3- Calcular vértice")
    print("4- gera grafico")
    print("5- voltar")
    escolha_função_2grau = int(input("olá escolha qual opção da calculadora voçê quer ultilizar: "))
    if escolha_função_2grau < 1 or escolha_função_2grau > 5:
        escolha_função_2grau = int(input("este numero é invalido, por favor escolha um dos numeros apontados na legenda"))
        return escolha_função_2grau
    return escolha_função_2grau

def escolha_usuario_exponencial():
    print()
    print("digite: ")
    print("1- Para verificar se é crescente ou decrescente")
    print("2- Para calcular função em x pedido")
    print("3- Para gerar gráfico")
    print("4- Para voltar")
    print()
    escolha_exponecial = int(input("Escolha qual opção voce deseja: "))
    if escolha_exponecial < 1 or escolha_exponecial > 4:
        escolha_exponecial = int(input("Essa opção não existe, escolha uma valida!: "))
        return escolha_exponecial
    return escolha_exponecial

def graficoExponencial(a, x):
    return (a**x)

def funcaoExponencial(a, x):
    return (a**x)

def Xvertice_Yvertice():
    valor_delta = (valor_b * valor_b) - 4 * valor_a * valor_c
    valor_delta = pow(valor_delta, 1 / 2)
    vertice_x = (-valor_b) / (valor_a * 2)
    vertice_y = (-valor_delta) / (valor_a * 4)
    if valor_a < 0:
        print("o vertice de x é maximo igual a: ", vertice_x)
    else:
        print("o vertice de x é minimo igual a: ", vertice_x)
    print("o vertice de y é igual a: ", vertice_y)

def matrizes_menu():
    print()
    print("digite: ")
    print("1- Para verificar se a matriz é quadrada ou não")
    print("2- Para multiplicação de matrizes")
    print("3- Para gerar matriz transposta")
    print("4- Para voltar")
    print()
    matrizes = int(input("Escolha qual opção voce deseja: "))
    if matrizes < 1 or matrizes > 4:
        matrizes = int(input("Essa opção não existe, escolha uma valida!: "))
        return matrizes
    return matrizes


def criação_da_matrizes(linhas,colunas):
    numero_de_linhas = linhas
    numero_de_colunas = colunas
    matriz = [0] * numero_de_linhas
     # esse bloco de comando forma a matriz necessária para gerar a matriz
    for linha in range(numero_de_linhas):
        for coluna in range(numero_de_colunas):
            matriz[linha] = [0] * numero_de_colunas
    #esse bloco muda os valores da sua matriz
    print()
    print("agora irei pedir os numero da sua matriz, eu começo colocando primeiro todos os numero de uma linha para depois ir para outra")
    print("os numeros de uma linha são colocados da esquerda pra direita")
    print()
    for linha in range(numero_de_linhas):
        for coluna in range(numero_de_colunas):
            matriz[linha][coluna] = int(input("digite o numero para ser colocado na sua matriz: "))           
    #esse bloco printa a matriz
    print()
    for cont in range(numero_de_linhas):
            print(matriz[cont])

    return matriz


a = 2
#vetorX = np

print()

while escolha_do_usuario != 4:

    escolha_do_usuario = opção_do_usuario()


    if escolha_do_usuario == 1:
        escolha_função_2grau = 0
        while escolha_função_2grau != 5:

            escolha_função_2grau = opção_do_usuario_função_2grau()
            print(escolha_função_2grau)

            if escolha_função_2grau == 1:
                valor_a = int(input("digite o valor de a: "))
                while valor_a == 0:
                    valor_a = int(input("o valor de a não pode ser 0, digite outro: "))
                valor_b = int(input("digite o valor de b: "))
                valor_c = int(input("digite o valor de c: "))
                valor_delta =  (valor_b * valor_b) -  4 * valor_a * valor_c
                valor_delta = pow(valor_delta,1/2)
                raiz_1 = (-valor_b + valor_delta)/2 * valor_a
                raiz_2 = (-valor_b - valor_delta)/2 * valor_a
                print("o valor das raizes são",raiz_1,"e",raiz_2)

            elif escolha_função_2grau == 2:
                valor_x = int(input("digite o valor de x: "))
                valor_a = int(input("digite o valor de a: "))
                while valor_a == 0:
                    valor_a = int(input("o valor de a não pode ser 0, digite outro: "))
                valor_b = int(input("digite o valor de b: "))
                valor_c = int(input("digite o valor de c: "))
                valor_x_final = (valor_a*(valor_x*valor_x)) + (valor_b * valor_x ) + valor_c
                print("o valor de f(",(valor_x),")","=", valor_x_final) 

            elif escolha_função_2grau == 3:
                valor_a = int(input("digite o valor de a: "))
                while valor_a == 0:
                    valor_a = int(input("o valor de a não pode ser 0, digite outro: "))
                valor_b = int(input("digite o valor de b: "))
                valor_c = int(input("digite o valor de c: "))
                Xvertice_Yvertice()

            elif escolha_função_2grau == 4:
                valor_a = float(input("Digita o valor de A seu lindo: "))
                valor_b = float(input("Digita o valor de B: "))
                valor_c = float(input("Digita o valor de C: "))

                y = Function('y')
                x = Symbol('x')

                y = x ** 2 - valor_b * x + valor_c

                print(solve(y, x))

                y1 = diff(y, x)
                x_v = solve(y1, x)
                y_v = y.subs(x, valor_b / 2)
                print("O ponto do vertice é: ", (x_v[0], y_v))

                plot(y, xlim=[0, 10], ylim=[-5, 5])

            #escolha_do_usuario = opção_do_usuario_função_2grau()

            if escolha_do_usuario == 5:
                escolha_do_usuario = opção_do_usuario()


    elif escolha_do_usuario == 2:
        funcao_exponencial = 0
        while funcao_exponencial != 4:


            funcao_exponencial = escolha_usuario_exponencial()

            print(funcao_exponencial)

            if funcao_exponencial == 1:
                valor_a = float(input("Digite o valor de a: "))
                valor_b = float(input("Digite o valor de b: "))
                if valor_a > 1:
                    print("É crescente!")
                elif valor_a > 0 and valor_a < 1:
                    print("É decrescente!")
                else:
                    print("Não existe!")

            elif funcao_exponencial == 2:
                valor_x = float(input("digite o valor de x: "))
                valor_a = int(input("digite o valor de a: "))
                valor_b = int(input("digite o valor de b: "))
                while valor_b < 0: 
                    valor_b = int(input("o b não pode ser negativo, digite outro valor de b: "))
                valor_b = valor_b ** valor_x
                valor_x_final = valor_a * valor_b
                print(valor_x_final)


            elif funcao_exponencial == 3:
                vetorX = np.arange(-7, 7, 0.1)

                a = float(input("Digite o valor de A campeão: "))
                x = float(input("Digite o valor de B ai: "))

                vetorY = []
                for x in vetorX:
                    vetorY.append(funcaoExponencial(a, x))

                fig = plt.figure(figsize=(5, 5))

                plt.plot(vetorX, vetorY, label='Função Exponecial', color='g')

                plt.title('f(x) = a^x')
                plt.xlabel('eixo x')
                plt.ylabel('eixo y')
                plt.legend()
                plt.grid(True, which='both')
                plt.axhline(y=0, color='k')
                plt.axvline(x=0, color='k')
                plt.show()
                fig.savefig('FExp.png')

                print(funcaoExponencial(a, x))

            #funcao_exponencial = escolha_usuario_exponencial()

            if escolha_do_usuario == 5:
                escolha_do_usuario = opção_do_usuario()

    elif escolha_do_usuario == 3:
        função_matriz = 0 


        while função_matriz != 4:
            função_matriz = matrizes_menu()


            if função_matriz == 1:
                linhas = int(input("digite quantas linhas sua matriz tem: "))
                colunas = int(input("digite quantas colunas sua matriz tem: "))
                #criação_da_matrizes(linhas,colunas)
                if linhas == colunas:
                    print()
                    print("a matriz é quadrada")
                else:
                    print()
                    print("a matriz não é quadrada")

            if função_matriz == 2:
                linhas = int(input("digite quantas linhas sua matriz tem: "))
                colunas = int(input("digite quantas colunas sua matriz tem: "))
                primeira_matriz = criação_da_matrizes(linhas,colunas)

                print()
                print("agora digite os valores da 2 matriz para ser multiplicada com a primeira")
                linhas_matriz2 = int(input("digite quantas linhas sua matriz tem: "))
                colunas_matriz2 = int(input("digite quantas colunas sua matriz tem: "))
                segunda_matriz = criação_da_matrizes(linhas_matriz2,colunas_matriz2)
                print()
                
                matriz_multiplicada = [0] * linhas
                if colunas != linhas_matriz2:
                    print("a multiplicação dessa matriz é imposivel")
                else: 

                    for linha in range(linhas):
                        for coluna in range(colunas_matriz2):
                            matriz_multiplicada[linha] = [0] * colunas_matriz2

                    for mudando in range(colunas_matriz2):
                        for mudei in range(linhas):
                            for muda in range(colunas):
                                    matriz_multiplicada[mudando][mudei] += primeira_matriz[mudando][muda] * segunda_matriz[muda][mudei]

                    '''for mudei in range(linhas):
                        for muda in range(colunas):
                            matriz_multiplicada[1][mudei] += primeira_matriz[1][muda] * segunda_matriz[muda][mudei]'''                    
                    '''for muda in range(colunas):
                        matriz_multiplicada[1][0] += primeira_matriz[1][muda] * segunda_matriz[muda][0]
                    for muda in range(colunas):
                        matriz_multiplicada[1][1] += primeira_matriz[1][muda] * segunda_matriz[muda][1]'''

                    print("final")
                    for cont in range(linhas):
                        print(matriz_multiplicada[cont])
                    
            if função_matriz == 3: 
                linhas = int(input("digite quantas linhas sua matriz tem: "))
                colunas = int(input("digite quantas colunas sua matriz tem: "))
                matriz = [0] * linhas
                linhas_transposta = colunas
                colunas_transposta = linhas
                matriz_transposta = [0] * linhas_transposta

                #forma a primeira matriz
                for linha in range(linhas):
                    for coluna in range(colunas):
                        matriz[linha] = [0] * colunas

                #forma a matriz transposta
                for linha in range(linhas_transposta):
                    for coluna in range(colunas_transposta):
                        matriz_transposta[linha] = [0] * colunas_transposta
             
                #esse bloco muda os valores das matrizes
                print()
                print("agora irei pedir os numero da sua matriz, eu começo colocando primeiro todos os numero de uma linha para depois ir para outra")
                print("os numeros de uma linha são colocados da esquerda pra direita")
                print()
                for linha in range(linhas):
                    for coluna in range(colunas):
                        matriz[linha][coluna] = int(input("digite o numero para ser colocado na sua matriz: "))  
                        matriz_transposta[coluna][linha] = matriz[linha][coluna]


                #esse bloco printa a matriz
                print()
                print("sua primeira matriz:")
                for cont in range(linhas):
                    print(matriz[cont])



                #esse bloco printa a matriz transposta
                print()
                print("sua matriz transposta:")
                for cont in range(linhas_transposta):
                    print(matriz_transposta[cont])


                






                    
    elif escolha_do_usuario == 5:
        escolha_do_usuario = opção_do_usuario()


print("Fim do uso da calculadora")
