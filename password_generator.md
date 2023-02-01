# Gerador de senhas em Python

from random import choices
import random
import string

#pode editar caso não queira algum caractere
min= 'abcdefghijklmnopqrstuvwxyz'
max= 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
num= '0123456789'
simbolos='[],.-_=+@#$%¨&*!'

tamanho_da_senha= int(input("Quantos digitos sua senha vai ter? "))
qntInt = int(tamanho_da_senha)
length = qntInt

#senha com todos os caracteres disponíveis
all = min + max + num + simbolos
passwordAll = "".join(random.sample(all,length))

#senha somente com letras minúsculas e números
MinNum = min+num
passwordMinNum = "".join(random.sample(MinNum,length))

#senha com letras minúsculas, maiúsculas e números
MMn = min + max + num
passwordMMn = "".join(random.sample(MMn, length))

#senha somente com números
def passwordNUM(lenght):
    passwordNUM= "".join(random.choices(string.digits, k=lenght))
    return passwordNUM

print ("A sua nova senha com todos os caracteres disponíveis é: ", passwordAll)

print ("A sua nova senha com letras minúscula e números: ", passwordMinNum)

print ("A sua nova senha com letras minúsculas, maiúsculas e números é: ", passwordMMn)

print ("A sua nova senha somente com números é: ", passwordNUM(tamanho_da_senha))
