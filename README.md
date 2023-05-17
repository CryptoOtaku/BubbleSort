# BubbleSort
BubbleSort
public class BubbleSort {
    public static void main(String[] args) {
        int[] numbers = {5, 2, 8, 1, 9};
        
        // Сортировка пузырьком
        for (int i = 0; i < numbers.length - 1; i++) {
            for (int j = 0; j < numbers.length - i - 1; j++) {
                if (numbers[j] > numbers[j + 1]) {
                    // Обмен значениями
                    int temp = numbers[j];
                    numbers[j] = numbers[j + 1];
                    numbers[j + 1] = temp;
                }
            }
        }
        
        // Вывод отсортированного массива
        System.out.println("Отсортированный массив:");
        for (int number : numbers) {
            System.out.print(number + " ");
        }
    }
}
