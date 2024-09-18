# Java-Projects-Collection
# Java-Projects-Collection
Static blocks in Java are used to initialize static variables or perform any static initialization tasks. Static blocks are executed when the class is first loaded into memory, even before the main method is executed. In this problem, you need to demonstrate the use of a static block to initialize a configuration setting. Implement a class Configuration with a static block that initializes a static variable. Then, use this variable in the main method to display its value.

Create a static variable.

In static block assign the variable the value 1024.

In static method returns the variable and in the main print "Configuration setting is: " + variable.

CODE:

class Main {
    public static void main(String[] args) {
        // Display the configuration setting
        System.out.println("Configuration setting is: " + Configuration.getSetting());
    }
}

class Configuration {
    // Declare a static variable
    private static int setting;

    // Static block to initialize the static variable
    static {
        setting = 1024;

    }

    // Static method to get the value of the static variable
    public static int getSetting() {
        return setting;
    }
}
