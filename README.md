import java.io.IOException;
public class Main
{
  public static void main (String[]args) throws IOException
  {

     caneta c1 = new  caneta ();

      c1.modelo = "Bic Cristal";
      c1.cor = "Azul";
      c1.ponta = 0.5;
      c1.carga = 90;

      c1.tampaF();
      c1.escrever();


  }
}

----------------------------------------------------------------------------------------------------------------------------------------

public class caneta{
 
    String modelo;
    String cor;
    double ponta;
    int carga;
    boolean tampado;

     public String toString() {
     return " Modelo: " + this.modelo + " Cor: " + this.cor + " Ponta: " + this.ponta + " Carga: " + this.carga ;
   }
    public void tampaF(){
      this.tampado = true;
    }
    public void tampaA(){
      this.tampado = false;
    }

     public void escrever(){
       if(this.tampado){
         System.out.println("Já pode começar a escrever com a " + this.modelo + " cor: " + this.cor + " ponta: " + this.ponta + " carga: " + this.carga);
       }else {
         System.out.println("Destampe a caneta!!");
       }
      
    }

    
}
