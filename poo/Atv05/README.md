### Notebook - Atv05
**********************				
 
* Item 1 - Declare uma variável do tipo real chamada gastosJaneiro e inicialize-a com o valor gasto no mês de janeiro, declare também as variáveis gastosFevereiro e gastosMarco, inicializando-as com os respectivos gastos, utilize uma linha para cada declaração;
* Item 2 - Crie uma variável chamada gastosTrimestre e inicialize-a com a soma das outras variáveis.
* Item 3 - Exiba a variável gastosTrimestre.
* Item 4 - Declare a variável mediaMensal e faça o cálculo para a média mensal de gastos.
* Item 5 - Exiba a mensagem "Valor da média mensal = " juntamente com o valor da média mensal.


#### Código java Comentado:
/*
 IFPR - Campus Cascavel
 Disciplina:Programação Orientada à Objetos
 Aluno:Luiz Carlos de Souza
 Data da criação:14/04/2023 
*/


//import java.text.NumberFormat;  // importantando pacote NumberFormat para apresentar valores das variáveis gastos em valor moeda
//import java.util.Locale; // cita o padrão da região que os dados serão apresentados neste exemplpo sera pt BR

public class Atv05{
    public static void main(String[] args){
        //Iniciando o objeto locale para pt BR
        //Locale localeBrasil = new Locale("pt","BR");
        //Utilizando a classe NumberFormat para formatar a saida em R$ Br
        //NumberFormat valormoedaBr = NumberFormat.getCurrencyInstance(localeBrasil);


        //Inicializando as variáveis
        float gastosJaneiro = 7594;
        float gastosFevereiro = 4544;
        float gastosMarco = 6964;
        float gastosTrimestre = 0;
        float mediaMensal = 0;
        
        
        //Variável gastoTrimestre recebendo os valores 
        gastosTrimestre = (gastosJaneiro + gastosFevereiro + gastosMarco);
        			
        mediaMensal = (gastosTrimestre/3);
        
        
        //Apresentando os gastosTrimestre
        //System.out.println("Total de gastos do trimestre foi de " + valormoedaBr.format(gastosTrimestre));
        //System.out.println("Valor da média mensal = " + valormoedaBr.format(mediaMensal));
       
        System.out.printf("Total gastos no Trimestre = R$ %.2f\n", + gastosTrimestre);
        System.out.printf("Valor da média mensal = R$ %.2f \n", + mediaMensal);
        
        


    }
    
}
