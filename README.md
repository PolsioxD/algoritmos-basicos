# algoritmos-basicos
//Algoritmos basicos para empezar en java 
package Paquete;

import java.util.Scanner;

public class Principal {
    public static void main(String []args){

        Scanner sp = new Scanner(System.in);

        System.out.println("\n-Ingrese su nombre completo: ");
        String nombre = sp.nextLine();
        System.out.println("\n-Igrese las horas trabajadas: ");
        int horas = sp.nextInt();
        System.out.println("\n-Ingrese el valor de cada hora: ");
        int valor = sp.nextInt();
        System.out.println("\n-Ingrese el interes por deducciones por ley: ");
        double interes = sp.nextDouble();

        int total1 = horas * valor;
        System.out.println("señor= " +nombre+ "su sueldo sin descuento es: " +total1);

        double total2 = total1*(interes/100);
        System.out.println("\n-Se le descontara " +total2+ " por deducciones de ley");
        double total3 = total1 - total2;
        System.out.println("Señor" +nombre+ "su salario bruto del mes es:" +total3);
        }
    }
