---
layout: post
title:  "2019년 2월 2주차 진행사항"
date:   2019-02-09 17:40:45 +0200
categories: jekyll update
---

이제 완성을 앞두고 여러가지 새로운 기술을 도입시켜서 시도해보았다.

첫번째로 배경색깔을 마스킹 할때 단순히 배열 값을 써서 특정 색깔의 범위를 가지는 부분(하늘)만 마스킹 하는것이 아닌

촬영하고자 하는 대상의 배경색을 추출하여 동적으로 배경을 마스킹 해서 좀더 정확하게 detection을 하기위한 노력을 해보았다.

간단하게 말하면 이미지 클러스터링을 통해 마스킹 할 대상의 배경을 동적으로 추출하는 것이라고 생각하면 된다.

예시는 다음과 같다.

- - -
![example1](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week6/capture1.JPG?raw=true){: width="900"}
- - -

- - -
![example2](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week6/capture2.JPG?raw=true){: width="900"}
- - -

- - -
![nice_performance](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week6/capture3.JPG?raw=true){: width="900"}
- - -

<br>
이로서 이미지 프로세싱 파트는 끝이 났다.
<br>
또한 머신러닝 파트도 추가적으로 데이터를 retrain시켜서 더 좋은 성능을 내는 것을 확인하였고 또한 기존의 sky, airplane, bird, tree
<br>
이렇게 선별하는 것 대신에 birds와 others로만 구분하게 해서 더 좋은 성능을 내게끔 코드를 수정하고 돌려 보았다.
<br>
다행히도 기존의 프로젝트 코드보다 더 좋은 성능을 내는 것을 확인했다. (물론 다른 영상에서도 그런지 더 추가적인 테스트를 해봐야 한다.)
<br>
이제 앞으로 남은 것은 계속해서 테스트 해보는 것과 논문을 쓰는것 두가지만 달성하면 프로젝트가 깔끔하게 끝날 것 같다.