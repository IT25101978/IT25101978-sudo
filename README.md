public class Calculator {

    public static int Add(int num1, int num2) {
        return num1 + num2;
    }

    public static int Multiply(int num1, int num2) {
        return num1 * num2;
    }

    public static int Square(int num) {
        return num * num;
    }

    public static void main(String[] args) {

        int Eq1 = Square(Add(Multiply(3, 4), Multiply(5, 7))); // (3*4 + 5*7)^2
        System.out.println(Eq1);

        int Eq2 = Add(Square(Add(4, 7)), Square(Add(8, 3))); // (4+7)^2 + (8+3)^2
        System.out.println(Eq2);
    }
}
