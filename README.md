# Pilha
Pilha(último a entrar, primeiro a sair)

package pilha;

import java.util.LinkedList;
import java.util.List;

public class Pilha {

    public static void main(String[] args) {
    
        //cria a lista dinâmica
        List<Integer> pilha = new LinkedList();
        pilha.add(4);
        pilha.add(1);
        pilha.add(152);
        pilha.add(154);
        pilha.add(54);
        pilha.add(14);
        pilha.add(15);
        
        //percorre a lista e imprime
        System.out.println("pilha de números:");
        int aux = 0;
        for (int i = 0; i < pilha.size(); i++) {
            aux = pilha.get(i);
            System.out.println(aux);
        }
        
        //começa a lista pelo final (assim como uma pilha)
        System.out.println("-----------");
        int fim = pilha.size() - 1;
        System.out.println("ultimo número:");
        System.out.println(pilha.get(fim));
        pilha.remove(fim);
        
        fim = pilha.size() - 1;
        System.out.println("ultimo número:");
        System.out.println(pilha.get(fim));
        pilha.remove(fim);
        
        fim = pilha.size() - 1;
        System.out.println("ultimo número:");
        System.out.println(pilha.get(fim));
        pilha.remove(fim);
        
        //percorre a lista e imprime
        System.out.println("-----------");
        System.out.println("pilha reajustada:");
        aux = 0;
        for (int i = 0; i < pilha.size(); i++) {
            aux = pilha.get(i);
            System.out.println(aux);
        }
    }
}
