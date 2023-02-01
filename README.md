# INSS-calculator

SB= float(input('Digite seu salário bruto: '))

if SB <= 1302.00:
    print('Alíquota de 7,5%')
    print('Será recolhido: ', SB * 0.075)
    print('Irá sobrar: ', SB-(SB * 0.75))

elif SB <= 2571.29:
    print('Alíquota de 9%')
    print('Será recolhido: ', SB * 0.09)
    print('Irá sobrar: ', SB-(SB * 0.09))

elif SB <= 3856.94:
    print('Alíquota de 11%')
    print('Será recolhido: ', SB * 0.12)
    print('Irá sobrar: ', SB-(SB * 0.12))

elif SB <= 7507.49:
    print('Alíquota de 14%')
    print('Será recolhido: ', SB * 0.14)
    print('Irá sobrar: ', SB-(SB * 0.14))

else:
    print('Valor inválido')
    
