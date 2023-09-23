# Doing the rectangle class again with the informations we learned from Unit 1 and Unit 2

public class RectangleV2 {

    // Attributes
    private double length;
    private double width;
    private double angle;
    private int sides;
    private String name;

    // Constructors
    public RectangleV2() {
        this.name = "RectangleV2";
    }

    public RectangleV2(double length, double width) {
        this.length = length;
        this.width = width;
        this.name = "RectangleV2";
    }

    // Getters
    public double getLength() {
        return length;
    }

    public double getWidth() {
        return width;
    }

    public String getName() {
        return name;
    }

    // Setters
    public void setLength(double length) {
        this.length = length;
    }

    public void setWidth(double width) {
        this.width = width;
    }

    // Other Methods

    @Override
    public String toString() {
        return "RectangleV2 [length=" + length + ", width=" + width + ", angle=" + angle + ", sides=" + sides + ", name="
                + name + "]";
    }

    public boolean equals(RectangleV2 otherRectangle) {
        return this.length == otherRectangle.length && this.width == otherRectangle.width;
    }

    public double getArea() {
        return length * width;
    }

    public double getPerimeter() {
        return 2 * (length + width);
    }
}
