# Average

import java.util.Scanner;

public class Averages {

    public static void main(String[] args) {
        try {
            int sum = 0;

            Scanner sc = new Scanner(System.in);
            System.out.println("Enter size of array");
            int n = sc.nextInt();

            int a[] = new int[n];
            System.out.println("Enter elements of array");
            for (int i = 0; i < n; i++) {
                a[i] = sc.nextInt();
                sum = sum + a[i];
            }

            int avg = sum / n;
            System.out.println("Average = " + avg);
        } catch (Exception ex) {
            System.out.println(ex);
        }
    }
}
