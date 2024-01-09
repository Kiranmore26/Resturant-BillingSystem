# Resturant-BillingSystem

package Anudip;
import java.util.Scanner;

public class My_hotel {

	public static void main(String[] args) 
	{
		int choice,ch1;
		int total=0;
		int  Quantity=1;
		String Item_or=" ";
		char ans;
		Scanner sc=new Scanner(System.in);
		System.out.println("Welcome to Priti's Hotel");
		do
		{
			System.out.println("1:Starters\n2:Main Course\n3:Deserts\n4:Drink");
			choice=sc.nextInt();
			switch(choice)
				{
				case 1:
						System.out.println("Starters:");
						System.out.println("1:MasalaPappad      80Rs.");
						System.out.println("2:panner-chilly     120Rs.");
						System.out.println("3:panner-tikka      150Rs.");
						ch1=sc.nextInt();
						System.out.println("Enter No of Quantities : ");
						Quantity=sc.nextInt();
							switch (ch1) 
							{
							case 1:
								 total=total+80*Quantity;
								 Item_or=Item_or+"MasalaPappad \n";
								break;
							case 2:
								 total=total+120*Quantity;
								 Item_or=Item_or+"panner-chilly \n";
								break;
							case 3:
								 total=total+150*Quantity;
								 Item_or=Item_or+"panner-tikka  \n";
								break;
		
							default:
								System.out.println("Wrong Input");
								break;
							}
						
					break;
				case 2:
					System.out.println("Maain course:");
					System.out.println("1:Palak Paneer    250Rs.");
					System.out.println("2:Biryani      350Rs.");
					System.out.println("3:ButterChicken      500Rs.");
					ch1=sc.nextInt();
					System.out.println("Enter No of Quantities : ");
					Quantity=sc.nextInt();					
						switch (ch1) 
						{
						case 1:
							 total=total+250*Quantity;
							 Item_or=Item_or+"Palak Paneer \n";
							break;
						case 2:
							 total=total+350*Quantity;
							 Item_or=Item_or+"Biryani \n";
							break;
						case 3:
							 total=total+500*Quantity;
							 Item_or=Item_or+"ButterChicken \n";
							break;
		
						default:
							System.out.println("Wrong Input");
							break;
						}
				break;
				case 3:
						System.out.println("Deserts:");
						System.out.println("1:Brownies      100Rs.");
						System.out.println("2:Cakes      120Rs.");
						System.out.println("3:Ice-Cream      150Rs.");
						ch1=sc.nextInt();
						System.out.println("Enter No of Quantities : ");
						Quantity=sc.nextInt();
							switch (ch1) 
							{
							case 1:
								 total=total+100*Quantity;
								 Item_or=Item_or+"Brownies \n";
								break;
							case 2:
								 total=total+120*Quantity;
								 Item_or=Item_or+"Cakes \n";
								break;
							case 3:
								 total=total+150*Quantity;
								 Item_or=Item_or+"ice-cream \n";
								break;
			
						default:
							System.out.println("Wrong Input");
							break;
							}
				break;
				case 4:
						System.out.println("Drinks:");
						System.out.println("1:coffee      60Rs.");
						System.out.println("2:Coke      70Rs.");
						System.out.println("3:7-UP      70Rs.");
						ch1=sc.nextInt();
						System.out.println("Enter No of Quantities : ");
						Quantity=sc.nextInt();
							switch (ch1) 
							{
							case 1:
								 total=total+60*Quantity;
								 Item_or=Item_or+"Coffee \n ";
								break;
							case 2:
								 total=total+70*Quantity;
								 Item_or=Item_or+"Coke \n";
								break;
							case 3:
								 total=total+70*Quantity;
								 Item_or=Item_or+"7-UP \n";
								break;
			
						default:
							System.out.println("Wrong Input");
							break;
							}
				break;
				default:
					System.out.println("Invalid choice");
					break;
				}
				
						System.out.println("Do you want to add any other item Y/N");
						ans=sc.next().charAt(0);
			}
		while(ans=='Y'||ans=='y');
		
		
		System.out.println("***********BILL***********)");	
		System.out.println("Total Items Order :   \n"+Item_or);
		System.out.println("Total Bill is :  "+total);
		System.out.println("***********Thanks for Coming***********");
		System.out.println("***********Visit Again***********)");

	}

}



