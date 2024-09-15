import javax.swing.JOptionPane;
public class ContagemIdade {
    public static void main (String args[]){
        int nasc[] = new int[3], atual[] = new int[3];
        nasc[0] = Integer.parseInt(JOptionPane.showInputDialog("Digite o dia do nascimento"));
        nasc[1] = Integer.parseInt(JOptionPane.showInputDialog("Digite o mes do nascimento"));
        nasc[2] = Integer.parseInt(JOptionPane.showInputDialog("Digite o ano do nascimento"));
        atual[0] = Integer.parseInt(JOptionPane.showInputDialog("Digite o dia atual"));
        atual[1]= Integer.parseInt(JOptionPane.showInputDialog("Digite o mes atual"));
        atual[2] = Integer.parseInt(JOptionPane.showInputDialog("Digite o ano atual"));
        JOptionPane.showMessageDialog(null,"A idade é: " + Function_Idade(nasc, atual)[0] + " dias, " + Function_Idade(nasc, atual)[1] + " meses, " + Function_Idade(nasc, atual)[2] + " anos.");
    }
    
    public static int[] Function_Idade(int nasc[], int atual []){
        int idade[] = new int [3];
       
        //cálculo dos dias
        if (nasc[0] < atual[0]){
            idade[0] = atual[0] - nasc[0];
        }
        else if (nasc[0] > atual [0]){
            if (atual[1] == 4 && atual[1] == 6 && atual[1] == 9 && atual[1] == 11){
                atual[0] = atual[0] + 30;
            }
            else if (atual[1] == 2){
                if (atual[2]%4 == 0){
                    atual[0] = atual[0] + 29;
                }
                else{
                    atual[0] = atual[0] + 28;
                }
            }
            else{
                atual[0] = atual[0] + 31;
            }
            idade[0] = atual[0] - nasc[0];
            atual[1] = atual[1] - 1;
        }
        
        //cálculo dos meses
        if (nasc[1] < atual[1]){
            idade[1] = atual[1] - nasc[1];
        }
        else if(nasc[1] > atual[1]){
            atual[1] = atual[1] + 12;
            idade[1] = atual[1] - nasc[1];
            atual[2] = atual[2] - 1;
        }
       
        
        //calculo dos anos
        idade[2] = atual[2] - nasc[2];
       
        
        //retorno
        return idade;
    }
}
