# Adding-the-sum-of-the-digits.(JAVA)
Adding the sum of the digits without using Modulo operator(%).
<br>
Author Kumar Aaditya

import java.util.Scanner;

public class LoopQuestions {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number: ");
        int num = sc.nextInt();

        int copy = num;
        int final_sum = 0;
        int i = 1;
        while(true){
            int digit = num/10;
            num /= 10;
            if(true) {
                int sum = (copy / 10) * 10;
                sum = copy - sum;
                copy /= 10;
                final_sum += sum;
            }
            if(digit == 0)
                break;
            i++;
        }
        System.out.println(final_sum);
