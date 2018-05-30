# Encapsulamento
Aula sobre Encapsulamento com JAVA


Encapsulamento
Encapsulamento vem de encapsular, que em programação orientada a objetos significa separar o programa em partes, o mais isolado possível. A idéia é tornar o software mais flexível, fácil de modificar e de criar novas implementações. O Encapsulamento serve para controlar o acesso aos atributos e métodos de uma classe. É uma forma eficiente de proteger os dados manipulados dentro da classe, além de determinar onde esta classe poderá ser manipulada. Usamos o nível de acesso mais restritivo, private, que faça sentido para um membro particular. Sempre usamos private, a menos que tenhamos um bom motivo para deixá-lo com outro nível de acesso. Não devemos permitir o acesso público aos membros, exceto em caso de ser constantes. Isso porque membros públicos tendem a nos ligar a uma implementação em particular e limita a nossa flexibilidade em mudar o código. O encapsulamento que é dividido em dois níveis:

Nível de classe: Quando determinamos o acesso de uma classe inteira que pode ser public ou Package-Private (padrão);
Nível de membro: Quando determinamos o acesso de atributos ou métodos de uma classe que podem ser public, private, protected ou Package-Private (padrão).
Então para ter um método encapsulado utilizamos um modificador de acesso que geralmente é public, além do tipo de retorno dele. Para se ter acesso a algum atributo ou método que esteja encapsulado utiliza-se o conceito de get e set. Por definição, com SET é feita uma atribuição a algum atributo, ou seja, define, diz o valor que algum atributo deve ter. E  com GET é possível recuperar esse valor. 

Exemplo:

private String atributo1 = new String();  
private String atributo2 = new String();  
public String getAtributo1(){  
  return this.atributo1;  
}  
public String getAtributo2(){  
  return this.atributo2;  
} 
 
Exemplo:

public class Pessoa{
  private String nome;
  private String sobrenome;
  private String dataNasc;
  private String rg;
  private String[] telefones;
   
  public String getNome(){
    return nome;
  }
  public void setNome(String n){
    nome = n;
  }
  public String getSobrenome(){
    return sobrenome;
  }
  public void setSobrenome(String s){
    sobrenome = s;
  }
  public String getDataNasc(){
    return dataNasc;
  }
  public void setDataNasc(String d){
    dataNasc = d;
  }
  public String getRg(){
    return rg;
  }
  public void setRg(String r){
    r = rg;
  }
  public String getTelefones(){
    return telefones;
  }
  public void setTelefones(String[] telefones){
    telefones[] = telefones;
  }
}
