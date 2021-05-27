---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

###01. 3개의 터널 통과

![tunnel](/assets/images/im1.jpg)
~~~c
#include <stdio.h>
int main() {
 int a,b,c;
 printf("세 터널의 높이를 차례대로 입력하세요 : ");
 scanf("%d%d%d",&a,&b,&c);
 if(a <= 170)
 {
   printf("충돌, %d",a);
 }
 else if(b<=170)
 {
   printf("충돌, %d",b);
 }
 else if(c<=170)
 {
   printf("충돌, %d",c);
 }
 else printf("무사통과");
 return 0;
}
~~~


