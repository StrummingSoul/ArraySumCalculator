# ArraySumCalculator
ArraySumCalc
public class ArraySumCalculator {
    public static void main(String[] args) {
        int[][] array = {
                {1, 2, 3},
                {4, 5, 6},
                {7, 8, 9}
        };

        int sum = calculateArraySum(array);
        System.out.println("Сумма элементов массива: " + sum);
    }

    public static int calculateArraySum(int[][] array) {
        int sum = 0;
        for (int[] row : array) {
            for (int element : row) {
                sum += element;
            }
        }
        return sum;
    }
}
