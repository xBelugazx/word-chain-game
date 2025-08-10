## 사이트 주소 : https://xbelugazx.github.io/word-chain-game/
(수정중)


# 🎮 실시간 끝말잇기 게임 (Real-time Word Chain Game)

친구와 함께 실시간으로 즐길 수 있는 웹 기반 끝말잇기 게임입니다. Firebase를 이용해 실시간 데이터 동기화를 구현했으며, Gemini API를 활용한 AI 힌트 기능을 통해 게임의 재미를 더했습니다.

## ✨ 주요 기능

* **실시간 멀티플레이:** Firebase의 Firestore를 사용하여 두 명의 플레이어가 실시간으로 게임을 즐길 수 있습니다.
* **게임 로비 시스템:** 공개된 방 목록을 보고 참여하거나, 친구와 함께 즐길 비공개 방을 만들 수 있습니다.
* **비밀번호 설정:** 비공개 방을 만들 때 비밀번호를 설정하여 원하는 친구와만 플레이할 수 있습니다.
* **닉네임 기능:** 각자 원하는 닉네임을 설정하여 게임에 참여할 수 있습니다.
* **AI 힌트 기능:** 단어가 생각나지 않을 때 Gemini API를 통해 AI에게 힌트를 얻을 수 있습니다.
* **자동 방 관리:** 방장이 나가거나 마지막 플레이어가 퇴장하면 방이 자동으로 삭제되어 데이터베이스를 깨끗하게 유지합니다.
* **반응형 UI:** PC와 모바일 환경 모두에 최적화된 화면을 제공합니다.

## 🛠️ 사용 기술

* **Frontend:** HTML, Tailwind CSS, JavaScript (ES Modules)
* **Backend & Database:** Google Firebase (Firestore, Authentication)
* **AI:** Google Gemini API

## 🚀 실행 방법

이 프로젝트는 별도의 서버 구축 없이 웹 브라우저에서 바로 실행할 수 있습니다.

1.  **Firebase 프로젝트 설정:**
    * [Firebase 콘솔](https://console.firebase.google.com/)에서 새 프로젝트를 생성합니다.
    * **Authentication** > **Sign-in method**에서 **'익명'** 로그인을 활성화합니다.
    * **Firestore Database**를 **'테스트 모드'**로 생성합니다.
    * 프로젝트 설정에서 웹 앱을 추가하고 `firebaseConfig` 정보를 복사합니다.

2.  **코드에 `firebaseConfig` 적용:**
    * `index.html` 파일 내의 `<script type="module">` 태그 안에서 `firebaseConfig` 변수를 찾아, 위에서 복사한 자신의 프로젝트 정보로 교체합니다.

3.  **실행:**
    * `index.html` 파일을 웹 브라우저에서 엽니다.
    * 또는 [GitHub Pages](https://pages.github.com/)나 [Netlify](https://www.netlify.com/) 같은 정적 호스팅 서비스를 이용해 웹에 배포하여 친구들과 공유할 수 있습니다.
