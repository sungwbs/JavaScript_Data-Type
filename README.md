# JavaScript_Data-Type

### 1. 데이터 타입에 관한 배경지식
> 자바스크립트 언어는 숫자 타입의 경우 정수형인지, 부동 소수형인지 구분하지 않고 64비트, 즉 8바이트를 확보합니다.

- 변수 = 변할 수 있는 데이터

- 식별자 = 변수명

- 리터널 = 변수에 할당하는 테이터

<br/> 

### 2. 변수선언과 데이터 할당
![](https://velog.velcdn.com/images/sungwbs/post/ac793a98-3f20-4d07-aaf8-b5fbd3b295fa/image.png)

1. ↑ 위에 그림을 보시면 a라는 변수가 @1003이라는 빈 공간을 확보합니다. 하지만 데이터영역에는 아무 값이 없습니다. 이러한 경우 식별자 a만 인식하고 출력시 **undefined**가 나옵니다. ( 호이스팅 )

![](https://velog.velcdn.com/images/sungwbs/post/9bd4bfc8-c774-4b9a-a65f-fc04f6f9978c/image.png)

2. ↑ 다음은 데이터영역 @5004에 ' abc '를 저장하고 @1003 공간 즉, 변수 a가 가지고 있는 공간 값에 저장합니다. 이러한 경우 값이 채워지게 됐으므로 a를 출력시 **' abc '**라는 값을 출력합니다.

![](https://velog.velcdn.com/images/sungwbs/post/662111da-e47e-46b7-afdc-d90a682c55e5/image.png)

2-1. ↑ 이 그림을 보시면은 @1003이라는 변수 a의 공간에 값을 @5004 주소를 넣었지만, @5005라는 주소값으로 바꾼 것을 볼 수 있습니다. 변수는 그대로 있고 값 영역에 주소만 바뀌었습니다. 변수 a를 출력시 @5005의 값인 **' abcdef '** 출력됩니다.

> ex) 만약에 500개의 변수를 생성해서 모든 변수에 숫자 5를 할당한다면?

- 위에서 언급했듯이 하나의 변수 공간을 생성할 때 8 바이트를 확보해야 합니다. 그리하여 500개의 변수를 생성할 때는 ( 500 * 8 ) = 4000 바이트가 소모가 됩니다.

- **그러나** 위에서 데이터 값에 주소를 저장해 주는 방식은 1 바이트만 소모가 됩니다. 그리하여 숫자 5를 한 번만 저장하고 해당 주소만 변수 영역에 저장하는 게 더 효율적으로 메모리 공간을 사용할 수 있습니다! ( 508byte )

** 결론 = 메모리 공간 사용량 4000 byte < 508 byte**

<br/> 

### 3. 변수 안에서 선언된 배열이나 키값이 메모리에 저장되는 방식

1. ![](https://velog.velcdn.com/images/sungwbs/post/dff31a3b-6238-46b3-acdb-6b19c59674c6/image.png)

![](https://velog.velcdn.com/images/sungwbs/post/fa426181-8524-4fc3-9696-7f10d54d9e7e/image.png)

2. ![](https://velog.velcdn.com/images/sungwbs/post/1f740de0-8f8a-44ce-874b-e9976371c181/image.png)

![](https://velog.velcdn.com/images/sungwbs/post/9e66487f-85b4-4bdb-b096-aab8ea739342/image.png)
![](https://velog.velcdn.com/images/sungwbs/post/10ba0b90-3f15-4fb5-b6a5-92609944cfe7/image.png)
