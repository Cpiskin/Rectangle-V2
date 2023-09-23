# Doing the rectangle class again with the informations we learned from Unit 1 and Unit 2

public class RectangleV2 {
    // Fields (Instance Variables)
    private int length;  // Uzunluk
    private int width;   // Genişlik

    // Constructor (Kurucu Metod)
    public RectangleV2(int length, int width) {
        this.length = length;
        this.width = width;
    }

    // Getter ve Setter Metodları
    public int getLength() {
        return length;
    }

    public void setLength(int length) {
        this.length = length;
    }

    public int getWidth() {
        return width;
    }

    public void setWidth(int width) {
        this.width = width;
    }

    // Alan Hesaplama Metodu
    public int calculateArea() {
        return length * width;
    }

    // Çevre Hesaplama Metodu
    public int calculatePerimeter() {
        return 2 * (length + width);
    }

    // Kare Kontrolü Metodu
    public boolean isSquare() {
        return length == width;
    }

    // Dikdörtgen Bilgilerini Yazdırma Metodu
    public void printInfo() {
        System.out.println("Uzunluk: " + length);
        System.out.println("Genişlik: " + width);
        System.out.println("Alan: " + calculateArea());
        System.out.println("Çevre: " + calculatePerimeter());
    }
}

