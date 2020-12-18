---
layout: post
title:  "구글 API 사용하기 (Google Cloud Platform 사용하기)"
date:   2017-01-30 00:39:36 +0900
---

https://console.cloud.google.com/

위 링크를 따라가면 구글 api를 사용할 수 있는 Google Cloud Platform 페이지가 열린다.

![image](https://user-images.githubusercontent.com/13210889/101986432-2914ea00-3cd1-11eb-9555-90a4db4ab4ee.png)

로그인 후 좌측 상단의 메뉴 버튼(가로로 세줄)을 누르시면 위 화면과 같은 창이 뜬다.

좌측 메뉴 중에서 `결제` 카테고리 클릭 후 무료 체험 비슷한 걸 신청하면 된다.

Google Cloud Platform 사용 권한을 얻었다면 이제 사용할 api를 선택해보자.

좌측 메뉴에서 API 관리자를 클릭

![image](https://user-images.githubusercontent.com/13210889/101986483-65e0e100-3cd1-11eb-9830-fbcb024764f7.png)

클릭 후 형광펜 칠한 `API 사용 설정` 을 클릭

![image](https://user-images.githubusercontent.com/13210889/101986497-73966680-3cd1-11eb-95e6-dc9ba916e074.png)

사용하려는 API 관련 키워드를 입력하고 검색하여 사용하려는 API를 클릭

필자의 경우는 Speech 관련 API를 사용하기 위해서 speech를 검색하여 Google Cloud Speech API를 클릭했다.

![image](https://user-images.githubusercontent.com/13210889/101986520-96287f80-3cd1-11eb-9b09-eb20a8f0e763.png)

필자는이미 해당 API를 사용중이기 때문에 위 화면과 같이 나타나지만, 사용 전에는 `사용` 같은 버튼이 있었다.

그걸 클릭하면 위 화면처럼 바뀌고, 해당 계정에서 선택한 API를 사용할 수 있게 된다.

*한가지 중요한 점은, API를 사용하기 전에

![image](https://user-images.githubusercontent.com/13210889/101986541-ba845c00-3cd1-11eb-9856-06478a664d48.png)

미리 만들어 놓은 프로젝트에 한해서만 선택한 API 사용 권한이 적용된다는 점이다.

![image](https://user-images.githubusercontent.com/13210889/101986575-f3243580-3cd1-11eb-8eb9-c0a62cdce64f.png)

이제 다시 API 관리자로 돌아와서, 형광색칠 된 `사용자 인증 정보`를 클릭

![image](https://user-images.githubusercontent.com/13210889/101986585-046d4200-3cd2-11eb-9b5e-5a06c60a6a51.png)

그리고 `사용자 인증 정보 만들기` 를 클릭

이 '사용자 인증 정보' 는 json 파일로 이루어진, 개발자가 구글 api를 사용하기 위한 권한을 인증해주는 파일의 정보 라고 이해면 쉽다.

![image](https://user-images.githubusercontent.com/13210889/101986601-1ea72000-3cd2-11eb-8d61-f08607471307.png)

`서비스 계정 키` 를 선택

![image](https://user-images.githubusercontent.com/13210889/101986606-2961b500-3cd2-11eb-86f7-c96337d15277.png)

서비스 계정 이름을 설정하고(사용자 임의), 역할은 개발에 필요한 옵션을 선택하시면 되자만, 가급적 `소유자`를 선택하는 것이 편하다. 물론 필수는 아니다.

키 유형은 json파일을 추천한다. 

이제 `생성` 버튼을 클릭하면

![image](https://user-images.githubusercontent.com/13210889/101986648-662dac00-3cd2-11eb-9c75-62e45e39dc41.png)

다음과 같은 팝업이 뜬다. 디폴트 다운로드 경로로 json파일이 저장된다. 

이제 해당 json파일을 `GOOGLE_APPLICATION_CREDENTIALS` 환경변수로 지정하여 인증하면 선택한 구글 API를 사용할 수 있다.

여기까지 구글 api 사용을 위한 간단한 과정을 소개했다.

-----

### 2020-12-12 업데이트
블로그 이사를 준비하며 UI가 옛날로 되어있다는 걸 깨닫고 최신 글을 다시 업데이트 해야겠다고 느꼈다. 하지만 혹시 모르니(히스토리 차원에서라도) 기존 글은 유지할 생각이다.

