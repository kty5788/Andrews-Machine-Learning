# Addition and Scalar Multiplication
머신러닝 13강
<pre>
이번 글에서는 행렬과 행렬의 덧셈 , 스칼라곱이라고 하는 행렬과 상수 간의 곱셈을 배워 볼 것이다.
정말 정말 쉬우니까 걱정하지 말자.

<img width="368" alt="스크린샷 2021-10-20 오후 5 59 37" src="https://user-images.githubusercontent.com/63940620/138062350-7a1ea6a0-e726-48ac-8f3d-a36d3865aedc.png">
위의 그림에서 행렬간의 덧셈을 하면 어떤 결과가 나올까?

본인이 행렬의 덧셈을 몰라도 맞추는 사람이 꽤 있을 거다.
바로 이렇게 더해진다.
<img width="590" alt="스크린샷 2021-10-20 오후 6 01 02" src="https://user-images.githubusercontent.com/63940620/138062598-2baedad4-e718-4ad0-9a33-cafaaa27cee8.png">

행렬 간의 덧셈을 할 때에는 같은 위치의 원소들 끼리 더 할 수 있다. (뺄셈도 마찬가지이다.)

<img width="388" alt="스크린샷 2021-10-20 오후 6 02 14" src="https://user-images.githubusercontent.com/63940620/138062819-597147cc-84f2-4377-b7e6-f13e9be50362.png">
만약 위의 그림처럼 다른 차원의 행렬 간의 덧셈을 하게 되면 어떻게 될까?
  - 차원이 다른 행렬간의 덧셈은 '불가능'하다. 정확히는 에러가 난다.


다음으로 행렬의 스칼라곱을 알아 보겠다.

여기서 스칼라란?
  - 숫자 또는 실수를 가리키는 용어이다.

<img width="253" alt="스크린샷 2021-10-20 오후 6 05 39" src="https://user-images.githubusercontent.com/63940620/138063353-0c233f90-5aaf-4b69-8b46-1c023f348307.png">
이 그림에서 실수 3과 행렬간의 곱이다.

이 것도 되게 쉽다.
행렬의 각각의 요소에 실수를 곱해주면 된다.
<img width="441" alt="스크린샷 2021-10-20 오후 6 09 18" src="https://user-images.githubusercontent.com/63940620/138063986-9305290e-0d54-4aed-a562-40fe7d10c159.png">

만약에 곱이 아니라 나누기 이면 어떨까?

<img width="211" alt="스크린샷 2021-10-20 오후 6 09 47" src="https://user-images.githubusercontent.com/63940620/138064061-74865087-0163-411d-94da-a8299c88c916.png">

나누기는 그냥 간단하게 역수의 곱을 취한다고 생각하면 된다. (아니면 그냥 나눠도 된다,)
</pre>
<pre>
한줄정리)
  - 행렬간의 덧셈을 배웠고 , 행렬과 스칼라곱을 배웠다.
</pre>