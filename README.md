# first-Assessment-
Assignment 

class Binary {

public static int binarySearch(int a[], int start, int end, int x) {

if(start <= end) {

int middle = (start+end)/2;

if(a[middle] == x) {

return middle;

} if(a[middle] > x) {

return binarySearch(a, start, middle-1, x);

} if(a[middle] < x) {

return binarySearch(a, middle+1, end, x);

}

}

return -1; // not found

} public static void main(String[] args) {

int a[] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

int indexResult = binarySearch(a, 0, 9, 7); System.out.println(indexResult);

}

}

Linear Search in Java

public class LinearSearch{

public static int sequentialSearch(int[] arr, int key){

for(int i=0;i<arr.length;i++){ 

if(arr[i] == key){ 

return i; 

}

}return -1;

}

 }public static void main(String a[]){

int[] a1= {10,20,30,50,70,90};

int key = 50;

 System.out.println(key+" is found at index: "+linearSearch(a1, key));

}

}    
