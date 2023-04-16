### Notebook - Atv06
**********************				
 
* Item 1 - Dados os valores de um depósito fixo mensal e um montante desejado, crie uma classe para determinar quantos meses serão necessários para acumular o montante desejado, considerando juros mensais de 0,5%. 


#### Código java Comentado:
/*
 Atividade Atv01 onde sera aperesentado a soma de n termos 
 IFPR - Campus Cascavel
 Disciplina:Programação Orientada à Objetos
 Aluno:Luiz Carlos de Souza
 Data da criação:16/04/2023 
 */

// neste exemplo a taxa de juros permaeceu aberta para o usuário digitar.
// import da classe Scanner para entrada de dados.
import java.util.Scanner;

public class Atv06 {
    public static void main(String [] args){
        // declaração do obejtos Scanner.
        Scanner EntradaDados = new Scanner(System.in);
        
        //Declaração das variáveis.
        double deposito, capitalDesejado;
        double taxa;
        int mes=0,ano;
        double totalJuros=0,acumulado=0;
        
        //Print para informar como classe funciona.
        System.out.println("\nClasse para calculo de juros simples para um montante :\n1º-Informe o Valor desejado.\n2º-Informe a taxa de juros.\n3º A saída sera a quantidade de meses,\npara obeter o valor desejado.\n");

        //solicitando o montante desejado.
        System.out.println("Informe o valor do montante desejado ex: R$ 16 ou R$ 160");
        capitalDesejado = EntradaDados.nextDouble();
        
        //solicitando os valores fixos dos depositos.
        System.out.println("Informe o valor do deposito fixo ex:R$ 10 ou 20");
        deposito = EntradaDados.nextDouble();
        
        //solicitando a taxa de juros para o usuário.
        System.out.println("Informe a uma tava de juros, utilize virgula para numeros quebrados ex:5 ou 0,5 %");
        taxa = EntradaDados.nextDouble();

        // while para calculo da taxa de juros mais acumulado
        while (acumulado != capitalDesejado){
            mes += 1;
            totalJuros = ((((deposito*taxa)/100)*mes));
            acumulado = totalJuros + deposito;
            
            //print mostrando valor mês a mês.
            //System.out.printf("Para %d meses o Total de Juros será R$ %.2f acumulando o total de R$ %.2f \n",mes,totalJuros,acumulado); 
        } 
        // if/ else para apresentar a saida tratando meses e anos    
        if (mes >= 12){
            ano = (mes/12);
            mes = (mes%12);
            System.out.printf("Para acumuluar valor R$ %.2f\nSerá Necessários %d ano e %d meses\nTaxa de Juros: %.0f %%\n",acumulado,ano,mes,taxa);

        }else{
            System.out.printf("Para acumuluar valor R$ %.2f.\nSerá Necessários %d meses\nTaxa de Juros a: %.2f\n",acumulado,mes,taxa);
            
        }

    }
    
}
