# aditAok
package latihan;

import java.util.Scanner;
public class KonversiBilangan {

    public static void main(String[] args) {
        Scanner inp = new Scanner(System.in);
        System.out.println("Pilih bilangan : \n1. Desimal\n2. Biner\n3. Hekxadesimal");
        System.out.print("Pilih menu tersebut (1/2/3): ");
        int menu = inp.nextInt();
        System.out.println("Menu yang dipilih : "+menu);
        
        switch (menu){
            case 1:
                System.out.println("Pilih konversi bilangan : ");
                System.out.println("1.Desimal ke biner");
                System.out.println("2.Desimal ke heksadesimal");
                System.out.print("Pilih menu tersebut (1 atau 2)");
                int masuk = inp.nextInt();
                System.out.println("Menu yang dipilih : "+masuk);
                
                if (masuk == 1){
                    System.out.print("Silakan Masukan bilangan desimal : ");
                    int angkadesimal = inp.nextInt();
                    String binerd;
                    binerd = Integer.toBinaryString(angkadesimal);
                    System.out.println("Bilangan biner = "+binerd+" "); 
                }
                if (masuk == 2){
                    System.out.print("Masukan bilangan desimal : ");
                    int angkad2 = inp.nextInt();
                    String heksad;
                    heksad = Integer.toHexString(angkad2);
                    System.out.println("Bilangan heksadesimalnya adalah : "+heksad);
                } 
                break;
                
            case 2:
                System.out.println("Pilih : ");
                System.out.println("1.Biner ke desimal");
                System.out.println("2.Biner ke heksadesimal");
                System.out.print("Pilih menu tersebut (1/2): ");
                int pilihanb = inp.nextInt();
                System.out.println("Menu yang dipilih : "+pilihanb);
                
                if (pilihanb == 1){ 
                    System.out.print("Silakan Masukan bilangan biner : ");
                    String angkab = inp.next();
                    int desimal = Integer.parseInt(angkab,2);
                    System.out.println("Bilangan desimalnya adalah = "+desimal);
                }
                if (pilihanb == 2){
                    System.out.print("Silakan Masukan bilangan biner : ");
                    int angkab2 = inp.nextInt();
                    String heksab = Integer.toHexString(angkab2);
                    System.out.println("Bilangan heksadesimalnya adalah = "+heksab);
                }
                break;
                
            case 3:    
                System.out.println("Pilih : ");
                System.out.println("1. Heksadesimal ke desimal");
                System.out.println("2. Heksadesimal ke biner");
                System.out.print("Pilih menu tersebut (1 atau 2): ");
                int pilihan = inp.nextInt();
                System.out.println("Menu yang dipilih : "+pilihan);
                
                if (pilihan == 1){
                    System.out.print("Silahkan Masukan bilangan heksadesimal : ");
                    String angkac = inp.next();
                    int desimalh = Integer.parseInt(angkac,16);
                    System.out.println("Bilangan desimal adalah = "+desimalh+" ");
                }
                if (pilihan == 2){
                    System.out.print("Silahkan masukan bilangan heksadesimal : ");
                    String angkac = inp.next();
                    long heksa2 = Long.parseLong(angkac,16);
                    String binerh = Long.toBinaryString(heksa2);
                    System.out.println("Bilangan binernya adalah = "+binerh); 
                }
                break;
        }   
    }
    
}
    

    

