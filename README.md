package sample;

public class Sample;
  public static void reverse(String[] array){
    if(array==null || array.length < 2) {
      return;
    }
    for(int i=0; i<array.length/2; i++){
      String temp = array[i];
      array[i]=array[array.length-1-i];
      array[array.length-1-i] = temp;
    }
}
  public static void main(String[] args){
    String[] cities = {"Dallas", "San Francisco", "Houston", "New York"}
    System.out.println("Original array : " + Arrays.toString(cities));
    reverse(cities);
    System.out.println("Reversed array : " + Arrays.toString(cities));
