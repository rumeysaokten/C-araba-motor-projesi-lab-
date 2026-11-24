# C-araba-motor-projesi-lab-
using System;

class Motor
{
    public string Model;
    public int BeygirGücü;
    public Motor(string model, int beygirGücü)
    {
        Model = model;
        BeygirGücü = beygirGücü;
    }
    public void Calistir()
    {
        Console.WriteLine($"{Model} calistiriliyor.");
    }
}

class Araba
{
    public string Marka;
    public Motor motor;
    public Araba(string marka, string _motor, int beygirGücü)
    {
        Marka = marka;
        motor = new Motor(_motor, beygirGücü);

    }
    public void BilgileriGöster()
    {
        Console.WriteLine($"{Marka} ");
        Console.WriteLine($"{ motor}");
    }

    
}
class Program4
{
    static void Main()
    {
        Araba araba = new  Araba("Opel","motor",2000);
        araba.BilgileriGöster();
        

    }
}
