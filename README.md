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
        long a = 1;
        long b = 1;
        
        System.out.print(a + " " + b + " ");
        
        for(int i = 3; i <= 20; i++) {
            long next = a + b;
            System.out.print(next + " ");
            a = b;
            b = next;
        }
        System.out.println("\n");
    }
}<img width="605" height="327" alt="스크린샷 2026-09-07 152000" src="https://github.com/user-attachments/assets/dfab2b7a-9587-4977-bfca-2650067c8241" />

