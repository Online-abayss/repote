# repote
##항해99 알고리즘 언어과제
```
1. 다음 코드를 실행하면 출력 결과로 5를 기대했는데 4가 출력되었습니다. 어디에서 잘못 작성된 것일까요?
```
```
int var1=5;
int var2=2;
double var3=var1/var2; -> var1,var2는 int인 정수형으로 받아서 쓰고 있기에, 결과값이 실수가 나오면 정수형값까지만 갖고, 나머지는 짤린다.
int var4=(int)(var3*var2);  ㄴ 그러므로 9번째 줄 코드를 double var3 = (double)var1/var2 로 바꿔야한다.
System.out.println(var4)
```
```
2. 다음 코드를 실행했을 때 출력 결과는 무엇입니까? (증감연산자에 대해 알아보세요!)
```
```
int x=10;
int y=20;
int z = (++x) + (y--); -> ++@ , --@ 는 +1이나 -1을 처리한 @값을 나타내며, 
System.out.println(z);    @++ , @--는 일단 원래값으로 계산하고 계산 끝나면 y를 +,-를 처리한다.
```
#### 그러므로 위 코드의 출력 결과는 11+20으로 31

```
3. while문과 Math.random() 메소드를 이용해서 2개의 주사위를 던졌을 때 나오는 눈을 (눈1, 눈2) 형태로 출력하고,
눈의 합이 5가 아니면 계속 주사위를 던지고, 눈의 합이 5이면 실행을 멈추는 코드를 작성해보세요. 
눈의 합이 5가 되는 조합은 
(1,4) 
(4,1) 
(2,3) 
(3,2)입니다.
```
```
public class test3 {
  public static void main(String[] args){
  int a = 0;
  int b = 0;
  
  System.out.println("시작!");
  
  while(a+b != 5){
  a = (int)(Math.random()*) +1;
  b = (int)(Math.random()*) +1;
  }
  System.out.println("("+a+","+b+")");
  System.out.println("끝!");
  }
}
```


