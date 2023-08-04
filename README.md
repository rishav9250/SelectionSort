# SelectionSort
here is a code of SelectionSort in java.

import java.util.*;
public class SortingSelectionSort {
    public static void SelectionSort(int array[]){
        for(int i=0;i<array.length-1;i++){
            int currentPosition =i;
            for(int j=i+1;j<array.length;j++){
                if(array[currentPosition] > array[j]){
                    currentPosition = j;
                }
            }
        int temp =array[currentPosition];
        array[currentPosition] =array[i];
        array[i] = temp;
        }
    }
public static void main(String[] args) {
    int array[] ={5,4,1,2,3};
    SelectionSort(array);
}
}

