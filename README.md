# numero-perfecto-en-Java-
 UN PROGRAMA QUE AVERIGUE SI UN NUMERO NATURAL POSITIVO ES PERFECTO O EN JAVA
/**
 * @author Gaby
 * /*UN NUMERO NATURAL SE DENOMINA PERFECTO CUANDO ES IGUAL A LA SUMA DE TODOS SUS DIVISORES, PRIMOS O NO EXCEPTO EL MISMO. POR EJEMPLO
 * 28=1+2+4+7+14. 
 * ESCRIBE UN PROGRAMA QUE AVERIGUE SI UN NUMERO NATURAL POSITIVO ES PERFECTO O NO*/
 
 import java.util.Scanner; //<--importamps scaneer para la entrada de datos
 
public class ejercicios2 {//<--- clase 

	
	public static void main(String[] args) {
		
		 int i;
		 int suma = 0;//<--- variables  
		 int  numero; //<---donde almacenamos el numero 
		 int opc;
		 
	        Scanner gaby = new Scanner(System.in);
	        
	        do {
	        System.out.println("Introduce un número un numero : ");
	        numero = gaby.nextInt();
	        
	        
	        
	        
	        for (i = 1; i < numero; i++) {  // usamos el bucle for para ir aumentando hasta llegar al numero                        
	            if (numero % i == 0) {//<--- si el numero es divisible entre los numeros que voy recorriendo 
	                suma = suma + i;   // si es asi entonces la variable suma aumenta el valor del iterador 
	            }
	        }
	        if (suma == numero) {  //<---- una ves acabado el bucle   si el numero es igual a la suma de sus divisores es perfecto                
	            System.out.println("el numero ingresado es Perfecto");
	        } else { 
	            System.out.println("El numero ingresado No es perfecto");//caso contrario no es perfecto

	        }
	        System.out.println("desea repetir ? presione 1 para repetir el proceso  y 2 para finalizar ");
	        opc = gaby.nextInt();
	        }while(opc == 1 );
	        System.out.println("programa finalizadom que le vaya bien ");
		
		

	}

}
