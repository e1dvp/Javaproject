import java.util.Arrays;
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        int [] arr=new int[5];
        for(int i=0;i< arr.length;i++){
            arr[i]=10+(int)(Math.random()*10);

        }
        Arrays.sort(arr);
        for(int i=0;i<arr.length;i++){
            System.out.print(arr[i]+" ");
        }
        System.out.println();
        int[] arr_reverse=reverse(arr);
        for(int i=0;i<arr_reverse.length;i++){
            System.out.print(arr_reverse[i]+" ");
        }
    }
    static int[] reverse(int[] array){
        int[] array2=new int[array.length];
        for(int i=0,j=array2.length-1;i<array.length;i++,j--){
            array2[i]=array[j];
        }
        return array2;
    }
}
