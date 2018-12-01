# Loop-Arraylist


import java.util.ArrayList;
import java.util.Iterator;


public class Loops1 {
    public static void main(String[] args) {
        
        ArrayList<Integer> obj = new ArrayList<Integer>();
        obj.add(10);
        obj.add(7);
        obj.add(39);
        obj.add(40);
        System.out.println(obj);
        System.out.println("For Loop: ");
        for(int counter = 0; counter < obj.size(); counter++) {
            System.out.println(obj.get(counter));
            
        }
        System.out.println("Advanced for loop");
        for(Integer num: obj) {
            System.out.println(num);
            
        }
        System.out.println("While loop:");
        int count = 0;
        while(obj.size() > count) {
            System.out.println(obj.get(count));
            count++;
        }
        System.out.println("Iterator");
        Iterator Iter = obj.iterator();
        while(Iter.hasNext()) {
            System.out.println(Iter.next());
        }
    }
}
