#include<iostream>
#include<conio.h>
#include<stdlib.h>

using namespace std;

void leerdatos();
void multiplicar(int **, int**,int ,int,int);
void resultados(int **,int,int);

int **puntero_matriz1, **puntero_matriz2,**matrizC, filas, col, filas2, col2;

int main(){
     leerdatos();

        for (int i = 0; i < filas2; i++)
    {
        delete[] puntero_matriz2[i];
    }
    delete[] puntero_matriz2;
    for (int i = 0; i < filas; i++)
    {
        delete[] puntero_matriz1[i];
    }
    delete[] puntero_matriz1;
     

getch();
return 0;

}

void leerdatos(){

     //Presentacion del programa y solicitamos los datos
     cout<<""<<endl;
     
     cout<<""<<endl;
     cout<<"--------------------------"<<endl;
     cout<<"MULTIPLICACION DE MATRICES"<<endl;
     cout<<"--------------------------"<<endl;
     cout<<""<<endl;
     cout<<"Datos de la MATRIZ 1"<<endl;
     cout<<""<<endl;
     cout<<"Ingrese el numero de filas:  ";
     cin>>filas;
     cout<<"Ingrese el numero de columnas: ";
     cin>>col;
     cout<<""<<endl;
     cout<<"Datos de la MATRIZ 2"<<endl;
     cout<<""<<endl;
     cout<<"Ingrese el numero de filas:  ";
     cin>>filas2;
     cout<<"Ingrese el numero de columnas: ";
     cin>>col2;
     cout<<""<<endl;
     
     if (col = filas2)
     {
       puntero_matriz1 = new int*[filas]; //Reservamos memoria para las filas de la matriz 1
     for (int i=0; i<filas; i++){
          puntero_matriz1 [i] = new int[col]; //Reservamos memoria para las columnas de la matriz 1
     }
       puntero_matriz2 = new int*[filas2]; //Reservamos memoria para las filas de la matriz 2
     for (int i=0; i<filas2; i++){
          puntero_matriz2 [i] = new int[col2]; //Reservamos memoria para las columnas de la matriz 2
     }
     cout<<"Ingrese los elementos de la PRIMERA MATRIZ: "<<endl;
     
     for (int i = 0; i < filas; i++){
          for (int j=0; j<col; j++)
          {
               cout<<"Ingresa los valores ["<<i<<"]["<<j<<"]:";
               cin>> *(*(puntero_matriz1+i)+j); //Guardamos los valores ingresados por el usuario
               cout<<""<<endl;
          }
     }
     cout<<""<<endl;
     cout<<"LA MATRIZ 1 ES:"<<endl;
     cout<<""<<endl;
     for(int i=0; i<filas; i++)
	{
 		for(int j=0; j<col; j++)
 		{
  		cout<<*(*(puntero_matriz1+ i)+ j)<<" ";
   	}
       cout<<"\n";
	}
     
     //Reservamos memoria para la MATRIZ 2

   

     cout<<"\nIngrese los elementos de la SEGUNDA MATRIZ: \n";
     cout<<""<<endl;
     for (int i = 0; i < filas2; i++){
          for (int j = 0; j < col2; j++)
          {
               cout<<"Ingresa los valores ["<<i<<"]["<<j<<"]:";
               cin>> *(*(puntero_matriz2+i)+j); //Guardamos los valores ingresados por el usuario
               cout<<""<<endl;
          }
     }
     cout<<""<<endl;
     cout<<"LA MATRIZ 2 ES:"<<endl;
     cout<<""<<endl;
     
      for(int i=0; i<filas2; i++)
	{
 		for(int j=0; j<col2; j++)
 		{
  	cout<<*(*(puntero_matriz2+ i)+ j)<<" ";
   	}
       cout<<"\n";
	}   
     multiplicar(puntero_matriz1, puntero_matriz2, filas,col,col2);
     resultados(matrizC, filas, col2);
     }
      
     
    /* filas3 = filas;
     col3 = col2;*/
     
     //Reservamos memoria para la MATRIZ 1
     
}


void multiplicar(int **puntero_matriz1, int **puntero_matriz2,int filas,int col,int col2){
     cout<<""<<endl;
     
   matrizC = new int* [filas];
    // matriz  b
    for (int i = 0; i < filas; i++)
    {
        matrizC[i] = new int[col2]; // reservando memoria  para las columnas
    }
     for (int i = 0; i < filas; i++){
          for (int j = 0; j < col2; j++)
          {
                (* (*(matrizC + i) + j) = 0);
               for (int k = 0; k<col; k++)
               {
                     * (*(matrizC + i) + j) += ( * (*(puntero_matriz1 + i) + k)) *  (*(*(puntero_matriz2 + k)+j));

               }
               
              
          }
}        
}



void resultados(int **matrizC,int filas,int col2){
     cout<<""<<endl;
     cout<<"El resultado de la multiplicacion de MATRIZ 1 y MATRIZ 2 es: "<<endl;
     cout<<""<<endl;
     for (int i = 0; i < filas; i++){
          for (int j = 0; j < col2; j++)
          {
              cout<< *(*(matrizC+i)+j)<< " "; 
          }
     cout<<"\n";     
}        

/* 3x2 2x4*/
}
