#include <stdio.h>
#include <string.h>
#include <ctype.h>
 
int esVocal(char c);
int main(){
	
char nombre[100];
char vocales[5]={'a','e','i','o','u' };
int i,r,p;
	
printf("Reglas\n puedes introducir como maximo 100 carateres.\n Puestes intrtroducir numeros  del (0) al (9) y letras de la (a) a la (z). \n");
printf("\nTeclea una cadena:");
scanf("%s", nombre);
    //printf("%s\n", nombre); // sirve para ver la cadena guardada
	
while (nombre[i]){
   if (isalpha(nombre[i])) r=r+1;
    else p=p+1;
    i++;
   }

 printf("Numeros %d\n", p);
 printf("Consonantes %d\n", r);
 return 0;
  
}
