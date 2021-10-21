# Matrix Matrix Multiplication
머신러닝 15강
<pre>
우리가 이전에 θ0 , θ1 변수들을 경사하강법에 사용하지 않고 어떻게 찾을 지에 대해 배우기 위해서는
어떠한 알고리즘에 대해 나중에 배울 것인데
이것을 배우기 위해서는 행렬 간의 곱셈을 배워야 한다.

<img width="322" alt="스크린샷 2021-10-21 오후 6 08 11" src="https://user-images.githubusercontent.com/63940620/138247173-30ab21e2-7117-44e7-afb3-7a19e677c1e3.png">

예를 들어 이러한 배열이 있다고 하자.
두 배열은 2 * 3 배열과 3 * 2 배열이다.

이 곱을 계산하기 위한 방법은 오른쪽 행렬에서 n*1 로 되어진 벡터 만큼 부분적으로 계산을 하는 것이다.


<img width="455" alt="스크린샷 2021-10-21 오후 6 10 49" src="https://user-images.githubusercontent.com/63940620/138247576-81e4a2bb-2782-40bc-a5ea-f2a3ba8e8005.png">
위의 그림처럼 말이다.

오른쪽 벡터도 똑같이 하면 된다.
<img width="432" alt="스크린샷 2021-10-21 오후 6 11 20" src="https://user-images.githubusercontent.com/63940620/138247652-45846d90-8248-4a3e-abf1-aafbb9767add.png">

그리고 최종적으로 이어 붙인다.
<img width="487" alt="스크린샷 2021-10-21 오후 6 11 54" src="https://user-images.githubusercontent.com/63940620/138247748-c340a2e5-3ebf-40f9-8ffd-e26e4d5c4246.png">

이러한 결과를 얻는다.
결과적으로 2 * 3 행렬 , 3 * 2 행렬에서 2 * 2 행렬을 얻게 되었다.

<img width="818" alt="스크린샷 2021-10-21 오후 6 14 53" src="https://user-images.githubusercontent.com/63940620/138248217-bbc2a391-f12b-437f-9c9f-03861ce6b0d1.png">

위의 그림은 행렬과 벡터의 곱 처럼 몇 차원의 행렬이 만들어지는지에 대한 것이다.
주의할점으로는) 차원의 행렬이 행렬 * 벡터와 같은 것이지 값은 다르다는 것을 인지하자.

![image](https://user-images.githubusercontent.com/63940620/138249173-aed7840d-5fae-48dd-add5-014089177691.png)
저번 글을 이해했다면 이 그림 하나만으로 완벽하게 이해할 수 있다.

그래서 이거를 왜 하는데?라고 물어본다면

<img width="820" alt="스크린샷 2021-10-21 오후 6 21 41" src="https://user-images.githubusercontent.com/63940620/138249315-b4ba3889-0109-41dc-bd5b-fd4aecf61379.png">

위의 그림을 보면 3개의 일차함수 식이 있다. 이것의 hθ(x)에 대한 식을 행렬로 매우 매우 간편하게 계산 할 수 있다.
</pre>
<pre>
한줄정리)
  - 행렬간의 곱셈을 배웠다.
</pre>
