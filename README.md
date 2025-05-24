# Arrreglos: Crear un programa que recorra un arreglo de enteros y al encontrar números impares, 
duplique su valor y muestre el nuevo arreglo con esos valores.  Arreglo original: [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,98,12]


#include <stdio.h>

int main() {
	int arr[]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,98,12};
	int n=sizeof(arr)/sizeof(arr[0]);//define la cantidad de elementos que hay en el arreglo
	printf("arreglo original: ");
	for( int i=0;i<n;i++){ //recorrido del arreglo
		printf("%d ",arr[i]);
	}
	for( int i=0;i<n;i++){ //modifica los valores impares	
		if(arr[i]%2!=0){
			arr[i]*=2;
		}
	}
	printf("\narreglo modificado: ");
	for( int i=0;i<n;i++){ 
		printf("%d ",arr[i]);
	}
	return 0;
}
