import java.util.Scanner;
import java.util.ArrayList;

public class Driver {

	private Scanner input;
	public Board board;
	public Player player;
	int i =0;
	ArrayList<String> playerNames = new ArrayList<String>();

	public Driver()
	{
		input = new Scanner(System.in);
		numberOfPlayers();
	}

	public static void main(String[] argvs){
		Driver driver = new Driver();
	}




	private void numberOfPlayers()
	{
		System.out.println("Enter the number of players: ");
		int i = input.nextInt();
		if (i>=3 && i < 7)
		{
			this.i=i;
			run();
		}
		else
		{
			System.out.println("Invalid Number of Players, has to be between 3 and 6");
			System.out.println("\nPress any key to continue...");
			input.nextLine();
			input.nextLine(); 
			//clear the terminal window and display the main menu again
			System.out.println("\f");
			numberOfPlayers();
		}


	}

	private void run()
	{
		int option = mainMenu();
		while (option != 0)
		{

			switch (option)
			{
			case 1:    addPlayer();
			break;
			}
			System.out.println("\nPress any key to continue...");
			input.nextLine();
			input.nextLine();  //this second read is required - bug in Scanner class; a String read is ignored straight after reading an int.

			//clear the terminal window and display the main menu again
			System.out.println("\f");
			option = mainMenu();
		}   
		System.out.println("Exiting... bye");
		System.exit(0);
	}

	private void firstMenu()
	{
		int option = mainMenu();
		while (option != 0)
		{

			switch (option)
			{
			case 1:    addPlayer();
			break;
		//	case 2:    load
			}
			System.out.println("\nPress any key to continue...");
			input.nextLine();
			input.nextLine();  //this second read is required - bug in Scanner class; a String read is ignored straight after reading an int.

			//clear the terminal window and display the main menu again
			System.out.println("\f");
			option = mainMenu();
		}   
		System.out.println("Exiting... bye");
		System.exit(0);
	}
	
	private int mainMenu()     
	{ 
		System.out.println("Welcome to Stocks and Shares");
		System.out.println("---------");     
		System.out.println("  1) Add Player Names");    
		int option = input.nextInt();
		return option;	
	}
	
	private int mainMenuTwo()
	{
		System.out.println("Stocks and Shares");
		System.out.println("---------");     
		System.out.println("  1) Draw Card");
		System.out.println("   2)  Get Current Stock Prices");
		System.out.println("   3)  Save Game");
		
		int option = input.nextInt();
		return option;	
	}


	private void addPlayer()  
	{
		for(int b=0; b<i; b++)
		{
			System.out.println("Player Number " + (b+1) + " enter your name: ");
			String c = input.nextLine();
			c = input.nextLine();
			playerNames.add(c);

		}
	}
}
