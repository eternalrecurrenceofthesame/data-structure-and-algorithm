## 알고리즘이란?

문제를 해결하기 위한 절차로, 명확하게 정의되고 순서가 있는 유한 개의 규칙으로 이루어진 집합

## 세 값의 최댓값 구하기
```
static int max3(int a, int b, int c){ // 매개변수(가인수)
  int max = a; // 초기화
  if(b > max)
    max = b; // 대입
  if(c > max)
    max = c;

return max;
}

System.out.println("max3(3,2,1) = " + max3(3,2,1)); // 매개변숫값(실인수)
System.out.println("max3(3,2,1) = " + max3(3,2,2));
System.out.println("max3(3,2,1) = " + max3(3,4,1));
...

```

문장이 순차적으로 실행되는 구조 = 순차 구조

조건을 평가한 결과에 따라 실행 흐름이 변경되는 if 문 = 선택 구조

#### + 세 값의 중앙값 구하기
```
static int med3(int a, int b, int c){
if(a >= b)
  if(b >= c)
    return b;
  
  else if(a <= c)
    return a;
  else   
    return c;
    
  else if(a > c)
    return a;
  
  else if(b > c)
    return c;
  
  else
    return b;
}
```
