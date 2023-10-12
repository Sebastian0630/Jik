# Jik
import math


while True:
    print("------------------------------------------------")
    print("Pc Kuli - 1 | V Kuli - 2")
    print("Pc Walca - 3 | pc szesciana - 4")
    print("pc prostopadloscianu - 5 | ")
    print("pc ostroslupa - 6 | ")
    print("pc graniastoslupa - 7")
    print("8 - wyjdz z programu")
    print("------------------------------------------------")
    inp = input("Podaj liczbe: ")
    if "1" == inp:
        r = float(input("r = "))
        Pc_kuli = 4/3*math.pi*pow(r,3)
        print(f"Pc-Kuli = {Pc_kuli}")
    elif "2" == inp:
        r = float(input("r = "))
        V_kuli = 4*math.pi*pow(r,2)
        print(f"V kuli = {V_kuli}")        
    elif "3" == inp:
        r = float(input("r = "))
        h = float(input("h = "))
        Pc_walca = 2*math.pi*h+2*math.pi*r*pow(2)
        print(f"Pc walca = {Pc_walca}")
    elif "4" == inp:
        a = float(input("a = "))
        Pc_szesciana = 6*(a**2)
        print(f"Pc szesciana = {Pc_szesciana}")
    elif "5" == inp:
        a = float(input("a = "))
        b = float(input("b = "))
        c = float(input("c = "))
        Pc_prostopadlosciana = (2*a*b)+(2*b*c)+(2*a*c)
        print(f"pc prostopadlosciana = {Pc_prostopadlosciana}")
    elif "6" == inp:
        Pp = float(input("Pp = "))
        Pb = float(input("Pb = "))
        Pc_ostroslupa = Pp+Pb
        print(f"Pc ostroslupa = {Pc_ostroslupa}")
    elif "7" == inp:
        Pp = float(input("Pp = "))
        Pb = float(input("Pb = "))
        Pc_graniastoslupa = 2*(Pp+Pb)
        print(f"Pc graniastoslupa = {Pc_graniastoslupa}")
    elif "8" == inp:
        break
