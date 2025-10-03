import java.util.Scanner;

public class SistemaEscolar {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double[] notas = new double[8];

        System.out.println("Digite as 8 notas anuais do aluno:");

        for (int i = 0; i < 8; i++) {
            System.out.print("Nota " + (i + 1) + ": ");
            notas[i] = scanner.nextDouble();
        }

        // Cálculo das médias bimestrais
        double b1 = (notas[0] + notas[1]) / 2;
        double b2 = (notas[2] + notas[3]) / 2;
        double semestre1 = (b1 + b2) / 2;

        double b3 = (notas[4] + notas[5]) / 2;
        double b4 = (notas[6] + notas[7]) / 2;
        double semestre2 = (b3 + b4) / 2;

        double mediaFinal = (semestre1 + semestre2) / 2;

        // Exibição dos resultados
        System.out.println("\nPráticas\n");

        System.out.printf("1º Bimestre: %.1f\n", b1);
        System.out.printf("2º Bimestre: %.1f\n", b2);
        System.out.printf("1º Semestre: %.1f\n", semestre1);
        System.out.println("----------------------");

        System.out.printf("3º Bimestre: %.1f\n", b3);
        System.out.printf("4º Bimestre: %.1f\n", b4);
        System.out.printf("2º Semestre: %.1f\n", semestre2);
        System.out.println("-----------------------");

        System.out.printf("Média Final: %.1f\n", mediaFinal);

        scanner.close();
    

import java.util.Scanner;

public class ConversaoTemperaturaCompleta {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Entrada de temperatura em Celsius
        System.out.print("Digite a temperatura em Celsius (°C): ");
        double celsius = scanner.nextDouble();

        // Cálculos de conversão
        double fahrenheit = (celsius * 9 / 5) + 32;
        double kelvin = celsius + 273.15;

        // Exibição dos resultados
        System.out.println("\nPráticas\n");

        System.out.printf("Temperatura em Celsius: %.1f °C\n", celsius);
        System.out.printf("Temperatura em Fahrenheit: %.1f °F\n", fahrenheit);
        System.out.printf("Temperatura em Kelvin: %.2f K\n", kelvin);

        scanner.close();
    }
}


