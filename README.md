# 🚌 교통약자를 위한 인쇄형 안내 키오스크
![image](https://github.com/user-attachments/assets/2a9a7ca7-8e54-4513-b285-b60347ee709f)

### 서비스 소개
교통약자를 위한 키오스크 길 찾기 프로그램인 “길:벗” 은 
순 한국말인 길과 벗을 합친 친근함이 묻어나는 합성어입니다. 
환승역을 몰라 버스에 탈 때마다 기사님께 길을 물어야되는 60대 김00 할머니
지나가는 택시마다 예약 중이어서 택시를 부르지 못해 추위에 한시간동안 떠는 70대 이00할아버지
디지털 시대에 기본적인 이동권을 보장받지 못하는 이들을 위해 “길:벗”은 
아날로그적 요소를 더해 교통약자의 이동에 디딤돌이 됩니다. 

---

### 팀원 소개

| 조해민 | 이주영 | 니스타 | 박찬호 |
| --- | --- | --- | --- |
| Front-end, 기획 | Front-end | Back-end(Google STT, TTS API 구현) | Back-end(Google Maps API 구현), Design |
| @chohaeminn | @ale8ander | @NishthaLath | @Codepumpking  |
| ![image](https://github.com/user-attachments/assets/97c7243b-10a5-41fa-a6c8-a7a66d9a05b5) | ![image](https://github.com/user-attachments/assets/79e0b7f0-ca94-4420-92a3-dc2bbacde397) | ![image](https://github.com/user-attachments/assets/dca32df1-f4ec-4b30-ab55-85221d90b792) | ![image](https://github.com/user-attachments/assets/24fd241a-cb9c-4e4f-a11a-a2190ce42f38)


---

### 🛠️ 주요기능

- 🗺️ 경로 약도 출력 서비스:
    - 어디서 무엇으로 환승해야하는지. 새로운 도착지까지 가는 길을 모르겠다고요?
    - 길:벗은 도착지까지 가는 여정 중 꼭 필요한  이동수단. 환승역. 도착역 등의 정보를 약도로 출력해줘요.
    - 해당 약도를 가지고 도착지까지 안심하고 갈 수 있어요.
    - 구글MAP API를 활용해 비용, 시간을 고려한 최적의 경로를 추천해줘요.
      
- 🎤 터치인식률이 떨어지는 노인을 위한 음성인식 기능:
    - 타자 치기가 어색하다면?🛠️
    - 연령대가 높아질수록 패드의 섬세한 터치인식률이 떨어지므로, 키오스크 사용에 불편함을 겪어요.
    - 음성인식이 텍스트로도 보여 익숙함에서 오는 안도감을 얻을 수 있어요.
    - 구글의 TTS와 STT 모델을 활용해 사용자의 음성을 인식해 검색해요.
    
- 🚕 택시 호출 서비스
    - 택시 이용율의 87%가 앱을 사용하시는 시대에 교통약자는  택시를 잡기가 힘들어요.
    - 길:벗이 대구로택시와 연계해 택시를 호출하고, 기사님의 정보까지 출력해드릴게요.
    - 대구로TAXI와 연계해 지역경제활성화를 이룰 수 있어요.

- 👵 교통약자 친화적 UI
    - 안내원 호출기능을 통해 문제가 생기면 주위 역무원에게 도움 요청이 가능해요.
    - 불필요한 요소를 지우고 필요한 정보를 큰 글씨로 담아 한눈에 파악이 가능해요.
    
    ---
### 시연 영상

https://github.com/user-attachments/assets/ea1db9d0-e893-4140-b8b5-936a34501f51

https://github.com/user-attachments/assets/adc7bf96-c417-4199-a60c-454b562029e9

https://github.com/user-attachments/assets/5b7f69b6-6e31-4145-b36e-4d3c4a41e5df

STT 시연영상 (용량 문제로 인하여 유튜브 링크 첨부)
https://youtube.com/shorts/wUzFPJoQFkM?si=IqeyyNgyLFtM0VEn

---

### 🖥️ 기술 아키텍처

![image](https://github.com/user-attachments/assets/9aa1f9d0-effe-44ac-8a48-1151a5a079b9)

## 2. 채택한 개발 기술과 브랜치 전략

### 1. **채택한 기술 스택**

### Front-end

- **React**
    - **장점**:
        - **컴포넌트 기반** 아키텍처로 코드 재사용이 용이하며, 유지보수성을 높여줍니다.
        - **Virtual DOM**을 통해 빠른 UI 업데이트가 가능하여 성능이 우수합니다.
        - **풍부한 생태계**: 다양한 라이브러리와 플러그인이 있어 개발이 수월합니다.
- **React Router**
    - **장점**:
        - 단일 페이지 애플리케이션(SPA)에서 **효율적인 라우팅**을 제공합니다.
        - 사용자가 앱을 탐색할 때 **페이지 리로드 없이** 부드러운 전환이 가능하여 UX를 향상시킵니다.
        - URL 구조에 따라 다양한 **경로 관리가 가능**하여, 페이지 전환을 간편하게 구현할 수 있습니다.

### Back-end

- **Node.js**
    - **장점**:
        - **비동기 I/O**와 이벤트 기반 서버 처리를 통해 고성능과 높은 처리량을 제공합니다.
        - **JavaScript 통합**으로, Front-end와 동일한 언어를 사용하여 개발이 수월합니다.
        - **경량 서버**: 빠른 응답성과 낮은 메모리 사용량으로 서버 자원을 효율적으로 사용합니다.
- **Express.js**
    - **장점**:
        - 간단하고 유연한 API를 통해 **빠른 서버 구축**이 가능합니다.
        - 다양한 미들웨어와 라우팅을 제공하여, **효율적인 요청 처리**를 할 수 있습니다.
        - **Node.js와의 높은 호환성**으로 백엔드 작업을 수월하게 지원합니다.
- **Google Cloud Platform (GCP)**
    - **장점**:
        - **확장성**: 애플리케이션의 필요에 따라 손쉽게 자원을 확장할 수 있습니다.
        - 다양한 서비스(API, 스토리지, 빅데이터 처리 등)를 제공하여 **복합적인 요구사항에 대응**할 수 있습니다.
        - 보안 기능이 강화된 인프라로, 안정적인 클라우드 서비스를 제공합니다.
- **Google Maps API**
    - **장점**:
        - 사용자가 **실시간으로 지도와 경로를 탐색**할 수 있게 해줍니다.
        - 다양한 지도 기능(거리 계산, 장소 검색 등)을 제공하여 **다양한 위치 기반 서비스를 구현**할 수 있습니다.
- **Google Cloud Speech-to-Text API**
    - **장점**:
        - 음성 인식 기능을 제공하여, 사용자가 **음성으로 서비스를 제어**할 수 있습니다.
        - 다양한 언어 지원으로 글로벌 서비스를 쉽게 확장할 수 있습니다.
        - 높은 정확도의 음성 인식 성능을 제공하여 **자연스러운 사용자 경험**을 보장합니다.

### Design/Tool

- **Figma**
    - **장점**:
        - 팀원 간 **실시간 협업**이 가능하여, 디자인 피드백을 빠르게 반영할 수 있습니다.
        - **프로토타이핑** 기능을 통해 인터랙티브한 UI를 미리 확인할 수 있어 사용자 경험을 개선합니다.
        - 디자인 시스템을 구축하여 일관된 UI 스타일을 유지할 수 있습니다.
- **GitHub**
    - **장점**:
        - **버전 관리**를 통해 코드의 변경 이력을 쉽게 추적할 수 있습니다.
        - **협업 지원**: Pull Request, 코드 리뷰 등을 통해 팀원 간 협업을 효과적으로 지원합니다.
        - GitHub Actions 등 다양한 **CI/CD** 기능을 제공하여, 개발 파이프라인을 자동화할 수 있습니다.

---

### 파일실행법(프로젝트 구조도 + 방안)
![image](https://github.com/user-attachments/assets/448f2871-b5cc-4b7b-83be-696fd57891ca)

https://github.com/orgs/VISIONED-KNU/repositories

1. 상기 링크에서 public과 src 폴더를 local 저장소에 다운로드합니다.
2. IDE의 console 창에서 new project를 생성할 곳으로 이동합니다.
3. npm create vite@latest 입력합니다.
![image](https://github.com/user-attachments/assets/1d629ea2-25dd-4e4d-b949-e1298598ea62)
4. 프로젝트명 입력합니다.
![image](https://github.com/user-attachments/assets/eb3661e4-fad9-4f5d-9ce4-845765c56c19)
5. framwork로 리액트 선택합니다.
![image](https://github.com/user-attachments/assets/fbaffa3f-a32a-42d4-ad07-e815d0aebeaf)
6. Javascript 선택합니다.
![image](https://github.com/user-attachments/assets/08826a6d-ecd3-4849-b6af-be7073a17534)
7. cd (프로젝트명) 입력합니다.
8. npm install
9. npm install react-router-dom
10. npm run dev 입력합니다.
11. 하기와 같이 프로젝트가 생성됩니다.
![image](https://github.com/user-attachments/assets/b5399c55-00c5-4ed3-9ce5-f40330ef11af)
12. 기존의 public과 src 폴더에 있던 파일들 모두 삭제하고 첫번째 단계에서 다운로드한 public과 src 파일들로 대체합니다.
13. 다시 console 창에서 npm run dev입력하면 해당 웹 링크 출력됩니다.
