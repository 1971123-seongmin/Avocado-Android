## AvocaDo
<p align="center">
 <img width="350" src="https://github.com/user-attachments/assets/5d413d5c-76dc-424b-ad4e-ed5c510bcefb" alt="아보카도"/>
</p>
<div align="center">
 생성형 AI 기반 영어단어 암기 보조 서비스 AvoCado (안드로이드 파트)
</div>

## 개요
- 2024년 한성대학교 창업동아리에서 진행한 프로젝트로, 생성형 AI를 활용해 영어단어 암기를 더 쉽고 재밌게 할 수 있도록 도와주는 앱입니다.
- 프로젝트 이름: AvocaDo (한성대학교 창업동아리)
- 프로젝트 기간: 2024.04 ~ 2024.07
- 개발 엔진 및 언어: Android Studio, Kotlin
- 멤버: 박지원, 김성민 외 기획 1명, 디자인 2명, 백엔드 2명, AI 1명

## 목차
  - [내용](#내용)
  - [화면](#화면)
  - [기술스택](#기술스택)
  - [저작권](#저작권)
  - [실행영상(챗봇)](#실행영상챗봇)
  - [느낀점](#느낀점)

## 내용
- **`로그인` :** 네이버, 카카오 소셜 로그인
- **`홈 화면` :** 출석체크를 통한 캐릭터가 성장, 인기 검색어, 추천 단어로 라이브러리에서 단어 학습
- **`단어장` :** 단어 검색 및 단어 학습 / 단어를 라이브러리에 저장 및 삭제 가능
- **`검색 화면` :** 단어를 검색하여 해당 단어를 단어장에서 공부 / 최근 검색어 검색
- **`라이브러리` :** 사용자 자신만의 라이브러리에 단어를 저장해 두고 볼 수 있다.
- **`생성형 AI 기반 학습 보조 (챗봇)` :**
    - 서버에서 파인 튜닝된 AI가 생성한 결과물을 받아 영어 단어 학습을 돕는다.
    - 서버 응답의 데이터 타입(뜻, 유사어, 어원, 팁)을 앱에서 판별하여 각 모드에 맞는 리스트나 카드 형태의 UI로 출력한다.
      - 단어의 뜻 : 단어의 의미와 상세 설명 데이터
      - 유사한 단어 : 맥락이 유사한 단어 목록
      - 어원 분류 : 단어의 어원 정보
      - 암기 팁 : AI가 생성한 암기 비법 데이터

## 화면

| **시작 화면** | **메인 홈** | **검색 화면** |
| :---: | :---: | :---: |
| <img width="250" src="https://github.com/user-attachments/assets/6eed4853-1376-4abb-b80c-8b0c29bf9ad0"/> | <img width="250" src="https://github.com/user-attachments/assets/5e1aa0ab-1a78-476b-8ac4-f8598a5b4d27"/> | <img width="250" src="https://github.com/user-attachments/assets/c54befd9-889f-4645-86e7-66b97f8a18c2"/> |

| **라이브러리** | **단어장** | **챗봇** |
| :---: | :---: | :---: |
| <img width="250" src="https://github.com/user-attachments/assets/858d1dce-822a-49e8-a6ce-a2a591475678"/> | <img width="250" src="https://github.com/user-attachments/assets/c7c2c408-2c3c-4b0f-b072-a823a6a14386"/> | <img width="250" src="https://github.com/user-attachments/assets/0b498551-af50-4098-ba2c-d0886c8ad5ab"/> |

---
## 기술스택
### **🤖** 안드로이드
| **Category** | **TechStack** |
| --- | --- |
| **Language** | Kotlin |
| **UI** | XML |
| **Architecture** | Repository Pattern, MVVM |
| **DI** | Hilt |
| **Network** | Retrofit, OkHttp |
| **Asynchronous** | Coroutines, Flow |
| **Jetpack** | DataBinding, Navigation, DataStore |
| **Social Login** | Kakao, Naver |
| **Image** | Glide |

## 저작권
Copyright 2024. 전세원 All rights reserved.<br>
ⓒ 2024. 전세원 All rights reserved.<br>
(c) 2024. 전세원 All rights reserved.

## 실행영상(챗봇)
<div align="center">
  <video src="https://github.com/user-attachments/assets/698a7b8d-fa76-4199-bea6-427367500543" width="200" height="200" controls>
  </video>
</div>

## 느낀점
- **다양한 직군과의 협업**: 창업동아리 프로젝트를 통해 기획, 디자이너, 백엔드 개발자와 함께 팀으로 소통하며 하나의 서비스를 처음부터 끝까지 완성하는 과정을 경험했습니다. 특히 피그마 디자인 가이드를 보고 UI를 구현하고, 백엔드와 API 명세서를 보며 조율하여 서버 연결 작업을 하는 등 실제 개발 프로세스의 기초를 경험할 수 있었습니다.

- **사용자 중심의 기능 구현**: 단순히 기술 구현에 그치지 않고, 캐릭터 성장 시스템 등 사용자의 재미와 편의를 고려한 기능을 구현하며 사용자 관점에서 앱을 바라보는 관점을 경험했습니다.

- **UI 설계**: 챗봇 결과의 데이터 타입별로 모두 다른 글자 수와 뷰 구조를 가진 챗봇 카드 UI를 구현하며, 개별 레이아웃 대응 방식의 한계를 경험했습니다. 이를 통해 앞으로의 개발 과정에서 재사용 가능한 컴포넌트 설계와 확장성 있는 UI 설계의 중요성을 체감하는 중요한 경험이 되었습니다.
