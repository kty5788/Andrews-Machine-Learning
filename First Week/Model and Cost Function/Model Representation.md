# Model and Cost Function
머신러닝 5강
<pre>

지도 학습 (Supervised Learning)의 전반적인 과정에 대해 알아보자.

아래의 그림은 Oregon과 Potland 도시의 주택 가격 데이터이다.
<img width="741" alt="스크린샷 2021-10-15 오후 4 17 11" src="https://user-images.githubusercontent.com/63940620/137447475-7bde1886-98bc-445a-ac9a-ca10e286f3a7.png">

주택 가격을 예측하는 가장 쉬운 방법은 모형에 맞춘 일직선을 그려보는 것이다.

<img width="722" alt="스크린샷 2021-10-15 오후 4 24 43" src="https://user-images.githubusercontent.com/63940620/137448456-dfccd726-4cd1-4821-9140-d3d7b2679754.png">

이것은 지도학습의 예이다. 

이것이 지도학습의 예라고 불리우는 이유는 : 데이터의 예시에 '적합한 답'을 주기 때문이다.
(다시 말해, 가격을 예측하는 회귀라는 의미의 문제이기 떄문이다.)

우리의 목표 : 이 데이터로부터 어떻게 주택 가격을 예측할 지 고민하고 학습시키는 것이다.
<img width="745" alt="스크린샷 2021-10-15 오후 4 32 45" src="https://user-images.githubusercontent.com/63940620/137449512-26ce258c-c2eb-4389-99b7-2ae4269eae70.png">

공식적으로, 지도 학습에서 데이터 셋을 가지고 있을 때 이 데이터 셋을 학습 셋이라고 부른다.

</pre>
