import java.util.Scanner;

//instrução1
//instrução2
//instrução3
//instrução4
//instrução5
//...

class CalculoTriangulo {
  
	public static void main(String args[]){  
   
    		Scanner teclado = new Scanner(System.in);
    
    		
            double lado1;
			double lado2;
			double lado3;
			double mult;
            double area;
			double p;
       
	        System.out.printf("insira o lado1: \n" );
            lado1 = teclado.nextDouble();
			
			System.out.printf("insira o lado2: \n" );
			lado2 = teclado.nextDouble();
			
			System.out.printf("insira o lado3: \n" ); 
			lado3 = teclado.nextDouble();
			
			
			if(lado1 == lado2 && lado1 ==lado3){
			System.out.printf("seu triangulo e equilatero\n\n");
			}
			
			if(lado1 == lado2 && lado1 != lado3){
		    System.out.printf("seu triangulo e isoceles \n\n");
			}
			
			if(lado1 != lado2 && lado1 !=lado3){
			 System.out.printf("seu triangulo e escaleno \n\n");
			}
  
            
            p = (lado1 + lado2 + lado3) / 2;
			System.out.printf("O perimetro do triangulo e: \n" + p + "cm \n");
			
  
		    area  =  p *((p-lado2) * (p-lado2) * (p-lado3));
            area  = Math.sqrt(area);
			System.out.printf("a area do triangulo e: \n" + area + "cm \n");
			
			System.exit(0);
		
	}

}
