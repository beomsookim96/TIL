---
layout: post
title: Sliding Window
description: Sliding Window
tags: algorithm java
minute: 1
---

#### Slding Window

시간복잡도를 신경써야할 때 사용하면 좋다.  

```java
import java.util.*;
public class Main {



    static void solution(int[] sell, int n, int m){

        Map<Integer,Integer> values = new HashMap<>();

        for (int i = 0; i < m; i++) {
            values.put(sell[i], values.getOrDefault(sell[i],0)+1);
        }
        int sum = values.size();
        System.out.print(sum + " ");

        for (int i = 1; i <= n-m; i++) {
            //왼쪽 끝의 것을 뺀다. 오른쪽 끝의 것을 더한다.
            int tmp = sell[i-1];
            values.put(tmp, values.getOrDefault(tmp,0)-1);
            if(values.get(tmp)==0){
                sum--;
            }
            values.put(sell[i+m-1], values.getOrDefault(sell[i+m-1],0)+1);
            if(values.get(sell[i+m-1])==1){
                sum++;
            }
            System.out.print(sum + " ");
        }

    } // solution

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int m = sc.nextInt();

        int[] sell = new int[n];
        for (int i = 0; i < n; i++) {
            sell[i] = sc.nextInt();
        }

        solution(sell,n,m);



    } // main()

} // end class
```