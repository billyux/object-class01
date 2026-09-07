# object-class01
public class HelloWorld {
    public static void main(String[] args) {
      
        for(int i = 0; i < 10; i++) {
            for(int j = 0; j <= i; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
        
        System.out.println();
        
    for(int i = 0; i < 10; i++) {
            for(int j = 0; j < 10 - i; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
        
        System.out.println();
     
        
        for(int i = 0; i < 10; i++) {
            for(int j = 0; j < 9 - i; j++) {
                System.out.print(" ");
            }
            for(int j = 0; j <= i; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
        
        System.out.println();
        
       
        for(int i = 0; i < 10; i++) {
            for(int j = 0; j < i; j++) {
                System.out.print(" ");
            }
            for(int j = 0; j < 10 - i; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
    }
}
<img width="629" height="509" alt="과제1 (2)" src="https://github.com/user-attachments/assets/66f34e74-3663-4b15-a900-aa79d8a676c0" />

#object-class02
public class HelloWorld {
    public static void main(String[] args) {
      
    	long[] fib = new long[20];
        fib[0] = 1;
        fib[1] = 1;
        for (int i = 2; i < 20; i++) {
            fib[i] = fib[i - 1] + fib[i - 2];
        }

    
        for (int i = 0; i < 20; i++) {
            System.out.print(fib[i] + " ");
        }
        System.out.println("\n");
    }
}<img width="605" height="327" alt="스크린샷 2026-09-07 152000" src="https://github.com/user-attachments/assets/dfab2b7a-9587-4977-bfca-2650067c8241" />

