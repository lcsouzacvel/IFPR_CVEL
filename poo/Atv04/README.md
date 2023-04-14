### Notebook - Atv04
**********************				
 
* Item 1 - Declare uma variável do tipo real chamada gastosJaneiro e inicialize-a com o valor gasto no mês de janeiro, declare também as variáveis gastosFevereiro e gastosMarco, inicializando-as com os respectivos gastos, utilize uma linha para cada declaração.
* Item 2 - Crie uma variável chamada gastosTrimestre e inicialize-a com a soma das outras variáveis.


#### Código java Comentado:
/*
 IFPR - Campus Cascavel
 Disciplina:Programação Orientada à Objetos
 Aluno:Luiz Carlos de Souza
 Data da criação:14/04/2023 
*/


// importantando pacote NumberFormat para apresentar valores das variáveis gastos em valor moeda
//import java.text.NumberFormat;
// cita o padrão da região que os dados serão apresentados neste exemplpo sera pt BR
//import java.util.Locale; 

public class Atv04{
    public static void main(String[] args){
        
        //Iniciando o objeto locale para pt BR
        //Locale localeBrasil = new Locale("pt","BR");
        
 
        //Inicializando as variáveis
        float gastosJaneiro = 8594;
        float gastosFevereiro = 3544;
        float gastosMarco = 5964;
        float gastosTrimestre=0;
        
        
        //Utilizando a classe NumberFormat para formatar a saida em R$ Br
        //NumberFormat valormoedaBr = NumberFormat.getCurrencyInstance(localeBrasil);

        
        //Variável gastoTrimestre recebendo os valores 
        gastosTrimestre = (gastosJaneiro + gastosFevereiro + gastosMarco);
        
        
        //Apresentando os gastosTrimestre com classe NumberFormat
        //System.out.println("Total de gastos do trimestre foi de " + valormoedaBr.format(gatosTrimestre));
        
        
        //apresentando de forma normal
        System.out.printf("Total gastos no Trimestre = R$ %.2f\n", + gastosTrimestre);


    }
    
}
