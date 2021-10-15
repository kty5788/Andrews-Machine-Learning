# Unsupervised Learning
Andrew Ng Machine Learning fourth course<br>
Andrew Ng 머신 러닝 4번째 강의
<pre>
전에 배웠던 악성 종양 구별 데이터를 다시 불러와보자.

<img width="449" alt="스크린샷 2021-10-15 오후 12 05 10" src="https://user-images.githubusercontent.com/63940620/137425872-8f540bb9-7cef-4f1b-943e-4a604218e0b0.png">

지도 학습에서는 명시적으로 어떤 게 양성인지 악성인지 소위 말하는 '정답'이 있다.
하지만 '비지도 학습'에서는 지도 학습과 다르게 주어진다.

<img width="464" alt="스크린샷 2021-10-15 오후 12 05 46" src="https://user-images.githubusercontent.com/63940620/137425933-0c8faac5-9308-4873-bc83-57af8ee351cc.png">

위의 데이터처럼 어떤 레이블도 갖고 있지 않거나 , 모두 같은 레이블을 갖고 있거나 , 또는 아예 레이블이 없는 경우도 있다.
그래서 이 데이터들로 무엇을 할지 , 또 각 데이터가 무엇인지 알 수 없다.

'이러한 데이터가 있을 때 어떤 구조를 찾을 수 있는 가?'에 대해서만 알 수 있다.

비지도 학습 알고리즘은 이 데이터에서 두 개의 클러스터(cluster)가 있다고 판단한다.
아래의 그림처럼

<img width="431" alt="스크린샷 2021-10-15 오후 12 08 17" src="https://user-images.githubusercontent.com/63940620/137426114-b0e4e7fa-4ed3-414b-91c0-6225870b24a2.png">

이러한 방식은 '구글 뉴스'에서 자주 사용된다.
(비슷한 or 같은 주제를 가진 뉴스들이 묶여서 같이 표시되는 것)


이것을 '클러스터링 알고리즘'이라고 한다.


비지도 학습의 클러스터링 알고리즘은
구글 뉴스를 제외하고 유전학적 자료 이해 , 대규모 컴퓨터 클러스터 , 소셜 네트워크 분석 , 시장 세분화 , 천문학 데이터 분석에도 쓰인다.

-----------------------------------------------------------------------------------------------------
이 이후로는 Octave 무료 오픈 소스 프로그래밍을 통해 강의가 이루어 질 것입니다.
-----------------------------------------------------------------------------------------------------
</pre>
<pre>
한줄 정리)
  '비지도 학습'은 알고리즘이 스스로, 오직 데이터로부터 알아내는 것이다. '비지도 학습'의 대표 알고리즘은 '클러스터링 알고리즘'이 있다.
</pre>