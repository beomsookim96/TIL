---
layout: post
title: Find Prime Number
description: FindPrimeNumber algorithm
tags: algorithm java
minute: 1
---
<br>

#### 에라토스 테네스의 체  
```java
import java.util.*;

public class Main {

    static void solution(int n){
        int[] era = new int[n+1];
        int count = 0;
        for (int i = 2; i <= n; i++) {
            if(era[i] == 0){
                count++;
                era[i] = 1;
                for (int j = i; j <= n; j=j+i) {
                        era[j] = 1;
                }
            }
        }

        System.out.println(count);
    }

    public static void main(String[] args){

        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.next());
        solution(n);

    }

}
```
소수를 찾는 방법 중 그나마 빠른 방법이라고 한다.  
이중for문을 돌기때문에 효율성에 신경써야한다.
