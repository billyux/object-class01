# object-class01
### mondai 01
```java
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
```
<img width="629" height="509" alt="과제1 (2)" src="https://github.com/user-attachments/assets/66f34e74-3663-4b15-a900-aa79d8a676c0" />

### mondai 02
```java
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
}
```
<img width="605" height="327" alt="스크린샷 2026-09-07 152000" src="https://github.com/user-attachments/assets/dfab2b7a-9587-4977-bfca-2650067c8241" />

### mondai 03
```java
public class HelloWorld {
    public static void main(String[] args) {
    	
    	long prev = 1;
        long curr = 1;
        
        for(int i = 2; i <= 20; i++) {
            long next = prev + curr;
            double ratio = (double) next / curr;
            System.out.printf("%d/%d=%.3f  ", next, curr, ratio);
            if((i - 1) % 4 == 0) {
                System.out.println();
            }
            prev = curr;
            curr = next;
        }
        System.out.println("\n");
    }
}
```
<img width="612" height="358" alt="스크린샷 2026-09-07 152706" src="https://github.com/user-attachments/assets/57affec6-cd84-4892-8b38-86a2d8563c00" />

### mondai 04
```java
public class HelloWorld {
    public static void main(String[] args) {
    	for(int j = 1; j <= 9; j++) {
            for(int i = 1; i <= 9; i++) {
                System.out.print(i + "*" + j + "=" + (i * j) + "\t");
            }
            System.out.println();
        }
    }
}
```
<img width="634" height="176" alt="스크린샷 2026-09-07 152843" src="https://github.com/user-attachments/assets/d3acdcb5-c50f-4f34-afc1-77212d18a8e2" />

### mondai 05-1
```java
public class HelloWorld {
    public static void main(String[] args) {
      
        int i;
     double j=0;
        int h=0;
  
        double a=0;
      
        for(i=1; i<1000;i++) {
        
        	if(i%2==1){
                
                j=4.0/(h*2+1);
                h++;
               a+=j;
               
                    
            }
            
        	if(i%2==0){
                
              j=4.0/(h*2+1);
                h++;
              a-=j;
                
                    
            }
            
        }
        
            System.out.printf("%.4f",a);
            
             
        	
    }
}
```
<img width="1543" height="725" alt="스크린샷 2026-09-08 150033" src="https://github.com/user-attachments/assets/166225c0-c1cd-477c-ab76-4902f1c8475c" />

### mondai 05-2
```java
public class HelloWorld {
    public static void main(String[] args) {
      
        int i;
     double j=0;
        int h=0;
        double k=0;
        double a=0;
      
        for(i=0; i<1000;i++) {
        
        	if(i%2==0){
             k = Math.pow(3, i); 
                j=(1.0* Math.sqrt(12))/(k*(h*2+1));
                h++;
               a+=j;
               
                    
            }
            
        	if(i%2==1){
                 k = Math.pow(3, i); 
              j=(1.0* Math.sqrt(12))/(k*(h*2+1));
                h++;
              a-=j;
                
                    
            }
            
        }
        
            System.out.printf("%.4f",a);
            
             
        	
    }
}
```
<img width="1530" height="696" alt="스크린샷 2026-09-08 152721" src="https://github.com/user-attachments/assets/07088f93-4032-43df-9da9-10394d7342da" />

### mondai 06
```java
public class HelloWorld {
    public static void main(String[] args) {
        int n=6;
         
    for(int i=0; i<n;i++)
        {
            for( int j=0; j<n-i-1;j++){
            System.out.printf(" ");}
              int a =1;
            for(int k=0;k<=i;k++){
                System.out.printf("%-4d",a);
                    a=a*(i-k)/(k+1);
            }
                 System.out.println();
        }
    }
}
```
<img width="1305" height="592" alt="스크린샷 2026-09-08 160146" src="https://github.com/user-attachments/assets/905ebc52-b5bb-42c7-a371-390603caf260" />

### mondai 07
```java
public class Helloworld {
    public static void main(String[] args) {

        int[] data = new int[20];

       
        for (int i = 0; i < 20; i++) {
            data[i] = (int)(Math.random() * 100);
        }

      
        for (int a = 0; a < data.length - 1; a++) {

            
            int min = a;

          
            for (int b = a + 1; b < data.length; b++) {
                if (data[b] < data[min]) {
                    min = b;
                }
            }

          
            int temp = data[a];
            data[a] = data[min];
            data[min] = temp;
        }

    
        for (int i = 0; i < data.length; i++) {
            System.out.println(data[i]);
        }
    }
}
```
<img width="708" height="545" alt="image" src="https://github.com/user-attachments/assets/4426feff-16cf-455a-93e5-9e1c03cba208" />

### mondai 08
```java
public class helloworld {
    public static void main(String[] args) {

        int score[][] = new int[30][5];

        // 점수 생성
        for (int i = 0; i < 30; i++) {
            for (int j = 0; j < 4; j++) {
                score[i][j] = (int)(Math.random() * 101);
            }
        }

        // 총점 계산
        for (int i = 0; i < 30; i++) {
            score[i][4] = score[i][0]
                        + score[i][1]
                        + score[i][2]
                        + score[i][3];
        }

        // 출력
        System.out.println("번호\t국어\t영어\t수학\t과학\t총점");

        for (int i = 0; i < 30; i++) {
            System.out.printf("%d\t%d\t%d\t%d\t%d\t%d%n",
                    i + 1,
                    score[i][0],
                    score[i][1],
                    score[i][2],
                    score[i][3],
                    score[i][4]);
        }
    }
}
```
<img width="364" height="511" alt="image" src="https://github.com/user-attachments/assets/1df0e043-a329-4817-9716-ed8894db664c" />

### mondai 10
```java
public class Helloworld {
    public static void main(String[] args) {
        int arrayCount = 1000;
        int maxValue = 100;
        int binSize = 10;
        int displayScale = 5;
        if (args.length >= 4) {
            arrayCount = Integer.parseInt(args[0]);
            maxValue = Integer.parseInt(args[1]);
            binSize = Integer.parseInt(args[2]);
            displayScale = Integer.parseInt(args[3]);
        }

        int[] data = new int[arrayCount];

        for (int i = 0; i < arrayCount; i++) {
            data[i] = (int) (Math.random() * maxValue);
        }

        int binCount = (maxValue + binSize - 1) / binSize;
        int[] histogram = new int[binCount];

        for (int i = 0; i < arrayCount; i++) {
            int bin = data[i] / binSize;
            histogram[bin]++;
        }

        for (int i = 0; i < binCount; i++) {
            int start = i * binSize;
            int end = Math.min(start + binSize - 1, maxValue - 1);

            System.out.printf("%2d~%-2d\t", start, end);

            int count = histogram[i] / displayScale;

            for (int j = 0; j < count; j++) {
                System.out.print("#");
            }

            System.out.println();
        }
    }
}
```
<img width="375" height="311" alt="image" src="https://github.com/user-attachments/assets/8e406536-625d-42d7-b22f-d1c4955cfb63" />

### mondai 11
```java
public class HELLOWORLD {
public static void main(String[] args) {//문자열의 타입      
		int array_count;
		if(args.length !=1)
			return;
		array_count = Integer.parseInt(args[0]);//이걸 하는 이유는 기존 string[]args은 문자열 이름을 저장하는데 Integer.parseInt(args[0])은 정수형으로 전환 args[0에 인자값을 바탕으로 배열의 크기를 정한다는 뜻 
		int[] arr = new int[array_count];// 배열의 크기(인자값)을 바탕으로 새로운 배열 생성
		for (int i=0; i<array_count; i++) {
			arr[i] = (int) (Math.random()*100);
		}
		for (int i=0; i<array_count; i++) {
			System.out.print(arr[i] + " ");  
		}
		System.out.println();
		double sum = 0;
		for (int i=0; i<array_count; i++) {
			sum+=arr[i];
		}
		System.out.printf("arithematic mean : = %f\n", sum/array_count);
		double prod = 1;
		for (int i=0; i<array_count; i++) {
			prod*=arr[i];
		}
		System.out.printf("geometric mean : = %f\n", Math.pow(prod, 1.0/array_count));
    double six =1;
    for (int i=0; i<array_count; i++){
        six+=1.0/arr[i];//(double)1이나 1.0을 사용해야함 아니면 정수 나눗셈이 되어버림 0만출력
        
    }  System.out.printf("hamonoic mean : = %f\n", array_count/six );
    int[] sortedArr = arr.clone();
        java.util.Arrays.sort(sortedArr);
        double median;
        if (array_count % 2 == 0) {
            median = (sortedArr[array_count / 2 - 1] + sortedArr[array_count / 2]) / 2.0;
        } else {
            median = sortedArr[array_count / 2];
        }
        System.out.printf("median           : = %f\n", median);
		
	}
}
```
<img width="1566" height="327" alt="image" src="https://github.com/user-attachments/assets/1d1fa480-693d-4096-b6b0-de8007cc5a5b" />




