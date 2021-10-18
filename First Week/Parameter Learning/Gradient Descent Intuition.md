# Gradient Descent Intuition
머신러닝 10강
<pre>

<img width="660" alt="스크린샷 2021-10-18 오전 9 44 52" src="https://user-images.githubusercontent.com/63940620/137651357-90d8927f-81d5-4a28-8fbc-f9e5956cb030.png">
저번 시간에 배운 경사 하강법 알고리즘이다. 하지만 a(Learning rate)와 뒤의 미분계수에 대해 정확하게 짚고 넘어가지 않았다.
이번 글에서는 이 애매한 부분을 해결할 것이다.


<img width="590" alt="스크린샷 2021-10-18 오후 3 57 12" src="https://user-images.githubusercontent.com/63940620/137683106-cc090ca0-f865-490e-a8ca-9b1bcb9cfb8b.png">
J(θ1)에 대한 (변수 하나)에 대한 이차함수이다.

J(θ1)에 대한 경사하강법 공식이다. 이것을 쉽게 풀어서 해석해보자.
<img width="407" alt="스크린샷 2021-10-18 오후 3 59 05" src="https://user-images.githubusercontent.com/63940620/137683359-7f1da3e6-7a6e-407f-8a09-b3c70dbfb6c1.png">

참고 !!!
아래의 두 사진들은 미분계수로 같은 값을 의미합니다. ( 기호의 차이 )
<img width="78" alt="스크린샷 2021-10-18 오후 4 01 09" src="https://user-images.githubusercontent.com/63940620/137683590-e2cc440d-73d0-4a76-a95b-fcc970159e3d.png">

<img width="88" alt="스크린샷 2021-10-18 오후 4 01 18" src="https://user-images.githubusercontent.com/63940620/137683611-7b393097-3350-4c08-a202-a0dadaacea26.png">

여기서 미분계수는 말 그대로 미분의 계수를 의미한다.

먼저 '미분'이란 미분(微分)으로 작을 미 , 나눌 분이다.
즉, 작게 나눈다는 뜻이다.

<img width="401" alt="스크린샷 2021-10-18 오후 4 08 00" src="https://user-images.githubusercontent.com/63940620/137684404-910236c3-934b-487a-bd17-6a1597e0cd8a.png">

위의 그림을 보자.
함수라는 것은 무수히 작은 값이 나와도 엄청 큰 값이 나와도 y값을 가지고 있다. (기본 지식)
위에 그림에는 매우 작게 나눠진 값(어떠한 적당한 값 , 초기에 선언하는 값)에 대한 J(θ1)의 값을 가지는 점이 있다.

그 다음에
*** 작게 나눠진 한 점을 지나는 접선의 기울기를 구한다 ***

<img width="391" alt="스크린샷 2021-10-18 오후 4 22 55" src="https://user-images.githubusercontent.com/63940620/137686182-4aaed621-87e6-44af-aa15-abadece842bc.png">

위의 일차함수의 기울기는 어떤가?
  - 위의 일차함수의 기울기는 양수이다.
그러면 θ1(변수 한개)에 대한 경사하강법은 θ1 - (양수)가 된다.
그러므로 최솟값 보다 오른쪽에 있는 점이 왼쪽(뺄셈)으로 간다.

만약 어떤 값(초기에 정한 값 or 계산하고 나온 값)이 최솟값보다 왼쪽에 있을 때는 어떻게 되는가?

<img width="414" alt="스크린샷 2021-10-18 오후 4 30 22" src="https://user-images.githubusercontent.com/63940620/137687189-fe6d47bc-ef28-4814-8c06-3732a788973f.png">

위의 그림을 보면 알겠지만
최솟값의 왼쪽에 있는 점에 접하는 직선의 기울기는 음수이다. 
그러므로 θ1 := θ1 - (음수) 이므로 결과적으로 값은 점점 오른쪽(덧셈)으로 간다.

이 방식으로 최솟값이 아닌 점은 최솟값을 향해 간다.
여기까지가 미분계수에 대한 설명이다.


다음으로 알아볼 것은 a(learning rate)이다. 앞에서 a는 보폭 과 같다고 하였다.


<img width="917" alt="스크린샷 2021-10-18 오후 4 36 52" src="https://user-images.githubusercontent.com/63940620/137688076-d63a58fe-0e34-4083-9ace-d97f7bdd9c8a.png">
그림을 보면 a값이 작아서 최솟값으로 내려가는데 오랜 시간이 걸린다. 비유를 하자면 같은 거리를 보폭을 작게 걷는 것과 같다.

만약 a값이 '매우 크다면' 어떨까?

<img width="930" alt="스크린샷 2021-10-18 오후 4 38 02" src="https://user-images.githubusercontent.com/63940620/137688229-9fbe97a5-d2f6-4446-b34a-a2ea8e64656c.png">

a값이 너무 크다면 값이 최솟값을 넘어가서 최솟값에 도달하지 못한다. 비유를 하자면 10mm거리를 보폭 1.5m 크기로 걷는 것과 같다. 

경사하강법의 문제점:

만약 이러한 함수가 있다고 하자.
<img width="758" alt="스크린샷 2021-10-18 오후 4 40 28" src="https://user-images.githubusercontent.com/63940620/137688569-3b175d90-17b8-4c92-9961-15b5df3736dd.png">

적절한 변수를 놓았을 때 어느 위치냐에 따라 지역 최솟값(Local minima) or 전역 최소값(global minima)가 될 수 있다.
(어느 한 논문에 따르면 Local minima에 빠질 확률이 매우 매우 적다고 한다. https://darkpgmr.tistory.com/148)
</pre>
<pre>
한줄정리)
  - 경사하강법의 '미분계수'와 '학습비율'이 만들어지는 과정과 그 이유에 대해 배웠다.
</pre>