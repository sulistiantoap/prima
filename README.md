# prima

package no2;
import java.util.Scanner;

public class No2 {

   
    public static void main(String[] args) {
        int awal,akhir,hasil;
        Scanner in = new Scanner(System.in);
        System.out.print("Masukan angka awal : ");
        awal = in.nextInt();
        System.out.print("Masukan angka akhir : ");
        akhir = in.nextInt();
        System.out.println("Angka prima antara " + awal + " sampai " +akhir + " adalah : " );
        while (awal <= akhir){
            int tmp = 0;
            for (int bagi = 2; bagi < awal; bagi++){
                if (awal%bagi==0){
                    tmp=1;
                }
            }
            if (tmp != 1){
                System.out.print(awal + " ");
            }
            awal++;
        }
    }
    
}
