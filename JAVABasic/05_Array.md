# <font color = #04499> 배열 ( Control ) </font>

같은 자료형의 변수를 하나의 묶음으로 다루는 것

변수 -> 한개의 데이터를 저장.

변수를 묶음으로 관리하자. => 배열.
(같은 자료형의 변수를 하나로 묶음)
저장된 값마다 인덱스 번호가 0부터 시작하여 설정.

한계: 같은 자료형만 묶을 수 있기에
다른 자료형을 묶고 싶을때 => 클래스, 컬렉션

Zero Base Index 기반.

arr[0] arr[1] arr[2] arr[3] arr[4]


배열 선언. => 
Stack 이라는 메모리 공간에 만들어진다.

자료형[] 배열명;
--> Stack이라는 공간에
arr 이라는 이름으로 하나만 생긴다.
실제로 값이 들어가는 공간이 아니라.

자료형 배열명[];

배열 할당.
자료형[] 배열명 = new 자료형[배열크기];
얼만큼의 공간을 만들건지에 대해 배열크기가 들어간다.

자료형 배열명[] = new 자료형[배열크기];


new => 힙 영역에 공간을 생성하는 키워드

int[] arr = new int[3];
int arr[] = new int[3];

할당된 영역에 대한 주소값이 생긴다.
(주소값을 실제로 볼 수가 없다.)

대입연산자.

오른쪽에 있는 값 new int[3]; 0x100 식의 주소값을
int[] arr이라는 곳에 들어간다.
new 연산자를 쓰면 주소값이 할당된다.


Stack		Heap		Static
		0x100
ㅁ = >    ㅁ	 ㅁ	ㅁ
	arr[0] arr[1] arr[2]


배열
(얇은 복사)

객체의 주소 값만 가져와 참조형 변수에 저장하고
하나의 객체를 두 변수가 참조하는 것

int[] arr1 = new int[4];

arr1 에 4개짜리 공간에 대한 주소값

int[] arr2 = arr1;

arr2 에 arr1의 주소값을 대입.
같은곳을 참조하게 된다.

arr1을 바꾸면 arr2도 바뀐다.

(깊은 복사)

arr1을 바꿔도 arr2가 바뀔일이 없다.

for(int i = 0; i < arr1.length; i++){
	arr2[i] = arr1[i];
}

system.arraycopy(arr1,0,arr2,0,arr1.length);
arr2 = Array.copof(arr1,arr1.lengh);
arr2 = arr1.clone();




