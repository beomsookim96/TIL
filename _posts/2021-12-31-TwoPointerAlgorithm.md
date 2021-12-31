---
layout: post
title: Two Pointer Algorithm
description: Two Pointer Algorithm
tags: algorithm java
minute: 1
---
<br>

#### Two Pointer Algorithm

교집합을 구하는 문제에서 사용가능하다.
O(n^2) 을 O(n)으로 줄여야 할 때 유용!

```java
import java.util.*;
public class Main {

    static void solution(int[] arr1, int[] arr2){
        ArrayList<Integer> arrayList = new ArrayList<>();
        Arrays.sort(arr1);
        Arrays.sort(arr2);
        int p1=0, p2=0;
        while(p1<arr1.length && p2<arr2.length){
            if(arr1[p1]==arr2[p2]){
                arrayList.add(arr1[p1]);
                p1++;
                p2++;
            }
            else if(arr1[p1]<arr2[p2]){
                p1++;
            }else {
                p2++;
            }
        }

        arrayList.forEach(i -> {
            System.out.print(i+" ");
        });

    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt(); // 첫 번째 배열의 크기
        int[] arr1 = new int[n];
        for (int i = 0; i < n; i++) {
            arr1[i] = sc.nextInt();
        } // end for
        int m = sc.nextInt(); // 두 번째 배열의 크기
        int[] arr2 = new int[m];
        for (int i = 0; i < m; i++) {
            arr2[i] = sc.nextInt();
        } // end for

        solution(arr1,arr2);
    } // main()

} // end class

```