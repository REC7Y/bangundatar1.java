# bangundatar1.java

public class bangundatar{
  void HitungLuas() {
      System.out.println("Liska");
      System.out.println("192-052");
      System.out.println("Menghitung LuasSegitiga");
      
  }
}
class LuasSegitiga extends bangundatar{
   double alas,tinggi;
   public LuasSegitiga(){
       alas =2;
       tinggi =4;
 }
 public LuasSegitiga(double inputAlas){
       this.alas=inputAlas;
       tinggi =12;
 }
 public LuasSegitiga(double inputAlas,double inputTinggi){
       this.alas =inputAlas;
       this.tinggi =inputTinggi;
 }
 public double getAlas(){
       return alas;
 }
 public void setAlas(double inputAlas){
       this.alas =inputAlas;
 }
 public double getTinggi(){
       return tinggi;
 }
 public void setTinggi(double inputTinggi){
        this.tinggi =inputTinggi;
 }
 @Override
  void HitungLuas(){
        double luas;
        luas =0.5*this.alas*this.tinggi;
        System.out.println("Luas segitiga dengan alas:"+alas+"cm,tinggi:"+tinggi+"cm adalah "+luas+"cm kuadrat.");
       }
  }
    class BangunDatarTest{
      public static void main(String[]args){
      bangundatar bd =new bangundatar();
      bd.HitungLuas();
      LuasSegitiga s =new LuasSegitiga();
      s.HitungLuas();
      LuasSegitiga s1 =new LuasSegitiga(10);
      s1.HitungLuas();
      LuasSegitiga s2 = new LuasSegitiga(3,5);
      s2.HitungLuas();
   
  }
}
