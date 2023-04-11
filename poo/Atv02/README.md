### Notebook - Atv02
**********************

Atv02

Apresente a soma de todos os argumentos inteiros ou reais recebidos
					
#### Código Comentado:

 Atividade Atv02
 
Atv02

Item 1 - Exibir a mensagem “Informe um inteiro: “, deixando o cursor na mesma linha.

Item 2 - Atribuir o produto das variáveis b e c para a variável a.

Item 3 - Demonstrar a execução do cálculo e utilizar um comentário para afirmar que é um programa de exemplo de folha de pagamento.

 IFPR - Campus Cascavel
 Disciplina:Programação Orientada à Objetos
 Aluno:Luiz Carlos de Souza
 Data da criação:11/04/2023 
 
##Codigo 
import java.util.Scanner; // Importação da classe Scanner do pacote java.util para ler os valores digitados.

public class Atv02{
    public static void main(String arg[]){
        Scanner leitura = new Scanner(System.in); // recebe os valores de entrada no objeto tipo Scanner "leitura".
        
        System.out.print("Informe um Inteiro:");// solicita a entrada de um valor inteiro e permanece na mesma linha por causa do print sem o ln.
        int b = leitura.nextInt();// utilizando o objeto do tipo Scanner leitura atribui o valor a variável b.

        System.out.print("Informe um Inteiro:");// solicita a entrada de um valor inteiro e permanece na mesma linha por causa do print sem o ln.
        int c = leitura.nextInt();// utilizando o objeto do tipo Scanner leitura atribui o valor a variável c.
        
        int a = b * c; // realiza o calculo entre b x c onde o resultado é armazenado em a.
        
        System.out.printf("Resultado entre produto %d X %d = %d", b, c, a);
        
        // programa executa um cálculo de exemplo de folha de pagamento
        
        
        leitura.close();

    }

}
