///# prueba-punteros

#include <stdio.h>

using namespace std;

short edad = 487;
int numero = 1535;
int *miptr = &numero; //// es equivalente al numero que se encuente en la direccion de memoria de la variable numero.
short *edad = &edad;


typedef struct{
     char nombre[10];
     unsigned char edad;
}registro;
 
void process_reg(registro *actual){
     unsigned char i=0;
     printf("\nnombre: ");
     while(actual->nombre[i] !='\0'){
         printf("%c",actual->nombre[i]);
         i++;
         
        }
        printf("\nedad: %d \n",actual->edad;
       
      }
      
      int main()
      {
          registro sergio={"sergio",24};
          registro xiomara={"xiomara",23};
          
          process_reg(&sergio);
          process_reg(&xiomara);
          
          return 0;
         
        }
