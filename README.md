#include <stdio.h>
#include <string.h>
#include <ctype.h>

int esVocal(char c);
int main(){
	
char nombre[100];
char vocales[5]={'a','e','i','o','u' };
int i,r,p,e;
e=0;

printf("Reglas\n puedes introducir como maximo 100 carateres.\n Puestes intrtroducir numeros  del (0) al (9) y letras de la (a) a la (z). \n No repueden dejar espacios ni teclear otro carateres diferentes a los ya mencionados.");
printf("\nTeclea una cadena:");
scanf("%s", nombre);
    //printf("%s\n", nombre); // sirve para ver la cadena guardada


	int resultado ,m;
	for (i=0;i<100;i++){
	
 	  resultado = esVocal(nombre[i]);
	  if(resultado == 1){m=1+m;}
	  else { }
}
	
	
// clasifica entre numeros y letras del alfabeto
	while (nombre[e]){
   if (isalpha(nombre[e])) r=r+1;
    else p=p+1;
    e++; }

 printf("Numeros %d\n", p);
 printf("vocales %d\n", m );
 printf("Consonantes %d\n", r=r-1-m);
 return 0;
  
}

int esVocal(char c){

	char vocales[5]= {'a', 'e', 'i', 'o', 'u'};
	int i;
	for (i = 0 ; i<5 ; i++){
		if(c==vocales[i]) return 1;
	}
}
