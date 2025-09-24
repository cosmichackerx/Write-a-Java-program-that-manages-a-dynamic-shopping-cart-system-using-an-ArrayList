# 📝 Program Statement (Assignment)

`Write-a-Java-program-that-manages-a-dynamic-shopping-cart-system-using-an-ArrayList
`

```
our program should:

Create an ArrayList of String type to store shopping cart items.

Add Elements → Add at least 5 items (including duplicates, e.g., “Milk” twice).

Access an Element → Display the first item in the cart.

Change an Element → Replace one item with a new one (e.g., change “Milk” to “Soy Milk”).

Remove an Element → Remove an item by index (e.g., remove the 3rd item).

ArrayList Size → Print the total number of items currently in the cart.

Loop Through an ArrayList → Display all items using a loop.

Other Types → Create a second ArrayList of Integer type for item quantities (e.g., [2, 1, 3…]).

Sort an ArrayList → Sort the shopping cart items alphabetically.

The var Keyword (Java 10+) → Use var to create another ArrayList for discount codes.

The List Interface → Declare the shopping cart as List<String> instead of ArrayList<String>.
```

```java
import java.util.*;
import java.io.*;

class shop{

    void shopping(){
        ArrayList<String> cart = new ArrayList<>(); // Create an ArrayList of String type to store shopping cart items.

        // Add Elements → Add at least 5 items (including duplicates, e.g., “Milk” twice).
        cart.add("Apple"); // 0
        cart.add("Banana"); // 1
        cart.add("Orange"); // 2
        cart.add("Watermelon"); // 3
        cart.add("Pineapple"); // 4
        cart.add("Mango"); // 5
        cart.add("Strawberry"); // 6
        cart.add("Apple"); // 7
        cart.add("Milk"); // 8

        System.out.println(cart.get(0)); // Access an Element → Display the first item in the cart.
        cart.set(0, "Milk"); // Change an Element → Replace one item with a new one (e.g., change “Milk” to “Soy Milk”).
        System.out.println("After replacing 0 with milk : "+cart.get(0));
        cart.remove(0); // Remove an Element → Remove an item by index (e.g., remove the 3rd item).
        System.out.println(cart.size()); // ArrayList Size → Print the total number of items currently in the cart.

        // Loop Through an ArrayList → Display all items using a loop.
        for(int i=0;i<cart.size();i++){
            System.out.println(cart.get(i));
        }

        // Sort an ArrayList → Sort the shopping cart items alphabetically.
        Collections.sort(cart);
        System.out.println(cart);

        // Other Types → Create a second ArrayList of Integer type for item quantities (e.g., [2, 1, 3…]).
        ArrayList<Integer> list = new ArrayList<>();
        list.add(1);
        list.add(2);
        list.add(3);

        Collections.sort(list);
        System.out.println(list);

        // The var Keyword (Java 10+) → Use var to create another ArrayList for discount codes.
        var discode = new ArrayList<Integer>();
        discode.add(100157);
        discode.add(100159);
        discode.add(1001611);

        System.out.println("Enter any number for discount : "+discode);

        // The List Interface → Declare the shopping cart as List<String> instead of ArrayList<String>.
        List<String> newlist = new ArrayList<>(cart.size());
        System.out.println(cart);


    }
}

public class Main {
    public static void main(String[] args) {

        shop shop = new shop();
        shop.shopping();

    }
}

/*
📝 Program Statement (Assignment)

“Write a Java program that manages a dynamic shopping cart system using an ArrayList.”

Your program should:

Create an ArrayList of String type to store shopping cart items.

Add Elements → Add at least 5 items (including duplicates, e.g., “Milk” twice).

Access an Element → Display the first item in the cart.

Change an Element → Replace one item with a new one (e.g., change “Milk” to “Soy Milk”).

Remove an Element → Remove an item by index (e.g., remove the 3rd item).

ArrayList Size → Print the total number of items currently in the cart.

Loop Through an ArrayList → Display all items using a loop.

Other Types → Create a second ArrayList of Integer type for item quantities (e.g., [2, 1, 3…]).

Sort an ArrayList → Sort the shopping cart items alphabetically.

The var Keyword (Java 10+) → Use var to create another ArrayList for discount codes.

The List Interface → Declare the shopping cart as List<String> instead of ArrayList<String>.
 */
```
