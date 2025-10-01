# Simple Food Vending Machine (java)
#simple Java console-based food ordering system

import java.util.*;

public class Main

{

public static void main(String[] args) {

Scanner s = new Scanner(System.in);

int pay;

String choice;

System.out.println("HI,Plz enter ur name:");

String name = s.nextLine();

System.out.println("Plz enter ur mobileno:");

String mobileno=s.next();

do{

System.out.println("hey "+name+",");

System.out.println(mobileno);

System.out.println("MENU");

System.out.println("1.Dal fry - 40"+"\n 2.paneer butter masala - 100"+"\n 3.chicken curry - 120"+" \n 4. fish fry - 100"+" \n 5. tomato curry - 30");

System.out.println("Select from the menu:");

int select = s.nextInt();

System.out.println("Enter quantity:");

int quan=s.nextInt();

switch(select){

case 1:

System.out.println("you selected dal fry pay "+quan*40+"rs");

System.out.println("Enter the amount to be paid:");

pay=s.nextInt();

if(pay==40*quan){

System.out.println("order placed");

}

else{

System.out.println("invalid order");

}

break;

case 2:

System.out.println("you selected paneer butter masala pay "+quan*100+"rs");

System.out.println("Enter the amount to be paid:");

pay=s.nextInt();

if(pay==100*quan){

System.out.println("order placed");

}

else{

System.out.println("invalid order");

}

break;

case 3:

System.out.println("you selected chicken curry pay"+quan*120+"rs");

System.out.println("Enter the amount to be paid:");

pay=s.nextInt();

if(pay==120*quan){

System.out.println("order placed");

}

else{

System.out.println("invalid order");

}

break;

case 4:

System.out.println("you selected fish fry pay"+quan*100+"rs");

System.out.println("Enter the amount to be paid:");

pay=s.nextInt();

if(pay==100*quan){

System.out.println("order placed");

}

else{

System.out.println("invalid order");

}

break;

default:

System.out.println("you selected tomato curry pay"+quan*30+"rs");

System.out.println("Enter the amount to be paid:");

pay=s.nextInt();

if(pay==30*quan){

System.out.println("order placed");

}

else{

System.out.println("invalid order");

}

break;

}

System.out.println("DO you want to order again?(yes/no):");

choice = s.next();

}

while (choice.equalsIgnoreCase("yes"));


System.out.println("Thank you for ordering ");

}

}
