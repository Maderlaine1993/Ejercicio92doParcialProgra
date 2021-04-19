# Ejercicio92doParcialProgra
/* Maderlaine Vanessa Aldana Martinez Carne 0909-20-6881
Ingenieria en Sistemas 
2do. Parcial Programación I
Ejercicio 9*/

//Declaración de librerias a utilizar 
#include <iostream>
#include <windows.h>
#include <conio.h>

using namespace std; 

int main ()
{
	int a[5], b[5]; //declaración de vectores
	float p1=0, p2=0; //declaración de variables promedio 
	int op=0; //declaración de switch
	int i,j,k; //variable tipo pointer 
	
	do //menu de opciones
	{
		system ("cls"); system("color f3"); 
		cout<< "1.- Ingreso de Datos"<<endl;
		cout<< "2.- Visualización primera nota Curso 1"<<endl;
		cout<< "3.- Visualización ultima nota Curso 2"<<endl;
		cout<< "4.- Calculo de Promedios de los Cursos"<<endl;
		cout<< "5.- Visualización de datos"<<endl;
		cout<< "6.- FIN"<<endl;
		cin>>op;
		cout<<endl;
		
		switch (op)
		{
			case 1: 
			for (i=0; i<5; i++)
			{
				cout<< "Notas Curso 1"<<endl;
				cin>>a[i];
			}
			for (j=0; j<5; j++)
			{
				cout<< "Notas Curso 2"<<endl;
				cin>>b[j];
			}
			break;
			
			case 2: 
				system("cls");
				cout<<endl;
				cout<<"Primera nota curso 1 :  "<< a[0] <<endl;
				cout<<endl;
				system("pause");
				break;
			
			case 3:
				system("cls");
				cout<<endl;
				cout<<"Ultima nota curso 2 :  "<< b[2] <<endl;
				cout<<endl;
				system("pause");
				break;
		
			case 4:
				system("cls");
				cout<<endl;
				cout<<"Promedios de los Cursos"<<endl;
				p1= (a[0]+a[1]+a[2]+a[3]+a[4])/5;
				p2= (b[0]+b[1]+b[2]+b[3]+b[4])/5;
				cout<< "Promedio Curso 1 : " << p1 << endl;
				cout<< "Promedio Curso 2 : " << p2 << endl;
				cout<<endl;
				system("pause");
				break;
				
			case 5:
				system("cls");
				cout<<endl;
				cout<<"Visualización de Datos:"<<endl;
				cout<<"Curso 1"<<endl;
				cout<< a[0] << "     " << a[1] << "     "<< a[2] << "      "<< a[3] << "     " << a[4] <<endl;
				cout<<"Promedio del Curso 1 :" <<p1<<endl;
				cout<<endl;
				cout<<"Curso 2"<<endl;
				cout<< b[0] << "     " << b[1] << "     "<< b[2] << "      "<< b[3] << "     " << b[4] <<endl;
				cout<<"Promedio del Curso 2 : "<<p2<<endl;
				cout<<endl;
				system("pause");
				break;
			case 6:
				system("cls");
				cout<<endl;
				cout<<"¿Seguro que deseas salir del programa?:"<<op<<endl;
				cout<<endl;
				system("pause");
				break;
		}
	}
	while(op);
	_getch();
}
/* Maderlaine Vanessa Aldana Martinez Carne 0909-20-6881
Ingenieria en Sistemas 
2do. Parcial Programación I
Ejercicio 9*/
