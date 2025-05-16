# Desafio-10
# QUESTAO 1
```java
package desafio;

public class Desafio {

    public static void main(String[] args) {
        int[] a = {26, 15, 10, 11, 83, 15, 4, 2, 21, 7};
        int[] b = {56, 64, 59, 55, 54, 32, 28, 25, 57, 19};
        int[] c = new int[10];
        for (int i = 0; i < a.length; i++) {
            c[i] = a[i] + b[i];
            System.out.println(a[i] + " + " + b[i] + " = " + c[i]);
        }
    }

}
```
# QUESTAO 2
```java
package desafio10;

public class Desafio {

    public static void main(String[] args) {
        int[] a = {2, 1, 1, 18, 13, 5, 4, 2, 31, 9};
        int[] b = {1, 0, 59, 55, 54, 36, 28, 28, 19, 9};
        int[] c = new int[10];
        for (int i = 0; i < a.length; i++) {
            c[i] = a[i] - b[i];
            System.out.println(a[i] + " - " + b[i] + " = " + c[i]);
        }
    }

}
```
# QUESTAO 3
```java
    int[] vetor = new int[10];
        int i;
        int max, min;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite 10 números inteiros:");
        for (i = 0; i < 10; i++) {
            vetor[i] = ler.nextInt();
        }

        max = vetor[0];
        min = vetor[0];

        for (i = 1; i < 10; i++) {
            if (vetor[i] > max) {
                max = vetor[i];
            }
            if (vetor[i] < min) {
                min = vetor[i];
            }
        }
        System.out.println("Valor máximo: " + max);
        System.out.println("Valor mínimo: " + min);
    }

}
```
# QUESTAO 4
```java

      int[] vetor = new int[10];
        int i;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite 10 números inteiros:");
        for (i = 0; i < 10; i++) {
            vetor[i] = ler.nextInt();
        }
        
        System.out.println("Números pares no vetor:");
        for (i = 0; i < 10; i++) {
            if (vetor[i] % 2 == 0) {
                System.out.println(vetor[i]);
            }
        }
    }
}
```
# QUESTAO 5
```java
 int[] vetor = new int[10];
        int i;
        Scanner ler = new Scanner(System.in);
        
        System.out.println("Digite 10 números inteiros:");
        for (i = 0; i < 10; i++) {
            vetor[i] = ler.nextInt();
        }

    
        System.out.println("Números ímpares no vetor:");
        for (i = 0; i < 10; i++) {
            if (vetor[i] % 2 != 0) {
                System.out.println(vetor[i]);
            }
        }
    }
}
```
# QUESTAO 6
```java
  int[] vetor = new int[10];
        int i;
        int soma;
        int quant;
        double media;
        Scanner ler = new Scanner(System.in);

        soma = 0;
        quant = 0;

        System.out.println("Digite 10 números inteiros:");
        for (i = 0; i < 10; i++) {
            vetor[i] = ler.nextInt();
        }

        for (i = 0; i < 10; i++) {
            if (i % 2 == 0) {
                soma += vetor[i];
                quant++;
            }
        }

        media = (double) soma / quant;

        System.out.println("Média dos valores nas posições pares: " + media);
    }
}
```
# QUESTAO 7
```java
 int[] vetor = new int[10];
        int i;
        int cont;
        Scanner ler = new Scanner(System.in);
        cont = 0;

        System.out.println("Digite 10 números inteiros:");
        for (i = 0; i < 10; i++) {
            vetor[i] = ler.nextInt();
        }

        for (i = 0; i < 10; i++) {
            if (i % 2 == 0) {
                cont++;
            }
        }

        System.out.println("Quantidade de elementos em índices pares: " + cont);
    }
}
```
# QUESTAO 8
```java
  int[] vetorOri = new int[30];
        int[] vetorMod = new int[30];
        int i;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite 30 números inteiros (use 0 para representar nulo):");
        for (i = 0; i < 30; i++) {
            vetorOri[i] = ler.nextInt();
        }

        for (i = 0; i < 30; i++) {
            if (vetorOri[i] == 0) {
                vetorMod[i] = 10;
            } else {
                vetorMod[i] = vetorOri[i];
            }
        }

        System.out.println("Vetor original:");
        for (i = 0; i < 30; i++) {
            System.out.print(vetorOri[i] + " ");
        }

        System.out.println();
        System.out.println("Vetor modificado (com 0 substituído por 10):");
        for (i = 0; i < 30; i++) {
            System.out.print(vetorMod[i] + " ");
        }
    }
}
```
# QUESTAO 9
```java
  int[] vetorA = new int[10];
        int[] vetorB = new int[10];
        int[] vetorRes = new int[10];
        int i;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite 10 números inteiros para o primeiro vetor:");
        for (i = 0; i < 10; i++) {
            vetorA[i] = ler.nextInt();
        }

        System.out.println("Digite 10 números inteiros para o segundo vetor:");
        for (i = 0; i < 10; i++) {
            vetorB[i] = ler.nextInt();
        }

        for (i = 0; i < 10; i++) {
            vetorRes[i] = vetorA[i] * vetorB[i];
        }

        System.out.println("Vetor que gerou-se da multiplicação:");
        for (i = 0; i < 10; i++) {
            System.out.print(vetorResultado[i] + " ");
        }
    }
}
```
# QUESTAO 10
```java
 int[] vetorA = new int[10];
        int[] vetorB = new int[10];
        int i, j;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite 10 números inteiros para o vetor A:");
        for (i = 0; i < 10; i++) {
            vetorA[i] = ler.nextInt();
        }

        j = 9;
        for (i = 0; i < 10; i++) {
            vetorB[i] = vetorA[j];
            j--;
        }

        System.out.print("Vetor B (ordem inversa do vetor A): ");
        for (i = 0; i < 10; i++) {
            System.out.print(vetorB[i] + " ");
        }
    }
}
