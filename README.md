# OOPS-in-java-
OOPS in java 
import java.util.Scanner;
public class Main{
    public static void main(String args[]){
        ShopMarket obj=new ShopMarket();
        Scanner sc=new Scanner(System.in);
        obj.setvalues(sc.nextLine(),sc.nextLine(),sc.nextInt(),sc.nextFloat());
        obj.display();
    }
}
class ShopMarket{
    String shopname;
    String items;
    int quantity;
    float price;
    public void setvalues(String shopname,String items,int quantity,float price){
        this.shopname=shopname;
        this.items=items;
        this.quantity=quantity;
        this.price=price;
    }
    public void display(){
        System.out.println("Shop Name:"+shopname);
      System.out.println("Items:"+items);
      System.out.println("Quantity:"+quantity);
      System.out.println("Price:"+price);
    }
}
