# JAVASCRIPT_VILLARAIZZ

public static void main(String[] args) {
          item item1 = new item();
        item item2 = new item("Orange", 25.0, "pc");
        item item3 = new item("Banana", 50.0, "kg");
        
        System.out.println(item1.DisplayItem());
        System.out.println("Qty: 20 - Total: " + item1.TotalPrice(20));
        System.out.println();
        
        System.out.println(item2.DisplayItem());
        System.out.println("Qty: 4 - Total: " + item2.TotalPrice(4));
        System.out.println();
        
        System.out.println(item3.DisplayItem());
        System.out.println("Qty: 2.5 - Total: " + item3.TotalPrice(2.5));
        System.out.println();
    }
}


