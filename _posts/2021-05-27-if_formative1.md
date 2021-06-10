---
layout: single
title: 조건문
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

### 01. 3개의 터널 통과

![im1](/assets/images/im1.jpg)
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

### 02. 사주보기

![im2](/assets/images/.jpg)
~~~c
#include <stdio.h>
 int main(void)
 {int year, month, day, res;
  printf("당신의 사주를 봐드립니다.\n");
  printf("연도, 월, 일을 차례대로 입력하세요: ");
  scanf("%d %d %d", &year, &month, &day);
  res = year - month +day;
  if(res%10==0)
  printf("당신의 사주는 대박입니다.\n");
  else
  printf("당신의 사주는 그럭저럭입니다.\n");
  return 0;
  }
  ~~~
  
  ### 03. 이 달은 며칠까지 있을까?
  
  ![im3](/assets/images/이 달 며칠.jpg)
  ~~~c
  #include <stdio.h>
int main(void) 
 {int a, b;
  printf("연도와 월을 입력하세요: ");
  scanf("%d%d", &a, &b);
  printf("%d년 %d월의 마지막 날은", a, b);
  if(b==1||b==3||b==5||b==7||b==8||b==10||b==12)
   printf("31일");
  else if(b==4||b==6||b==9||b==11)
   printf("30일");
  else
    if((a%4==0 && !(a%100==0)) || a%400==0)
     printf("29일");
    else
     printf("28일");
  
  return 0;
}
~~~

### 04. 30분 전

![im4](/assets/images/30.jpg)
~~~c
#include <stdio.h>
 
int main(void) {
 int hour, min;
 printf("시간과 분을 입력하세요: ");
 scanf("%d%d", &hour, &min);
 printf("입력한 시간의 30분 전의 시간은 ");
 if(min>=30)
  printf("%d시%d분", hour, min-30);
 else
 {
   if(hour==00)
    printf("%d시%d분", 23, min+30);
   else
    printf("%d시%d분", hour-1, min+30);
 }
 return 0;
}
~~~
