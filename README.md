# Trabajo-Final-Progamaci-n-1
package programas;

import java.util.Scanner;

public class Final {
    public static void main(String[] args) {
        String codigoproducto=" ";
        int kilos = 0;
        float precio = 0;
        float importeFactura = 0;
        float facturacionTotal = 0;
        int contador = 0;
        int totalKilos = 0;
        Scanner sc=new Scanner(System.in);

        for (int i=1; i<=2; i++) {
            System.out.println("Factura número: " +i);
            System.out.println("Código del producto: ");
            codigoproducto=sc.next();
            System.out.println("Cantidad en kilos: ");
            kilos=sc.nextInt();
            System.out.println("Precio Total: ");
            precio = sc.nextFloat();
            importeFactura = kilos * precio;
            facturacionTotal = importeFactura + facturacionTotal;

            if (importeFactura>=100){
                contador++;
            }
            totalKilos = kilos + totalKilos;

        }
        System.out.println("Los Detalles de la venta son: ");
        System.out.println("Facturación Total: S/. " + facturacionTotal);
        System.out.println("Total de Kilos Vendidos: " + totalKilos);
// Código del producto "Azucar" es: UPC1
// Código del producto "Sal" es: UPC2
// Código del producto "Arroz" es: UPC3
// Código del producto "Lentejas" es: UPC4
// Código del producto "Pimienta" es: UPC5
// Código del producto "Manzana" es: UPC6
// Código del producto "Pera" es: UPC7
// Código del producto "Galleta" es: UPC8
// Código del producto "Gelatina" es: UPC9
// Código del producto "Flan" es: UPC10
    }
}
