# [Mirror_fairyTale] Deepfake project 거울동화

## 1. Deepfake project 소개
거울동화 프로젝트는 실제 얼굴 사진을 동화 캐릭터 애니메이션에 삽입하여 아이들의 정서적, 교육적 목적을 위해 진행되고 있는 프로젝트이다. 해당 프로젝트는 Deepfake 기술을 사용하기 위해 Faceswap, DeepfaceLab 라이브러리를 활용하여 실제 얼굴 이미지를 다양한 방식을 통해서 애니메이션 영상에 접목시키기 위한 연구를 진행 중이다.

![20220124_112627](https://user-images.githubusercontent.com/67012957/152676877-056e8057-9165-4782-948a-267ea460d6b8.png)
![20220124_112613](https://user-images.githubusercontent.com/67012957/152676861-992c2e04-0226-4c1c-bac1-8369801a725b.png)

---

## 2. Deepfake project 연구 내용
애니메이션은 유튜브의 가디언즈 애니메이션을 선택하여 학습 진행하였다.

### 2.1. TEST 1 - 실제 인물 사진 + 애니메이션 결합
실제 인물 사진을 여러 방향으로 촬영하여 영상으로 변환 후 학습 진행

![학습사진](https://user-images.githubusercontent.com/67012957/152676907-792253ca-2964-4504-8386-a8c3133e5db6.PNG)
![20220124_1129220](https://user-images.githubusercontent.com/67012957/152676898-6d5704d9-4d45-410a-bf3a-7ce49cb61807.png)

**- 학습 결과 : 애니메이션 영상에 실제 인물 사진을 직접 학습하다 보니 눈 크기, 스타일, 질감 등등 어색한 부분이 많이 발생하였다.**

---

### 2.2. TEST 2 - 캐릭터화 사진 + 애니메이션 결합
실제 인물 사진을 TOONME라는 사진 캐릭터 변환 프로그램을 사용하여 캐릭터화한 뒤,    
캐릭터화한 사진들을 이어붙여 영상으로 변환 후 학습 진행

![학습사진2](https://user-images.githubusercontent.com/67012957/152676916-651c9ee9-9e0d-4747-9508-08a1b65b8a55.PNG)

**- 학습 결과 : TEST 1 결과보다는 훨씬 영상미가 자연스러워졌지만,    
캐릭터가 대사를 읽을 때 입이 벌어지지 않는 등의 섬세한 작업 오류 문제 발생**

---

### 2.3. TEST 3 - 캐릭터화 영상 필터 + 애니메이션 결합
실제 인물 사진을 스노우 어플의 캐릭터화 영상 필터를 사용하여 영상으로 변환 후 학습 진행

![dongha_fin](https://user-images.githubusercontent.com/67012957/152676609-6d6ced1e-64ee-4f7e-b5a5-fb47385c2f29.png)
![20220124_1125219](https://user-images.githubusercontent.com/67012957/152676891-14164e98-fc00-4062-9a04-cdc1a2b8dbf6.png)

**- 학습 결과 : TEST 1,2 결과보다 훨씬 영상미가 자연스러워지고, 캐릭터 대사 시 입이 함께 벌어짐과 함께 섬세한 영상 제작 완성!    
그러나, TEST 1,2 보다 더 오랜기간 학습을 하였지만 데이터가 다소 깨지는 현상 발생**

---

## 3. Deepfake project 결과
