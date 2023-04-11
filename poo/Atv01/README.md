### Notebook - Atv01
**********************

Atv01

Apresente a soma de todos os argumentos inteiros ou reais recebidos
					
#### Código Comentado:

 Atividade Atv01 onde sera aperesentado a soma de n termos 
 IFPR - Campus Cascavel
 Disciplina:Programação Orientada à Objetos
 Aluno:Luiz Carlos de Souza
 Data da criação:11/04/2023 
 
##Codigo 

import java.util.Scanner; // Importação da classe Scanner do pacote java.util para ler os valores digitados
import java.io.IOException; // Importação da classe IOException para tratar exeções

Scanner leitura = new Scanner(System.in); // prepada a entrada dos valores  na variável "valor"
        String s = ""; // inicia a variável s com valor vazio
        double soma = 0, valores = 0; // inicia as variáveis para leitura e soma 

        System.out.println("Digite os valores a ser somados, DIGITE s Sair");
        
        while(!"s".equals(s)){ // utilizando o metodo .equals porque s é uma variável do tipo String
            
            valores = leitura.nextDouble();// utilizando o objeto do tipo Scanner leitura 
            s = String.valueOf(valores); // passa para a variável s o que foi lido na variável Scanner 
            soma += valores;// soma os valores cada vez que passa por leitura acumula em valores          
            System.out.println("TOTAL DA SOMA =" + soma);// printa o total acumulado do valores
                
        }   
        leitura.close();// fecha a variável do tipo Scanner 
