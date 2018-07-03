# Objetos_get_set

#Classe Cachorro
import javax.swing.*;

public class Cachorro{
    String nome;
    int idade;

    public Cachorro(){

        //JOptionPane.showMessageDialog(null,getNomeCachorro());
    }

    public Cachorro(String nome) {
        this.nome = nome;
        //JOptionPane.showMessageDialog(null,"Nome: "+this.nome);
    }

    public void setNomeCachorro(String nome){
        this.nome = nome;
    }

    public String getNomeCachorro(){
        return nome;
    }

    public void meuCachorro(String nome, Integer idade){
        this.nome = "Suzi";
        this.idade = 10;
        JOptionPane.showMessageDialog(null,"Nome"+this.nome+" Idade: "+this.idade);
    }

    public String lateCachorro(){
        return ("Au au");
    }
}

#Classe Principal
import javax.swing.*;

public class Principal {

    public static void main(String[] args) {

        Cachorro c1 = new Cachorro("simba");
        Cachorro c2 = new Cachorro();
        c2.setNomeCachorro("Suzi");
        JOptionPane.showMessageDialog(null,c2.getNomeCachorro());
    }
}


