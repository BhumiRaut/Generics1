# Generics1
package PACK1;
public class L1 {

    public static <NA> int search(NA[] arr, NA t) {
        for (int i = 0; i < arr.length; i++) {
            if (arr[i].equals(t)) {
                return i;
            }
        }
        return -1;
    }

    public static void main(String[] args) {
        String[] vehicles = {"Car", "Bike", "Bus", "Truck", "Scooter"};

        System.out.println("Index of 'Bus': " + search(vehicles, "Bus"));
        System.out.println("Index of 'Train': " + search(vehicles, "Train")); 
    }
}
