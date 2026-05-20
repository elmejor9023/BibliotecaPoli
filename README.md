[Ejercicio1.java](https://github.com/user-attachments/files/28040056/Ejercicio1.java)
[Ejercicio2.java](https://github.com/user-attachments/files/28040059/Ejercicio2.java)package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio2 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double celsius, fahrenheit;[Uploading Ejercicio3.java…]()


        System.out.print("Ingrese la temperatura en grados Celsius: ");
        celsius = entrada.nextDouble();

        fahrenheit = (celsius * 9/5) + 32;

        System.out.println("La temperatura en Fahrenheit es: " + fahrenheit);

    }
}

package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio3 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double nota1, nota2, nota3, promedio;

        System.out.print("Ingrese la primera nota: ");
        nota1 = entrada.nextDouble();

        System.out.print("Ingrese la segunda nota: ");
        nota2 = entrada.nextDouble();

        System.out.print("Ingrese la tercera nota: ");
        nota3 = entrada.nextDouble();

        promedio = (nota1 + nota2 + nota3) / 3;

        System.out.println("El promedio final es: " + promedio);

    }
}
package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio4 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        int numero;

        System.out.print("Ingrese un número entero: ");
        numero = entrada.nextInt();

        if (numero % 2 == 0) {
            System.out.println("El número es PAR.");
        } else {
            System.out.println("El número es IMPAR.");
        }

    }
}
package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio5 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double horasTrabajadas, valorHora, salario;

        System.out.print("Ingrese las horas trabajadas: ");
        horasTrabajadas = entrada.nextDouble();

        System.out.print("Ingrese el valor por hora: ");
        valorHora = entrada.nextDouble();

        salario = horasTrabajadas * valorHora;

        System.out.println("El salario total es: $" + salario);

    }
}
ackage fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio6 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double num1, num2, num3;

        System.out.print("Ingrese el primer número: ");
        num1 = entrada.nextDouble();

        System.out.print("Ingrese el segundo número: ");
        num2 = entrada.nextDouble();

        System.out.print("Ingrese el tercer número: ");
        num3 = entrada.nextDouble();

        if (num1 >= num2 && num1 >= num3) {
            System.out.println("El número mayor es: " + num1);
        } else if (num2 >= num1 && num2 >= num3) {
            System.out.println("El número mayor es: " + num2);
        } else {
            System.out.println("El número mayor es: " + num3);
        }

    }
}
package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio7 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        int numero;

        System.out.print("Ingrese un número: ");
        numero = entrada.nextInt();

        System.out.println("Tabla de multiplicar del " + numero + ":");

        for (int i = 1; i <= 10; i++) {
            System.out.println(numero + " x " + i + " = " + (numero * i));
        }

    }
}
package fundamentosprogramacion;

public class Ejercicio8 {

    public static void main(String[] args) {

        int contador = 1;

        while (contador <= 100) {

            System.out.println(contador);

            contador++;
        }

    }
}
package fundamentosprogramacion;

import java.util.Scanner;

public class Ejercicio9 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double num1, num2, resultado;
        int opcion;

        System.out.print("Ingrese el primer número: ");
        num1 = entrada.nextDouble();

        System.out.print("Ingrese el segundo número: ");
        num2 = entrada.nextDouble();

        System.out.println("\nSeleccione una operación:");
        System.out.println("1. Suma");
        System.out.println("2. Resta");
        System.out.println("3. Multiplicación");
        System.out.println("4. División");

        System.out.print("Opción: ");
        opcion = entrada.nextInt();

        switch (opcion) {

            case 1:
                resultado = num1 + num2;
                System.out.println("Resultado: " + resultado);
                break;

            case 2:
                resultado = num1 - num2;
                System.out.println("Resultado: " + resultado);
                break;

            case 3:
                resultado = num1 * num2;
                System.out.println("Resultado: " + resultado);
                break;

            case 4:
                if (num2 != 0) {
                    resultado = num1 / num2;
                    System.out.println("Resultado: " + resultado);
                } else {
                    System.out.println("Error: No se puede dividir entre cero.");
                }
                break;

            default:
                System.out.println("Opción inválida.");
        }

    }
}
public class Ejercicio10 {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);

        double compra, descuento, total;

        System.out.print("Ingrese el valor de la compra: ");
        compra = entrada.nextDouble();

        if (compra >= 100000) {

            descuento = compra * 0.10;
            total = compra - descuento;

            System.out.println("Descuento aplicado: $" + descuento);
            System.out.println("Total a pagar: $" + total);

        } else {

            System.out.println("No aplica descuento.");
            System.out.println("Total a pagar: $" + compra);

        }

    }

