package com.mycompany.soma;

import java.util.Scanner;


public class SOMA {

    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
   public class Fibonacci {
    public static void main(String[] args) {
        // Número a ser verificado na sequência de Fibonacci
        int numero = 21; // Você pode alterar este valor para o número desejado
        
        if (verificaFibonacci(numero)) {
            System.out.println(numero + " pertence à sequência de Fibonacci.");
        } else {
            System.out.println(numero + " não pertence à sequência de Fibonacci.");
        }
    }
    
    public static boolean verificaFibonacci(int num) {
        int anterior = 0;
        int atual = 1;
        
        if (num == anterior || num == atual) {
            return true;
        }
        
        while (atual < num) {
            int proximo = anterior + atual;
            anterior = atual;
            atual = proximo;
            
            if (atual == num) {
                return true;
            }
        }
        
        return false;
    }
}
}
