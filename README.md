package pl.grzesiu.testing;

import java.util.Scanner;

public class TempChk {

    private int temp;

    public int getTemp() {
        return temp;
    }

    public void setTemp(int t) {
        this.temp = t;
    }

    public boolean check()
    {
        return temp > 0;
    }

    public static void main(String[] args) {
        System.out.println("Podaj aktualną temperaturę: ");
        Scanner input = new Scanner(System.in);
        int t = input.nextInt();
        TempChk tpCh = new TempChk();
        tpCh.setTemp(t);
        if (tpCh.check()) {
            System.out.println("Temperatura jest dodatnia");
        }
        else {
            System.out.println("Brrr...");
        }
    }
}
