# 자바 11월 20일 변수와 배열 

## 1. 사용자에게 입력을 받고, 동일한 내용을 세번 출력하는 코드를 작성하시오. 

```java  
public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        String s1= scanner.nextLine();
        System.out.println(s1);
        System.out.println(s1);
        System.out.println(s1);
    }  
```

# Q2두개의 숫자를 입력받고, 순서를 바꿔서 출력하시오. 
```java  

public class Day1variable {
    //단축키 메인 탭 하면 만들어짐
    public static void main(String[] args) {
        //정수형 자료형
        int[] score;
        Scanner scanner = new Scanner(System.in);
        score =new int[2];
        score[0]=scanner.nextInt();
        score[1]=scanner.nextInt();
        System.out.println(score[1]);
        System.out.println(score[0]);


    }
}

```

# 를 출력하는 코드를 만들어 보시오.
```java 
public class Day1variable {
    //단축키 메인 탭 하면 만들어짐
    public static void main(String[] args) {
        //정수형 자료형
       System.out.println("   *   *   ");
       System.out.println("  *** ***  ");
       System.out.println(" ********* ");
       System.out.println(" ********* ");
       System.out.println("   *****   ");
       System.out.println("     *     ");



    }
}
```
## 시간과 오전 오후를 입력받고, 오전 XX시 의 형식으로 출력하는 코드를 작성하시오. 
```java 
import java.util.Scanner;

public class Day1variable {
    //단축키 메인 탭 하면 만들어짐
    public static void main(String[] args) {
        //정수형 자료형
       Scanner scanner =new Scanner(System.in);
       System.out.println("오전 오후를 입력하세요.");
       String amPm=scanner.nextLine();
       System.out.println("시간을 입력하세요 ");
       int hour=scanner.nextInt();
       String so=" %s %d시";
       System.out.println(String.format(so,amPm,hour));


    }
}


```

## ## 시간과 오전 오후를 입력받고, 오전 XX시 의 형식으로 출력하는 코드를 작성하시오. 
```java 
import java.util.Scanner;

public class Day1variable {
    //단축키 메인 탭 하면 만들어짐
    public static void main(String[] args) {
        //정수형 자료형
       Scanner scanner =new Scanner(System.in);
       System.out.println("오전 오후를 입력하세요.");
       String amPm=scanner.nextLine();
       System.out.println("시간을 입력하세요 ");
       int hour=scanner.nextInt();
       String so=" %s %d시";
       System.out.println(String.format(so,amPm,hour));


    }
}


```
## 사용자에게 3개의 0.0 ~ 4.5 사이의 실수를 입력받고그 뒤에 3개의 이름을 입력받은 뒤이름 - <이름>, 학점 - <실수>
의 형태로 3줄을 출력하는 프로그램을 작성하시오. 단, 실수의 범위가 틀려도 상관없다. 
```java 
import java.util.Scanner;

public class Day1variable {
    //단축키 메인 탭 하면 만들어짐
    public static void main(String[] args) {
        //정수형 자료
        double [] grade;
        grade =new double[3];
        System.out.println("학점 입력:");
       Scanner scanner =new Scanner(System.in);
       grade[0]=scanner.nextDouble();
       grade[1]=scanner.nextDouble();
       grade[2]=scanner.nextDouble();
       System.out.println("이름 입력:");
        scanner.nextLine();
        String [] name;
       name = new String[3];
       name[0]=scanner.nextLine();
       name[1]=scanner.nextLine();
       name[2]=scanner.nextLine();

       String formats="이름: %s 학점 : %.2f";

       System.out.println(String.format(formats,name[0],grade[0]));
       System.out.println(String.format(formats,name[1],grade[1]));
       System.out.println(String.format(formats,name[2],grade[2]));



    }
}



```



