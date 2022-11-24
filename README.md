# -constractor-overloading
//writing program through java in oop

* To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package lab;
import java.util.Scanner;
/**
 *
 * @author student
 */

class person {
    String name;
    String id;
    int age;
    Scanner scan=new Scanner(System.in);
    person(){
        System.out.println("enter details=");
        System.out.println("id=");
        id=scan.next();
         System.out.println("name=");
        name=scan.next();
         System.out.println("age=");
        age=scan.nextInt();
    }
    person( String n,String i,int a){
          name=n;
    id=i;
     age=a;
    }
    person(person p1){
         this.id= p1.id;
        this.name=p1.name;
        this.age=p1.age;
    }
     void display(){
         System.out.println("id="+id);
        System.out.println("name="+name);
        System.out.println("age="+age);
        
    }
}
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package inheritancelab;



/**
 *
 * @author student
 */
public class lab {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
          person p1=new person();
          person p2=new person("numl-s22-1102","Nayyab",15);
          person p3=new person(p1);
          student s1=new student();
          teacher t1=new teacher();
          p1.display();
          p2.display();
          p3.display();
          
          
    }
    
}
