# test
public class main {
   public static void main(String[] args) {
       Scanner kb = new Scanner(System.in); //ตัวอ่านข้อมูล
       double price,total,sale; //กำหนดตัวแปร price = ราคาสินค้า , total = ราคารวมหลังส่วนลด , sale = ส่วนลด
       System.out.println("=== Program discount price ==="); //แสดงข้อความ === Program discount price ===
       System.out.print("Input price : "); //แสดงข้อความ Input price เพื่อกรอก
       price = kb.nextDouble(); //ตัวร้อนค่าจากคีย์บอร์ด
       System.out.println("=== Calculate total price ==="); //แสดงข้อความ === Calculate total price ===
       if (price >= 1 && price < 500) { // ถ้าราคาสินค้าอยู่ในช่วง 1-500 ลูกค้าจะได้ sale 0
           total = 0; //กำหนด total = 0
           System.out.println("Total price : " + (int)price); //แสดงค่าสินค้า
       } else if (price > 501 && price < 1000) { //ถ้าราคาสินค้าอยู่ในช่วง 501-1000 ลูกค้าจะได้ sale 3
           sale = 0.03; //กำหนดให้ส่วนลด sale เท่ากับ 1% หรือ 0.03
           total = price - (price * sale); //สูตรการคำนวณ
           System.out.println("Total price : " + (int)total); //แสดงค่าสินค้า
       } else if (price > 1001 && price < 2000) { //ถ้าราคาสินค้าอยู่ในช่วง 1001-2000 ลูกค้าจะได้ sale 4
           sale = 0.04; //กำหนดให้ส่วนลด sale เท่ากับ 4% หรือ 0.04
           total = price - (price * sale); //สูตรการคำนวณ
           System.out.println("Total price : " + (int)total); //แสดงค่าสินค้า
       } else if (price > 2001 && price < 5000) { //ถ้าราคาสินค้าอยู่ในช่วง 2001-5000 ลูกค้าจะได้ sale 7
           sale = 0.07; //กำหนดให้ส่วนลด sale เท่ากับ 7% หรือ 0.07
           total = price - (price * sale); //สูตรการคำนวณ
           System.out.println("Total price : " + (int) total); //แสดงค่าสินค้า
       } else if (price > 5001 ) { //ถ้าราคาสินค้ามากกว่า 5001 ลูกค้าจะได้ sale 10
           sale = 0.1; //กำหนดให้ส่วนลด sale เท่ากับ 1% หรือ 0.1
           total = price - (price * sale); //สูตรการคำนวณ
           System.out.println("Total price : " + (int)total); //แสดงค่าสินค้า
       }
   }
}
