# SSUETDSAlab4

/*
Task 1
public class lab4MuhammadTalha {
    public static void main(String[] args) {
        double[] ArrTalha = {1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8};

        double sum = calculateSum(ArrTalha);
        double mean = calculateMean(ArrTalha);

        System.out.println("Array according to Muhammad Talha Named ArrTalha: " 
                + java.util.Arrays.toString(ArrTalha));
        System.out.println("Sum of ArrTalha: " + sum);
        System.out.println("Mean of ArrTalha: " + mean);
    }

    public static double calculateSum(double[] array) {
        double sum = 0;
        for (double num : array) {
            sum += num;
        }
        return sum;
    }

    public static double calculateMean(double[] array) {
        return calculateSum(array) / array.length;
    }
}

*/
/*
Task 2
import java.util.Arrays;
public class lab4MuhammadTalha {
    public static void main(String[] args) {
        double[] talhaArray = {10.1, 20.2, 30.3, 40.4, 50.5, 60.6, 70.7};
        double talhaKey = 40.4;
        
        System.out.println("Original Array: " + Arrays.toString(talhaArray));

        double[][] result = splitArray(talhaArray, talhaKey);

        System.out.println("First Part of Talha Array: " + Arrays.toString(result[0]));
        System.out.println("Second Part of Talha Array: " + Arrays.toString(result[1]));
    }

    public static double[][] splitArray(double[] array, double key) {
        int index = -1;

        for (int i = 0; i < array.length; i++) {
            if (array[i] == key) {
                index = i;
                break;
            }
        }
        
        if (index == -1) {
            return new double[][]{array, new double[0]};
        }
        
        double[] TalhaArr1 = Arrays.copyOfRange(array, 0, index + 1);
        double[] TalhaArr2 = Arrays.copyOfRange(array, index + 1, array.length);

        return new double[][]{TalhaArr1, TalhaArr2};
    }
}
*/
/*Task 4
public class lab4MuhammadTalha {
    public static int findMissingNumberinArrayofTalha(int[] ArrTalha) {
        int n = ArrTalha.length;
        int expectedSum = n * (n + 1) / 2; 
        int actualSum = 0;
        
        for (int num : ArrTalha) {
            actualSum += num; 
        }
        
        return expectedSum - actualSum; 
    }

    public static void main(String[] args) {
        int[] ArrTalha = {0 , 2 , 3 , 4 , 5};
        System.out.println("Missing number from ArrTalha: " + findMissingNumberinArrayofTalha(ArrTalha));
    }
}
*/
/*
import java.util.Arrays;
public class lab4MuhammadTalha {
    public static void zigzagSortTalha(int[] arrTalha) {
        for (int i = 0; i < arrTalha.length - 1; i++) {
            if (i % 2 == 0) {
                if (arrTalha[i] > arrTalha[i + 1]) {
                    swapTalha(arrTalha, i, i + 1);
                }
            } 
            else {
                if (arrTalha[i] < arrTalha[i + 1]) {
                    swapTalha(arrTalha, i, i + 1);
                }
            }
        }
    }

    private static void swapTalha(int[] arrTalha, int iTalha, int jTalha) {
        int tempTalha = arrTalha[iTalha];
        arrTalha[iTalha] = arrTalha[jTalha];
        arrTalha[jTalha] = tempTalha;
    }

    public static void main(String[] args) {
        int[] arrTalha = {4, 3, 7, 5, 8, 6, 2, 1};
        zigzagSortTalha(arrTalha);
        System.out.println("Talha's zigzag sorted array: " + Arrays.toString(arrTalha));
    }
}
/*

/* *--------------------------------------------------------------* */

import java.util.*;

public class lab4MuhammadTalha {
    public static int[] mergeAndRemoveDuplicates(int[] arrTalha1, int[] arrTalha2) {
        Set<Integer> setTalha = new HashSet<>(); 
        
        for (int num : arrTalha1) setTalha.add(num);
        for (int num : arrTalha2) setTalha.add(num);
        
        int[] resultTalha = new int[setTalha.size()];
        int i = 0;
        for (int num : setTalha) resultTalha[i++] = num;

        return resultTalha;
    }

    public static void main(String[] args) {
        int[] arrayTalha1 = {1, 2, 3, 4};
        int[] arrayTalha2 = {3, 4, 5, 6};

        int[] mergedArrayTalha = mergeAndRemoveDuplicates(arrayTalha1, arrayTalha2);
        System.out.println("Talha's merged array with no duplicates: " + Arrays.toString(mergedArrayTalha));
    }
}



/*
Task # 4

public class lab4MuhammadTalha {
    public static void main(String[] args) {
        int[] ArrTalha = {1, 2, 3, 4, 5, 6};
        countEvenOdd(ArrTalha);
    }

    public static void countEvenOdd(int[] ArrTalha) {
        int even = 0;
        int odd = 0;

        for (int num : ArrTalha) {
            if (num % 2 == 0) {
                even++;
            } else {
                odd++;
            }
        }

        System.out.println("Even numbers in Talha's array: " + even);
        System.out.println("Odd numbers in Talha's array: " + odd);
    }
}
*/



/*
//Task # 3
public class lab4MuhammadTalha {
    public static void main(String[] args) {
        String[] words = {"Talha", "civic", "ssuet", "level"};

        for (String word : words) {
            if (isPalindrome(word)) {
                System.out.println("Muhammad Talha "+ word + " is a palindrome.");
            } else {
                System.out.println("Muhammad Talha " + word + " is not a palindrome.");
            }
        }
    }

    public static boolean isPalindrome(String str) {
        int left = 0;
        int right = str.length() - 1;

        while (left < right) {
            if (str.charAt(left) != str.charAt(right)) {
                return false;
            }
            left++;
            right--;
        }

        return true;
    }
}
*/



/*
Task 2
public class lab4MuhammadTalha {
    public static int[] MergeArr(int[] ArrTalha1, int[] ArrTalha2) {
        int[] mergedArray = new int[ArrTalha1.length + ArrTalha2.length];

        for (int i = 0; i < ArrTalha1.length; i++) {
            mergedArray[i] = ArrTalha1[i];
        }
        for (int i = 0; i < ArrTalha2.length; i++) {
            mergedArray[ArrTalha1.length + i] = ArrTalha2[i];
        }

        return mergedArray;
    }

    public static void main(String[] args) {
        int[] ArrTalha1 = {1, 2, 3, 4};
        int[] ArrTalha2 = {5, 6, 7, 8};

        int[] mergedArray = MergeArr(ArrTalha1, ArrTalha2);

        System.out.println("Merged Array a/c to Talha: " + java.util.Arrays.toString(mergedArray));
    }
}




/*
//Task # 1
public class lab4MuhammadTalha {
    public static void main(String[] args) {
        int[] ArrTalha1 = {1, 2, 3, 4};
        int[] ArrTalha2 = {5, 6, 7, 8};

        System.out.println("Before Swap:");
        System.out.println("Array 1 according to Talha: " + java.util.Arrays.toString(ArrTalha1));
        System.out.println("Array 2 according to Talha: " + java.util.Arrays.toString(ArrTalha2));

        for (int i = 0; i < ArrTalha1.length; i++) {
            int MyArr3 = ArrTalha1[i];
            ArrTalha1[i] = ArrTalha2[i];
            ArrTalha2[i] = MyArr3;
        }

        System.out.println("After Swap:");
        System.out.println("Array 1 according to Talha: " + java.util.Arrays.toString(ArrTalha1));
        System.out.println("Array 2 according to Talha: " + java.util.Arrays.toString(ArrTalha2));
    }
}

*/
