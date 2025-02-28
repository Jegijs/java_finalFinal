To launch the app press the manual start button in IDea. 

To use person class use, example(You can choose whatever the persons name and other details are) = Person person1 = new Person("John", "Doe", 25, 1.80, 75, "Latvia", 2000, true); 

To see the person class with all the set details use: person1.printInfo();

Regarding the bonus task where you could add an option to restart the app and add an option to input invalid data repeatedly, I thought I could implement a while cycle, however I didnt find a way to implement it like I would like so didnt add it:

Scanner scanner = new Scanner(System.in);

while (true) {  // Loop to restart the survey if needed
    System.out.println("Lai restartētu aptauju, ievadi: 0");
    System.out.println("Ievadi uzvārdu: ");

    if (lastName.equals("0")) {
        System.out.println("Restarting survey...");
        continue; // Restarts the loop
    }

    if (lastName.isEmpty()) {
        System.out.println("Uzvārds nevar būt tukšs. Lūdzu, ievadiet vēlreiz.");
        continue;  // Asks for input again
    }

    // If input is valid, break the loop and continue the program
    break;
}

// Continue with the rest of the program...
System.out.println("Paldies! Tavs uzvārds ir: " + lastName);
