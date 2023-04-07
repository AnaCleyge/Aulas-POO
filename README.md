# Aulas-POO
Aulas Anima
public class MatrizAleatoria {
        public static void main(String[] args) {
            
        int[][] matriz = new int[7][7];

        Random rand = new Random();
        for (int i = 0; i < 7; i++) {
            for (int j = 0; j < 7; j++) {
                matriz[i][j] = rand.nextInt(10);
            }
        }

        for (int i = 0; i < 7; i++) {
            for (int j = 0; j < 7; j++) {
                System.out.print(matriz[i][j] + " ");
            }
            System.out.println();
        }

        int maiorNumero = matriz[0][0];
        int linhaMaiorNumero = 0;
        int colunaMaiorNumero = 0;
        for (int i = 0; i < 7; i++) {
            for (int j = 0; j < 7; j++) {
                if (matriz[i][j] > maiorNumero) {
                    maiorNumero = matriz[i][j];
                    linhaMaiorNumero = i;
                    colunaMaiorNumero = j;
                }
            }
        }
        System.out.println("O maior número da matriz é " + maiorNumero + " e sua posição é (" + linhaMaiorNumero + "," + colunaMaiorNumero + ")");

        int maiorValorLinha3 = matriz[3][0];
        int menorValorLinha3 = matriz[3][0];
        for (int j = 0; j < 7; j++) {
            if (matriz[3][j] > maiorValorLinha3) {
                maiorValorLinha3 = matriz[3][j];
            }
            if (matriz[3][j] < menorValorLinha3) {
                menorValorLinha3 = matriz[3][j];
            }
        }
        System.out.println("O maior valor da linha 3 é " + maiorValorLinha3 + " e o menor valor da linha 3 é " + menorValorLinha3);

        int maiorValorLinha5 = matriz[5][0];
        int menorValorLinha5 = matriz[5][0];
        for (int j = 0; j < 7; j++) {
            if (matriz[5][j] > maiorValorLinha5) {
                maiorValorLinha5 = matriz[5][j];
            }
            if (matriz[5][j] < menorValorLinha5) {
                menorValorLinha5 = matriz[5][j];
            }
        }
        System.out.println("O maior valor da linha 5 é " + maiorValorLinha5 + " e o menor valor da linha 5 é " + menorValorLinha5);
    }
}
