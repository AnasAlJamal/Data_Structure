public class Stack {


               

    public static void main(String[] args) {
        Stack stack = new Stack(5);
        stack.push(1);
        stack.push(2);
        stack.push(3);
        stack.print();
                      //System.out.println(stack.pop());
                      //System.out.println(stack.peek());
    }
    
    
    
    private int[] arr;
    private int top;
    private int capacity;

    // constructor to initialize stack
    public Stack(int size) {
        arr = new int[size];
        capacity = size;
        top = -1;
    }

    // push elements into the stack
    public void push(int x) {
        if (isFull()) {
            System.out.println("Stack Overflow");
            System.exit(1);
        }
        arr[++top] = x;
    }

    // pop elements from the stack
    public int pop() {
        if (isEmpty()) {
            System.out.println("Stack Underflow");
            System.exit(1);
        }
        return arr[top--];
    }

    // check if stack is full
    public boolean isFull() {
        return top == capacity - 1;
    }

    // check if stack is empty
    public boolean isEmpty() {
        return top == -1;
    }

    // return the top element of stack
    public int peek() {
        if (!isEmpty()) {
            return arr[top];
        } else {
            System.exit(1);
            return -1;
        }
    }

    void print (){
        System.out.println("[ ");
        for (int i = top ;  i >=0 ; i --){
            System.out.println(arr[i]);
        }
        System.out.println("]");
    }

}
