# ExercicioAulaDePOO

import java.util.Locale;
import java.util.Scanner;
class Main {

  public static void main(String[] args) {  

		int questao;
		Locale.setDefault(Locale.US);
		Scanner sc = new Scanner(System.in);
		do {
			System.out.println("Informa qual questão deseja desenvolver: ");
			System.out.println("");
			System.out.println("1 - Cálculo Triângulo, circulo, quadrado, retângulo, trapéio ");
			System.out.println("2 - Ler duas Peças e Calcular o valor total da Nota ");
			System.out.println("3 - DIFERENCA = (A * B - C * D). ");
			System.out.println("4 - Cálculo de Almoço");
			System.out.println("5 - Compra de Bolsa");
			System.out.println("0 - Sair");
					
			questao = sc.nextInt();
			
			if (questao == 0) {
				System.out.println("\nAté Logo!");
				sc.close();			
			}
			
			switch (questao){
	        case 1:
	    			  double numA,numB,numC;

          
          System.out.printf("Digite o valor de A:");
          numA = sc.nextDouble();
          System.out.printf("Digite o valor de B:");
          numB = sc.nextDouble();
          System.out.printf("Digite o valor de C:");
          numC = sc.nextDouble();
          sc.close();
          
          double AreaDoT = (numA * numC) / 2;
          System.out.println("A) Sua área do Triângulo é:" + AreaDoT);
          double pi = 3.14159;
          double AreaDoC = pi * Math.pow(numC, 2);
          System.out.println("B) Sua área do Circulo é:" + AreaDoC);
          double AreaDoTrapezio = ((numA + numB) / 2 ) * numC;
          System.out.println("C) Sua área do Trapézio é:" + AreaDoTrapezio);
          double AreaDoQuadrado = Math.pow(numB,2);
          System.out.println("D) Sua área do Quadrado é:" + AreaDoQuadrado);
          double AreaDoRetangulo = numA * numB;
          System.out.println("E) Sua área do Retângulo é:" + AreaDoRetangulo);
          

	    		break;	    		
	        case 2:
	    		 System.out.print("Digite o código da peça 1: ");
    int codigo1 = sc.nextInt();
           System.out.print("Digite o número de peças 1: ");
    int quantPeca1 = sc.nextInt();
    System.out.print("Digite o valor da peça 1: ");
    double valorPeca1 = sc.nextDouble();
          System.out.print("Digite o código da peça 2: ");
   int codigo2 = sc.nextInt();
          System.out.print("Digite o número de peças 2: ");
    int quantPeca2 = sc.nextInt();
    System.out.print("Digite o valor da peça 2: ");
    double valorPeca2 = sc.nextDouble();
    sc.close();


    System.out.printf("VALOR PEÇA 1: %.2f R$\nVALOR PEÇA 2: %.2f R$", quantPeca1 * valorPeca1, quantPeca2 *    valorPeca2);
    System.out.println(" ");
	            break;	            
	        case 3:
	    		int A , B , C , D, Diferenca;

          System.out.printf("Digite o valor de A:");
          A = sc.nextInt();
          System.out.printf("Digite o valor de B:");
          B = sc.nextInt();
          System.out.printf("Digite o valor de C:");
          C = sc.nextInt();
          System.out.printf("Digite o valor de D:");
          D = sc.nextInt();

          Diferenca = (A*B)-(C*D);
          System.out.println("Diferença é: " + Diferenca);
	    		break;	    		
	        case 4:
	          double  PesoPorQuilo, PrecoFinal;
          System.out.printf("Digite o Quilo:");
          PesoPorQuilo = sc.nextDouble();
          PrecoFinal = 23 * PesoPorQuilo;
          System.out.println("Você vai Pagar: " + PrecoFinal );
      
	            break;	            
	        case 5:	        	           
	            System.out.println("---- LOJA DE BOLSA ----_-");
          System.out.println("1- Bolsa Gucci - 5000 R$");
          System.out.println("2- Bolsa Louis Vuitton - 10000 R$");
          System.out.println("3- Bolsa Christian Dior - 3000 R$");
          System.out.println("4- Bolsa Hermès - 7000 R$");
          System.out.println("5- Bolsa Prada - 2000 R$");
          System.out.println("0- Sair");
          int valor = sc.nextInt();
    
            if (valor == 1){ 
              System.out.println("Bolsa Gucci");
              System.out.println("Formas de pagamentos: ");
              System.out.println("A VISTA: - Desconto 10% - " + (5000 - (5000*0.10)) + " R$");
              System.out.println("PARCELADO EM 2X -   " + 5000 / 2);
              System.out.println("PARCELADO EM 10X -Acréscimo 5% - " + ((5000 * 0.05) + 5000) / 10 +   " R$\n");
              
            }else if (valor == 2){ 
              System.out.println("Louis Vuitton");
              System.out.println("Formas de pagamentos: ");
              System.out.println("A VISTA: - Desconto 10% - " + (10000 - (10000*0.10)) + " R$");
              System.out.println("PARCELADO EM 2X -   " + 10000 / 2);
              System.out.println("PARCELADO EM 10X -Acréscimo 5% - " + ((10000 * 0.05) + 10000) / 10 +   " R$\n");
              
            }else if (valor == 3){ 
              System.out.println("Christian Dior");
              System.out.println("Formas de pagamentos: ");
              System.out.println("A VISTA: - Desconto 10% - " + (3000 - (3000*0.10)) + " R$");
              System.out.println("PARCELADO EM 2X -   " + 3000 / 2);
              System.out.println("PARCELADO EM 10X -Acréscimo 5% - " + ((3000 * 0.05) + 3000) / 10 +   " R$\n");
              
            }else if (valor == 4){ 
              System.out.println("Hermès");
              System.out.println("Formas de pagamentos: ");
              System.out.println("A VISTA: - Desconto 10% - " + (7000 - (7000*0.10)) + " R$");
              System.out.println("PARCELADO EM 2X -   " + 7000 / 2);
              System.out.println("PARCELADO EM 10X -Acréscimo 5% - " + ((7000 * 0.05) + 7000) / 10 +   " R$\n");
              
            }else if (valor == 5){ 
              System.out.println("Prada");
              System.out.println("Formas de pagamentos: ");
              System.out.println("A VISTA: - Desconto 10% - " + (2000 - (2000*0.10)) + " R$");
              System.out.println("PARCELADO EM 2X -   " + 2000 / 2);
              System.out.println("PARCELADO EM 10X -Acréscimo 5% - " + ((2000 * 0.05) + 2000) / 10 +   " R$\n");
              
            }else{
              System.out.println("Até logo!\n");
            }
	            break;	        
			}			
		} while (questao != 0);		
		sc.close();		
    
    
  }
  

  
}
