import java.util.Iterator;
import java.util.Stack;

public class arrangeStack {
	public static void arrangeStacky(Stack<Integer> original) {
	  Stack<Integer> even = new Stack<Integer>();
    Stack<Integer> odd = new Stack<Integer>();
    while (!original.empty()) {
        int n = original.pop();
        if (n % 2 == 0) {
            even.push(n);
        } else {
            odd.push(n);
        }
    }
    while (!odd.empty()) {
        original.push(odd.pop());
    }
    while (!even.empty()) {
        original.push(even.pop());
    }
    
    Iterator<Integer> iter = original.iterator(); //loop the Stack
    while (iter.hasNext()){
        System.out.println(iter.next());
    }
}

	public static void main(String[] args) { 
		Stack<Integer> original = new Stack<Integer>();
		original.push(11);
		original.push(12);
		original.push(21);
		original.push(22);
		arrangeStacky (original);
	}
}
