
# <font color = #04499> 02. 변수 (Variable) </font>

+ 변수(Variable) : 메모리상에 값을 저장할 수 있는 공간
    ```
    가독성이 좋아짐
    재사용성 증가로 인한
    코드량 감소
    유지보수 용이
    ```

+ 변수의 선언 : 메모리 공간에 데이터를 저장할 수 있는 공간을 할당하는 것

    ||||
    |------|---|---|
    |자료형|변수명 ;|
    |변수타입지정|변수명지정

   
# 자료형

- 자료형 종류
- 1.논리형(boolean)
- 2.문자형
-   문자(char)
-   문자열(String) ---- 참조형 자료형 (클래스)

(모든 클래스는 자료형이 될 수가 있다.)



```java
package com.kh.first;
// 한 줄 주석 (// 뒤부터 )
/* 여러줄 주석	
   안녕하세요
 */
public class TestClass{
	public static void main(String[] args){
		System.out.println("Hellow World"); // 출력하는 문장
	/*
		boolean 1byte 
		char    2byte
		String  참조형
		byte    1byte
		short   2byte
		int     4byte
		long	8byte
		float	4byte
		double	8byte
		*/	
	}
}
```
