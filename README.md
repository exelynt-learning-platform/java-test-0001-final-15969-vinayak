# java-test-0001-final-15969-vinayak
Final Project Assignment - This repository contains the complete final project code and documentation.
public class HollowDiamondPattern {
    public static void main(String[] args) {
        int n = 5;

        // Upper part
        for (int i = 1; i <= n; i++) {

            // Spaces before star
            for (int j = i; j < n; j++) {
                System.out.print(" ");
            }

            // Stars with hollow center
            for (int k = 1; k <= (2 * i - 1); k++) {
                if (k == 1 || k == (2 * i - 1))
                    System.out.print("*");
                else
                    System.out.print(" ");
            }

            System.out.println();
        }

        // Lower part
        for (int i = n - 1; i >= 1; i--) {

            // Spaces before star
            for (int j = n; j > i; j--) {
                System.out.print(" ");
            }

            // Stars with hollow center
            for (int k = 1; k <= (2 * i - 1); k++) {
                if (k == 1 || k == (2 * i - 1))
                    System.out.print("*");
                else
                    System.out.print(" ");
            }

            System.out.println();
        }
    }
}
