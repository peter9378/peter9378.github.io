-

# aws에서 amplify를 통해 github과 연동된 react 빌드 환경 구축하기
1. `AWS Amplify`서비스 콘솔로 이동한다.
1. Deliver 하위의 Get started를 클릭한다.
![image](https://user-images.githubusercontent.com/13210889/107113666-bb85d400-68a3-11eb-92e0-3c8fcbdac510.png)
- 공식 설명서에는 deploy 하위의 GET STARTED를 선택하라고 나온다(`2021-02-06` 기준).
- 현재는 업데이트되었는지 Deliver 하위를 선택해야 한다.
1. GitHub를 선택 후 Continue
![image](https://user-images.githubusercontent.com/13210889/107113720-11f31280-68a4-11eb-8d8d-36cf452fb62f.png)
1. github 계정 인증
![image](https://user-images.githubusercontent.com/13210889/107113757-4f57a000-68a4-11eb-8ec3-e5f2bccd4315.png)
1. 연동할 repository와 branch를 선택하고 다음 클릭
![image](https://user-images.githubusercontent.com/13210889/107113782-8037d500-68a4-11eb-84ee-18144d984052.png)
1. 빌드 설정에 수정할 항목이 있으면 수정해도 좋다. 일단 기본 빌드 설정을 사용해서 진행
![image](https://user-images.githubusercontent.com/13210889/107113807-a52c4800-68a4-11eb-82c3-e6cdbbfd4711.png)
1. 설정을 다시 한번 확인 후 `저장 및 배포` 클릭
![image](https://user-images.githubusercontent.com/13210889/107113819-c2611680-68a4-11eb-9fd5-6781c35f0685.png)
    - 성격이 급해서 이미 눌러버려따
1. 빌드가 완료되면 다음 링크에서 확인할 수 있다.
![image](https://user-images.githubusercontent.com/13210889/107113876-2a176180-68a5-11eb-8907-68777903b6b3.png)




출처 및 참고: https://aws.amazon.com/ko/getting-started/hands-on/build-react-app-amplify-graphql/module-one/?e=gs2020&p=build-a-react-app-intro
