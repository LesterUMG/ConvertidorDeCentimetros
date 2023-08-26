# TAREA 1 DE ALGORITMOS
# Lester López
## El siguiente programa es sobre la conversión de centímetros a metros, yardas, varas, pulgadas o pies.
>Algoritmo en Pseudocodigo
 ```
 Algoritmo AlgoritmoParaConversionDeUnidades
	//Algoritmo donde el usuario ingrese centimetros para convertirlos en metros, yardas, varas, pulgadas y pies
	Definir num, r Como Real
	Definir opc Como Entero
	Escribir "Ingrese el dato de los centimetros que desea convertir";
	Leer num;
		Escribir "Elija una de las siguientes unidades para convertir tu dato:";
		Escribir "1. Metros";
		Escribir "2. Yardas";
		Escribir "3. Varas";
		Escribir "4. Pulgadas";
		Escribir "5. Pies";
		Leer opc;
		si opc = 1 Entonces
			r = num/100 ;
			Escribir num " centimetros = " r " metros";
		SiNo
			si opc = 2 Entonces
				r = num * 0.0109361
				Escribir r " yardas";
			SiNo
				si opc = 3 Entonces
					r = num / 502.92
					Escribir r " varas";
				SiNo
					si opc = 4 Entonces
						r = num / 2.54
						Escribir r " pulgadas";
					SiNo
						si opc = 5 Entonces
							r = num / 30.48
							Escribir r " pies";
						SiNo
							Escribir "La opcion " opc " no existe";
						FinSi
					FinSi
				FinSi
			FinSi
		FinSi
	
FinAlgoritmo
  ```
---
---
>Algoritmo en C++
 ```C++
 //Programa para realizar conversiones de cm a otra unidades
#include<iostream>
using namespace std;
int main()
{
	double num, r=0;
	int opc;
	cout<< "Ingrese el dato de los centimetros que desea convertir"<<endl; cin>> num;
	cout<< "Elija una de las siguientes unidades para convertir su dato"<<endl;
	cout<< "1. Metros"<<endl;
	cout<< "2. Yardas"<<endl;
	cout<< "3. Varas"<<endl;
	cout<< "4. Pulgadas"<<endl;
	cout<< "5. Pies"<<endl; cin>> opc;
	if(opc==1)
	{
		r=num/100;
		cout<<num<<" centimetros = "<<r<<" Metros";
	}
	else if(opc==2)
	{
		r=num*0.0109361;
		cout<<num<<" centimetros = "<<r<<" yardas";
	}
	else if (opc==3){
		r=num/502.92;
		cout<<num<<" centimetros = "<<r<<" varas";
	}
	else if(opc==4){
		r=num/2.54;
		cout<<num<<" centimetros = "<<r<<"  pulgadas";
	}
	else if(opc==5){
		r=num/30.48;
		cout<<num<<" centimetros = "<<r<<" pies";
	}
	else{
		cout<<"La opcion "<<opc<<" no existe";
	}
		
	return 0;
}
  ```
---
---
>Algoritmo en Phyton
```Python
#Programa para conversion de unidades
num=float(input("Ingrese el numero de centimetros que desea convertir \n"))
opc=int(input("Ingrese una de las siguientes opciones para convertir tu dato: \n"
"1.Metros \n2.Yardas \n3.Varas \n4.Pulgadas \n5.Pies \n"))
if opc == 1 :
    resultado = num / 100 
    print(num,"centimetros =", resultado,"metros")
elif opc == 2 :
    resultado = num * 0.0109361
    print(num,"centimetros =", resultado," yardas")
elif opc == 3 :
    resultado = num / 502.92
    print(num,"centimetros =", resultado," varas")
elif opc == 4 :
    resultado = num / 2.54
    print(num,"centimetros =", resultado," pulgadas")
elif opc == 5 :
    resultado = num / 30.48
    print(num,"centimetros =", resultado," pies" )
else:
    print("Opcion", opc,"no existe")

```
  ---
  ---