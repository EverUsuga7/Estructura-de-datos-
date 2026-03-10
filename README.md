# Estructura-de-datos-
proyecto de programación, estructura de datos
import java.util.Scanner;

public class DiferenciaArreglos {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Definir dos arreglos unidimensionales para almacenar 7 números
        double[] arreglo1 = new double[7];
        double[] arreglo2 = new double[7];
        double[] arregloDiferencia = new double[7];
        
        // Llenar el primer arreglo
        System.out.println("=== LLENADO DEL PRIMER ARREGLO ===");
        for (int i = 0; i < arreglo1.length; i++) {
            System.out.print("Ingrese el número " + (i + 1) + " para el primer arreglo: ");
            arreglo1[i] = scanner.nextDouble();
        }
        
        // Llenar el segundo arreglo
        System.out.println("\n=== LLENADO DEL SEGUNDO ARREGLO ===");
        for (int i = 0; i < arreglo2.length; i++) {
            System.out.print("Ingrese el número " + (i + 1) + " para el segundo arreglo: ");
            arreglo2[i] = scanner.nextDouble();
        }
        
        // Calcular la diferencia y llenar el tercer arreglo
        for (int i = 0; i < arregloDiferencia.length; i++) {
            arregloDiferencia[i] = arreglo1[i] - arreglo2[i];
        }
        
        // Calcular el promedio del tercer arreglo
        double suma = 0;
        for (int i = 0; i < arregloDiferencia.length; i++) {
            suma += arregloDiferencia[i];
        }
        double promedio = suma / arregloDiferencia.length;
        
        // Mostrar resultados
        System.out.println("\n=== RESULTADOS ===");
        System.out.println("El promedio de los datos del tercer arreglo es: " + promedio);
        
        System.out.println("\n=== DATOS DEL TERCER ARREGLO (DIFERENCIAS) ===");
        for (int i = 0; i < arregloDiferencia.length; i++) {
            System.out.println("Posición " + (i + 1) + ": " + arreglo1[i] + " - " + arreglo2[i] + 
