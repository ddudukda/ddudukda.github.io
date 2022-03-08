---
title:  "Q.15596(java)"
categories:
 - baekjoon
tags:
 - funtion  
author_profile: true
sidebar:
    nav: "sidebar_main"  
---
#### 함수

* * *
~~~java
class Test {
     long sum(int[] a){
        long sum = 0;
        for(int i=0; i<a.length; i++){
            sum += a[i];
        }
        return sum;
    }
}
~~~
*****