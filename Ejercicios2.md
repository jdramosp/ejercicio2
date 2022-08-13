package ejercicio_java2;

/**
 *
 * @author Julio Ramos
 */
public class metodoNumMenor {
    

   static int metodoNumMenor (int numero[])
   {
   
       int menor;
       menor=numero[0];
       for(int i=0; i<numero.length;i++)
       {
       
           if(numero[i]<menor)menor=numero[i];
        }
       return menor;
          
    }
}


----------------------------------------------------------------------


package ejercicio_java2;

import java.util.Scanner;

/**
 *
 * @author Julio Ramos
 */
public class Ejercicio_java2 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        Scanner opcion = new Scanner(System.in);
        
 
{
   int num;
   int ingresado[]=new int[3];
     System.out.println("Los números añadidos son:" );
   for(int i=0; i<ingresado.length; i++)
   {      
      ingresado[i] = opcion.nextInt();
     }
   num = metodoNumMenor.metodoNumMenor(ingresado);
    System.out.println("El número menor es:"+num);
}
    }
}
