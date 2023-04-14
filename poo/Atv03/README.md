### Notebook - Atv03
**********************
###### Apresente a soma de todos os argumentos inteiros ou reais recebidos.
					
### Atividade Atv03
 
* Item 1 - Usando a classe JOptionPane para entrada de dados, receba a nota de duas provas e de um trabalho.
* Item 2 - Calcule a média
* Item 3 - Mostre a média usando o showMessageDialog da classe JOptionPane

###### IFPR - Campus Cascavel
###### Disciplina:Programação Orientada à Objetos
###### Aluno:Luiz Carlos de Souza
###### Data da criação:11/04/2023 
 
#### Código Comentado:
// importando biblioteca JOptionPane para abrir janelas

import javax.swing.JOptionPane;


public class Atv03{
    public static void main(String args[]){
        String aux; // variável aux para criar o obejeto do tipo JOptionPane
        
        float p1=0, p2=0, t1=0, media=0; //variáveis para calculos das notas
        
        try { // try catch para entrada das notas
            aux = JOptionPane.showInputDialog("Entre com  a nota 1");
            p1 = Float.parseFloat(aux);

            aux = JOptionPane.showInputDialog("Entre com a nota 2");
            p2 = Float.parseFloat(aux);

            aux = JOptionPane.showInputDialog("Entre com a nota do trabalho");
            t1 = Float.parseFloat(aux);
            
        } catch (NumberFormatException erro) { // caso digitado caracteres apresenta mensagem de erro
            JOptionPane.showMessageDialog(null,"Entre somente com numeros" + erro.toString());
        }
        
        // realizando o calculo das notas
        media = ((p1 + p2 + t1)/3);
        
        // mostrando a mensagem na tela com JOptionpane
        JOptionPane.showMessageDialog(null,"Nota 1:"+ p1 +"Nota 2:"+ p2 +"Trablho:"+ t1 +"Média notas foi="+ media);
        System.exit(0);



    }

}
