# SNAP Service 서버
## 서비스
> AI를 활용한 포토부스 웹 서비스

![main](https://i.postimg.cc/DZ2snJsw/main.png)

SNAP은 인공지능을 응용한 포토부스 서비스로</br>
AI를 활용한 포토부스 시장에서의 앞으로 추가되기에 적합한 서비스입니다.
이미지 저장, 불러오기, AI기반 필터링, AI 포즈 추천등
다양한 편의 기능을 포함하고 있습니다.

## 팀원
| 프론트엔드 | 백엔드 |
| :----:    | :----: |
| 김준경, 전예빈, 조병진 | 이찬혁 |

## 기능
> 다양한 AI 활용 서비스
### 1. 이미지 촬영 </br>
웹캠을 이용하여 촬영 (휴대폰 같은 외부 장치 사용 가능), 촬영한 사진을 서버에 업로드함,</br>
후에 2번째 기능을 통해 편집 가능
### 2. 이미지 AI 필터링 </br>
촬영한 이미지를 미드저니 AI를 통해 키워드에 맞은 이미지로 변환</br>
ex) 수채화, 에니메이션 캐릭터, 역동적인..
### 3. AI 촬영 포즈 추천 </br>
어떤 포즈로 사진을 찍을지 고민될때, Chat GPT AI를 통하여 4가지의 포즈를 추천받을 수 있음

## 구조
> 유연하고 확장성 높은 서버 구조

![](https://i.postimg.cc/wBYL4bjJ/map.png)

### 1. 다양한 AI API 사용
Chat GPT 3.5 API, Midjourney API를 통해 사용자에게 다양한 AI 서비스 제공

### 2. 서비스 아키텍처
특정시간에 트래픽이 급증하는 포토부스 시장 특성상, 안정적이고 유연한 서비스 공급을 위해, MSA구조로 각서비스를 AWS의 EC2로 분리한뒤  로브벨런서를 통해 안정적이고 유동적인 서비스

### 3. CICD 구축
Git Actions를 통한 지속적 통합/지속적 배포를 통하여 빠른 개발속도

### 4. SSL 인증
Gabia 도메인의 네임서버를 변경한뒤 CloudFlare의 DNS 프록시를 통해 HTTPS 사용

## 기술 스택

1. 프론트엔드

| Typescript | Zustand |  Next   |
| :--------: | :--------:  | :------: |
|   ![](https://i.postimg.cc/zXvpZMSR/ts.png)    |   ![](https://i.postimg.cc/x8cmhrDf/zustand.jpg)     | ![](https://i.postimg.cc/7Yq83x4r/next.png) |

2. 백엔드

| Java 17    | Spring Boot |  Amazon Web Service   |  Cloud Flare   |
| :--------: | :--------:  | :------: | :-----: |
|   ![](https://i.postimg.cc/RFR7HQ9t/java.jpg)    |   ![](https://i.postimg.cc/nc5vBL83/spring.png)     | ![](https://i.postimg.cc/BnrB9nMj/aws.png) | ![](https://i.postimg.cc/VvkjBrLV/cloudflare.png) |

<br>

## 배운점 / 느낀점
> 새롭고 다양한 AI 경험

이번 연합해커톤에서 AI API를 자주 사용하며, 생각보다 AI는 어려운 기술이 아니고, 적은 비용으로도 서비스의 품질을 크게 높일 수 있다는것을 알았다.
특히, 미드저니 API를 사용하며, 힘들줄 알았던 고해상도의 이미지 생성을 쉽게 할 수 있었다. 추후 진행할 다양한 프로젝트의 문제 해결로 AI 기술을 사용할 수 있을 것 같다.