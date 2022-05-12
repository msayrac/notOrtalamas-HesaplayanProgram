# notOrtalamas-HesaplayanProgram
Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın.

Ödev
Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.

Not : If ve Else kullanılmayacak...

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        // variables
        int mat, phy, chem, lit, music;

        // Scanner class described
        Scanner input = new Scanner(System.in);

        // user login

        System.out.println("Please enter math point :");
        mat = input.nextInt();

        System.out.println("Please enter physics point :");
        phy = input.nextInt();

        System.out.println("Please enter literature point :");
        lit = input.nextInt();

        System.out.println("Please enter music point :");
        music = input.nextInt();

        double avg = (mat+phy+lit+music)/4;

        System.out.println("ortalamanız : " + avg);

        String result = 50<avg ? "Pass" : "Fail";

        System.out.println("Your final result is " +result);




    }
}

