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

public class item {
    private String name;
    private double price;
    private String unit;
    
    // Default constructor
    public item() {
        name = "Apple";
        price = 30.0;
        unit = "pc";
    }
    
    // Constructor with parameters
    public item(String name, double price, String unit) {
        this.name = name;
        this.price = price;
        this.unit = unit;
    }
    
    // Encapsulated methods
    public String getName() {
        return name;
    }
    
    public void setName(String name) {
        this.name = name;
    }
    
    public double getPrice() {
        return price;
    }
    
    public void setPrice(double price) {
        this.price = price;
    }
    
    public String getUnit() {
        return unit;
    }
    
    public void setUnit(String unit) {
        this.unit = unit;
    }
    
    // TotalPrice method
    public double TotalPrice(double qty) {
        return qty * price;
    }
    
    // DisplayItem method
    public String DisplayItem() {
        return name + " for " + price + " per " + unit;
    }}
