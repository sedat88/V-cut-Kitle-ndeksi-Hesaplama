# V-cut-Kitle-ndeksi-Hesaplama
import java.util.Scanner;
public class Main {
    public static void main (String[]orgs) {

        // Vücut Kitle İndeksi Hesaplama
        // Formül : Kilo (kg) / Boy(m) * Boy(m)

        Scanner input = new Scanner(System.in);
        System.out.print("Lütfen boyunuzu (metre cinsinde) giriniz :");
        double boy = input.nextDouble();
        System.out.print("Lütfen kilonuzu giriniz : ");
        double kg = input.nextDouble();
        double vucutkitlendeksi = kg/(boy*boy);

        String sonuç="";
        if(vucutkitlendeksi<20){
            sonuç="Zayıf";
        }
        if(vucutkitlendeksi>25){
            sonuç="Fazla kilolu";
        }
        if(vucutkitlendeksi>=20 && vucutkitlendeksi<=25){
            sonuç="Normal";
            System.out.print("Vücut Kitle İndeksiniz: " + vucutkitlendeksi + " ("+sonuç+")");

        }



