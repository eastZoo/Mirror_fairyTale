
# [Mirror_fairyTale] Deepfake project 거울동화

## 1. Deepfake project 소개
거울동화 프로젝트는 실제 얼굴 사진을 동화 캐릭터 애니메이션에 삽입하여 아이들의 정서적, 교육적 목적을 위해 진행되고 있는 프로젝트이다.
해당 프로젝트는 Deepfake 기술을 사용하기 위해 Faceswap, DeepfaceLab 라이브러리를 활용하여 실제 얼굴 이미지를 다양한 방식을 통해서 애니메이션 영상에 접목시키기 위한 연구를 진행 중이다.
  <div>
    <img src="https://user-images.githubusercontent.com/67012957/152676877-056e8057-9165-4782-948a-267ea460d6b8.png" width="500" height="260">
    <img src="https://user-images.githubusercontent.com/67012957/152676861-992c2e04-0226-4c1c-bac1-8369801a725b.png" width="500" height="260">
  </div>
---


## 2. Deepfake project 연구 내용
애니메이션은 유튜브의 가디언즈 애니메이션을 선택하여 학습을 진행했다.

### 2-1. TEST 1 - 실제 인물 사진 + 애니메이션 결합
실제 인물 사진을 여러 방향으로 촬영하여 영상으로 변환 후 학습을 진행했다.

<div>
    <img src="https://user-images.githubusercontent.com/67012957/152679653-8ea84c0d-7c45-4795-9d76-97bea98e786a.png">
    <img src="https://user-images.githubusercontent.com/67012957/152681285-16abf978-c7af-4d5d-a188-236fa1a2c2c1.gif">
</div>


**- 학습 결과 : 애니메이션 영상에 실제 인물 사진을 직접 학습하다보니 눈 크기, 스타일, 질감 등등 어색한 부분이 많이 발생하였다.**

---

### 2-2. TEST 2 - 캐릭터화 사진 + 애니메이션 결합
실제 인물 사진을 'TOONME'라는 사진 캐릭터 변환 프로그램을 사용하여 캐릭터화한 뒤,    
캐릭터화한 사진들을 이어붙여 영상으로 변환 후 학습을 진행했다.

<div>
  <img src="https://user-images.githubusercontent.com/67012957/152679660-6dfab81e-f2d3-4a54-83b6-f30af1064ed1.png">
  <img src="https://user-images.githubusercontent.com/67012957/152681304-9c8bb6ee-4379-473a-8ee3-4d57c096cae2.gif">
</div>


**- 학습 결과 : TEST 1 결과보다는 훨씬 영상미가 자연스러워졌지만,    
캐릭터가 대사를 읽을 때 입이 벌어지지 않는 등의 섬세한 작업에서 오류 문제 발생하였다.**

---

### 2-3. TEST 3 - 캐릭터화 영상 필터 + 애니메이션 결합
실제 인물 사진을 스노우 어플의 캐릭터화 영상 필터를 사용하여 영상으로 변환 후 학습을 진행했다.

<div>
  <img src="https://user-images.githubusercontent.com/67012957/152679669-d3f16306-e34c-4ec6-bddd-2be0af3b254c.png">
  <img src="https://user-images.githubusercontent.com/67012957/152681319-7e28cb2c-7963-4936-a2b3-7a910545008a.gif">
</div>

**- 학습 결과 : TEST 1,2 결과보다 훨씬 영상미가 자연스러워지고, 캐릭터 대사 시 입이 함께 벌어짐과 함께 섬세한 영상 제작에 성공했다.
그러나, TEST 1,2 보다 더 오랜 기간 학습을 진행했지만 결과 데이터가 다소 깨지는 현상이 발생하였다.**

---

## 3. Deepfake project 결과
TEST를 진행하면서 실제 인물을 캐릭터화하는 방향으로 자연스러움과 정확도를 개선하고자 했다.
추후 TEST 1, TEST 2, TEST 3의 결과를 바탕으로 각각의 TEST에서 발생했던 문제점을 개선하기 위해 명도, 채도 및 선명도의 차이를 둔 여러 경우의 데이터셋(Dataset)을 이용한 테스트 케이스(Test Case)를 작성해 연구를 계속 진행하고자 한다.





