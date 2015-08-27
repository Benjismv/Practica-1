
package Ejercicios;

public class ej5 {
public static void main(String[] args)throws IOException {

BufferedReader en=new BufferedReader (new InputStreamReader (System.in));

int num,cont,invnum,i,pot,gnum;
int sumainv;
System.out.print("introduzca un numero=");
  num=Integer.parseInt(en.readLine());
  cont=0;
  i=0;
  pot=1;
  sumainv=1;
  gnum=num;
  do { 
    num=num/10; 
    cont+=1;
    } 
    while(num!=0);
      for(i=0;i<(cont-1);i++){ // ciclo para hallar la potencia
     pot=pot*10;
}
  invnum=(gnum/pot);
  do {
  invnum=(gnum%10)*pot;
  sumainv= invnum+sumainv;
  pot=pot/10;
  gnum=gnum/10;
}
    while(pot>1);
      System.out.println("el numero esta formado por="+cont+ " "+"digitos");
        System.out.print("el numero al revés es:"+sumainv); 
    }
}
