---
layout: post
title:  "To do list - week4"
date:   2019-01-21 15:40:45 +0200
categories: jekyll update
---

이번에 실제로 코드를 돌려 보고 여러가지를 테스트 해보았다.

실제로 코드가 돌아가는 부분은 detection.py 부분에 다 구현되어 있었다.

Data Preprocess는 다음과 같다.
1. convert to hsv (#1 frame)
2. make the frame extracted only leaf (#2 frame) + median
3. remove all leaves on original frame by using  #2 frame (#3 frame)
4. resize each all frames
5. apply #3 frame with MOG (#4 frame) + median

실제로 그림으로 보자면 다음과 같다.
- - -
![picture1](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week4/1_21_1.JPG?raw=true){: width="930"}
- - -
![picture2](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week4/1_21_2.JPG?raw=true){: width="930"}
- - -

또한 이전 팀에서 했던 것을 박준원 팀원의 주도하에 문서로 정리 해보는 시간을 가졌다.

![picture3](https://github.com/JoJeongJin/jojeongjin.github.io/blob/master/assets/_week4/1_21_3.JPG?raw=true){: width="930"}
- - -

이로서 다음 단계는 전처리 또는 머신러닝을 최적화 시키는 방식으로 프로젝트를 진행해 나갈 예정이다.