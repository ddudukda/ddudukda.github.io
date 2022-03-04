---
title:  "Q.10871(java)"
categories:
 - baekjoon(java)
tags:
 - if
 - for  
author_profile: true
sidebar:
    nav: "sidebar_main"  
---
#### if, for문

* * *
~~~java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.StringTokenizer;

public class Main {
    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StringTokenizer st = new StringTokenizer(br.readLine(), " "); //공백 기준으로 쪼개기
        int n = Integer.parseInt(st.nextToken());
        int x = Integer.parseInt(st.nextToken());
        StringBuilder sb = new StringBuilder(); //가공데이터 받기
        st = new StringTokenizer(br.readLine(), " "); 
        int arr[] = new int[n];
        for (int i = 0; i < n; i++) {
            int arrx = Integer.parseInt(st.nextToken()); 
            arr[i] = arrx;
            if(arrx < x){
                sb.append(arrx).append(" ");
            }
        }
        System.out.println(sb);
    }
}
~~~
*****

<details>
<summary>정리</summary>
- StringBuilder <br>
- .append
</details>