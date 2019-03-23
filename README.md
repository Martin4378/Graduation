# Graduation

import java.util.Scanner;

public class P44_Graduation {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String studentName = scanner.nextLine();
        int level = 1;
        double averageGrade = 0;

        while (level <= 12) {
            double currentGrade = Double.parseDouble(scanner.nextLine());

            if (currentGrade >= 4.0) {
                level++;
                averageGrade += currentGrade;

            }

            averageGrade /= 12;
            System.out.printf("%s graduated. Average grade: %.2f", studentName, averageGrade);

        }
    }
}
