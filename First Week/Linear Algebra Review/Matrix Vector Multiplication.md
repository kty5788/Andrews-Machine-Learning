# Matrix Vector Multiplication
머신러닝 (14강)
<pre>
행렬 벡터 간의 곱셈을 알아보겠다.

예제를 보자.
<img width="242" alt="스크린샷 2021-10-21 오후 3 22 16" src="https://user-images.githubusercontent.com/63940620/138222473-afb36492-733e-4e09-abdb-656404b8400a.png">

위의 두 개의 행렬들은 서로 다른 차원을 가지고 있다.

행렬과 벡터간의 곱셈 방법은

<img width="378" alt="스크린샷 2021-10-21 오후 3 25 10" src="https://user-images.githubusercontent.com/63940620/138222852-5cd26520-0f4f-4824-9202-a2e2c7a5f52d.png">

* A행렬의 첫 번쨰 행과 , 행의 숫자에 이에 대응하는 수를 곱해서 더할 것이다. *
(1 * 1 + 3 * 5 = 16)

<img width="394" alt="스크린샷 2021-10-21 오후 3 26 51" src="https://user-images.githubusercontent.com/63940620/138223062-60c4644a-a250-4398-b8ee-b7fb64f85a6e.png">

이런 식으로 계속 계산을 하다보면 3 * 1 짜리 벡터가 나온다.

<img width="378" alt="스크린샷 2021-10-21 오후 3 29 16" src="https://user-images.githubusercontent.com/63940620/138223354-f8933dac-562a-47f5-8df6-3fe20080cbe1.png">

3*2 차원의 행렬과 2 * 1 벡터의 곱을 하고 나니 3 * 1짜리 벡터가 생겼다.

** m * n 행렬과 n * 1 벡터의 곱은 무조건 m * 1 차원의 벡터가 나온다.
<img width="594" alt="스크린샷 2021-10-21 오후 3 33 35" src="https://user-images.githubusercontent.com/63940620/138223902-43d56b35-5982-4696-950d-3a6f61764f1a.png">

이해가 되지 않는 사람들을 위해 하나만 더 풀어보자.

<img width="475" alt="스크린샷 2021-10-21 오후 3 36 09" src="https://user-images.githubusercontent.com/63940620/138224253-2a0b1eab-9654-4c63-beac-49664a804032.png">

1 * 1 + 2 * 3 + 1 * 2 + 5 * 1 = 14
0 * 1 + 3 * 3 + 0 * 2 + 4 * 1 = 13
-1 * 1 + (-2) * 3 + 0 * 2 + 0 * 1 = -7
이런 과정을 거쳐서
[14; 13; -7;]의 3 * 1 벡터가 나온다.

그래서 이거를 왜 배우냐?
  - 계산 , 연산을 더 빠르게 하기 위함이다.

<img width="745" alt="스크린샷 2021-10-21 오후 3 51 22" src="https://user-images.githubusercontent.com/63940620/138226269-e9e40c37-ddf9-44a5-b5c8-74647608a050.png">

위의 데이터를 가진 주택가격을 예측한다고 할때
행렬과 백터를 사용하여 쉽게 연산할 수 있다.

<img width="455" alt="스크린샷 2021-10-21 오후 3 54 41" src="https://user-images.githubusercontent.com/63940620/138226695-06188972-cdf4-4c64-b2ec-f18fe2cc3d99.png">


</pre>
