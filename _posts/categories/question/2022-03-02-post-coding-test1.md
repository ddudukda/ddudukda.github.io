---
title:  "Q.2480(java)"
categories:
 - question
tags:
 - baekjoon
 - java  
author_profile: true
sidebar:
    nav: "sidebar_main"  
---
#### if문

* * *
~~~java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.StringTokenizer;

public class Main {
    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        StringTokenizer st = new StringTokenizer(br.readLine());
        int data1 = Integer.parseInt(st.nextToken());
        int data2 = Integer.parseInt(st.nextToken());
        int data3 = Integer.parseInt(st.nextToken());
        //모두 같음
        if (data1 == data2 && data2 == data3) {
            System.out.print(10000 + (data1 * 1000));
        }
        //두개씩 같음 
        else if (data1 == data2 || data1 == data3) {
            System.out.print(1000 + (data1 * 100));
        } 
        else if (data2 == data3) {
            System.out.print(1000 + (data2 * 100));
        }
        //모두 다를 때, 최대값 이용 
        else {
            
            int maxdata = Math.max(Math.max(data1, data2), data3);
            System.out.print(maxdata * 100);
        }
    }

}
~~~
*****
<details>
<summary>정리</summary>
> BufferedReader 문자열, Integer.parseInt 형변환<br>
> StringTokenizer <br>
> Math.max(a,b) 최대값 뽑기
</details>
