# BMI_Rechner


#!/usr/bin/python3

name=input('Name:')
groesse=input('Koerpergroesse:')
bmi=0
while True:
    gewicht=input('Gewicht:')
    if not len(gewicht) > 0:
        break
    try:
        bmi=round(float(gewicht)/(float(groesse)**2),2)
        print(bmi)
    except:
        continue
    if bmi >=25:
        print('Uebergewicht');
    elif bmi <=18.5:
        print('Untergewicht');
    else:
        print('Normalgewicht');
