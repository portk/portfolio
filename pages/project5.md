## KEPCO Digital Boot Camp Sprint II : 태양광 전력 생산량 예측 서비스 개발
#### 개관
|제목|내용|
|----|----|
|프로젝트명|태양광 전력 생산량 예측 서비스 개발|
|프로젝트에 대한 설명|기상청 API 데이터를 활용한 태양광 전력 생산량 예측 서비스 개발|
|프로젝트 기간 및 규모|2024-01-17 ~ 2024-01-26 (10일) <br> 5명|
|프로젝트 개발 이슈|기상청 api에 있던 위성데이터는 망가져있었고, 날씨 데이터는 이상치와 null값이 혼재해 있었다.|
|프로젝트 결과물·성과|[프로젝트 레포지토리](https://github.com/yoon0718/solar-power-forecast)(제 작업물은 kkh branch에 있습니다)|
||![main1](https://github.com/portk/portfolio/blob/main/images/sunlab_main.png)|
||![main1](https://github.com/portk/portfolio/blob/main/images/sunlab_main2.png)|
||![main1](https://github.com/portk/portfolio/blob/main/images/sunlab_pred1.png)|
||![main1](https://github.com/portk/portfolio/blob/main/images/sunlab_pred2.png)|

#### 구체사항
|항목|내용|
|----|----|
|프로젝트에서 구현한 기능|백엔드: Spring Boot 3 - 일반 데이터(JDBC), Django - 모델<br>딥러닝 모델구축(프론트에 노출x)|
|프로젝트에서 사용한 기술스택|Web : Spring Boot 3, Django<br>tensorflow|
|해당 기술 스택을 사용한 이유|Spring Boot : 프론트 측에서 필요한 정보를 보내줄 수 있는 서버를 구축하기 위해 사용하였습니다<br>Django : Python으로 만들어진 모델을 원활하게 돌리며 모델이 동작할 때 필요한 메모리 확보를 원활하게 하기 위해 분리하여 만들었습니다.<br>tensorflow : 딥러닝 모델을 제작할 때 사용한 라이브러리입니다. 정확하게는 텐서플로우의 Keras를 이용하였습니다.|
|성과|데이터 전송과 모델의 동작 모두 성공적으로 작동하였습니다<br>모델을 만들었었고 20%미만의 상대오차를 보여주었습니다.|
|보완점|모델서버의 경우 모델을 불러와 동작하는 것이 요청 이후 일어나기 때문에 로딩 시간이 다소 발생합니다. 미리 온로드 상태로 대기할 수 있게 하면 더 빠르게 동작할 수 있어보입니다.<br>결과 발송용 데이터를 만드는데 생각보다 오래걸리게 만들어졌습니다. 이것에 대한 최적화가 필요합니다.|
|프로젝트를 수행하며 성장한점 및 느낀점|데이터 전처리는 늘 고난의 행군이라고 느꼈습니다. 전처리에 기간이 절반이상 소요되었습니다.<br>전처리 작업을 하며 최대한 numpy와 pandas를 이용하고, 상황에 따라 데이터를 가져올 때 쿼리문을 가지고 해결하는 것이 가장 빠르다는 것을 느꼈습니다.|

[목록으로](https://github.com/portk/portfolio)
