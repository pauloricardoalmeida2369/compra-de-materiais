import random

def random_generator():
    return random.randint(1, 10)


def random_generator2():
    return random.randint(0, 3)


def random_generator5():
    return random.randint(2, 5)


def random_generator4():
    return random.randint(1, 15)


def random_generator3():
    ruas = ["Centro", "Pirituba", "leopoldina", "perdizes", "jaragua"]
    return random.choice(ruas)





produtos={1:["Plástico", (random_generator()),  (random_generator2()), (random_generator3())],
        2:["Vidro", (random_generator()),  (random_generator2()), (random_generator3())],
        3:["Papelão", (random_generator()),  (random_generator2()), (random_generator3())],
        4:["Isopor", (random_generator()),  (random_generator2()), (random_generator3())],
        5:["Latinha", (random_generator()),  (random_generator2()), (random_generator3())],
        6:["Madeira", (random_generator4()),  (random_generator5()), (random_generator3())],
        7:["Metal", (random_generator4()),  (random_generator5()), (random_generator3())],
        8:["Tecido", (random_generator()),  (random_generator2()), (random_generator3())],
}

carrinho=[]


fim="CONTINUAR"






while fim!="FINALIZAR":

    r=str(input("Digite um dos materias que procura: latinhas, papelão, vidro, madeira, isopor, plástico, metal, tecido\n"))

    if r=="plástico" or r=="PLÁSTICO" or r=="plastico" or r=="PLASTICO":

        print("-"*20)
        print("Temos os seguintes anúncios:\n")

        print("Produto:", produtos[1][0], "/ Quantidade:", produtos[1][1], "/ Preço por unidade:", produtos[1][2], "/ Rua:", produtos[1][3])
        print("-"*20)

        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        print("-"*20)

        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":

            carrinho.append(produtos[1])
            print("-"*20)
            print("Os itens foram adicionados ao seu carriho!\n")

            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="vidro" or r=="VIDRO":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[2][0], "/ Quantidade:", produtos[2][1], "/ Preço por unidade:", produtos[2][2], "/ Rua:", produtos[2][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[2])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="papelão" or r=="PAPELÃO" or r=="papelao" or r=="PAPELAO":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[3][0], "/ Quantidade:", produtos[3][1], "/ Preço por unidade:", produtos[3][2], "/ Rua:", produtos[3][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[3])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="isopor" or r=="ISOPOR":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[4][0], "/ Quantidade:", produtos[4][1], "/ Preço por unidade:", produtos[4][2], "/ Rua:", produtos[4][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[4])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="latinha" or r=="LATINHA":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[5][0], "/ Quantidade:", produtos[5][1], "/ Preço por unidade:", produtos[5][2], "/ Rua:", produtos[5][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[5])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="madeira" or r=="MADEIRA":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[6][0], "/ Quantidade:", produtos[6][1], "/ Preço por unidade:", produtos[6][2], "/ Rua:", produtos[6][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[6])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="metal" or r=="METAL":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[7][0], "/ Quantidade:", produtos[7][1], "/ Preço por unidade:", produtos[7][2], "/ Rua:", produtos[7][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[7])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue

    elif r=="tecido" or r=="TECIDO":
        print("-"*20)
        print("Temos os seguintes anúncios:\n")
        print("Produto:", produtos[8][0], "/ Quantidade:", produtos[8][1], "/ Preço por unidade:", produtos[8][2], "/ Rua:", produtos[8][3])
        print("-"*20)
        r1=str(input("Deseja os itens desse anúncio? Digite SIM ou NÃO: "))
        if r1=="SIM" or r1=="sim" or r1=="s" or r1=="ss":
            carrinho.append(produtos[8])
            print("Os itens foram adicionados ao seu carriho!\n")
            fim=str(input("CONTINUAR as compras ou FINALIZAR?: "))
        else:
            continue







soma=0
#condição usada para linkar o final da repetição While à esta parte final
if fim=="FINALIZAR":
    print("-"*20)
    print("-"*20)
    print("Este é seu carrinho de compras:\n")
    print("-"*20)

    for i in carrinho:

        print("Produto:", i[0], "/ Quantidade:", i[1], "/ Preço:", i[2], "/ Rua:", i[3])
        print("-"*20)
        #calculo do preço dos itens do carrinho
        calculo=i[1]*i[2]
        soma=soma+calculo
    print("-"*20)
    #o programa printa o preço final
    print(f"O preço final da sua compra é {soma} reais")
    #o usuario decide se vai continuar a compra
    r2=str(input("Finalizar compra? "))
    print("-"*20)


    if r2=="SIM"or r2=="sim" or r2=="s" or r2=="ss" or r2=="FINALIZAR" or r2=="finalizar":
        print("-"*20)
        r3=int(input("Qual a forma de pagamento?\n PIX [1]  Cartão de crédito [2]  Cartão de débito [3] \n"))
        print("-"*20)
        if r3==1:
            print("Chave PIX: 40238917409823\n")
            print("Aguardando pagemento...\n")
            print("Aguardando pagemento...\n")
            print("Aguardando pagemento...\n")
            print("Pagamento recebido, retire seus produtos nas ruas: ")
            for i in carrinho:
                print("Rua:", i[3])
                print("-"*20)
            print("Finalizado.")
        if r3==2 or r3==3:
            cartao=str(input("Nome: "))
            cartao1=int(input("Digite o CPF: "))
            cartao2=int(input("Digite a data de vencimento no formato XX.XX.XX: "))
            cartao3=int(input("Digite o CVV: "))
            print("Aguardando pagemento...")
            print("Aguardando pagemento...")
            print("Aguardando pagemento...")
            print("Pagamento recebido, retire seus produtos nas ruas: ")
            for i in carrinho:
                print("Rua:", i[3])
                print("-"*20)
            print("Finalizado.")
    else:
        print("Compra cancelada. Programa finalizado.")
