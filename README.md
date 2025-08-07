<img src="https://capsule-render.vercel.app/api?type=waving&color=0C356A&height=200&text=SKN%20AI%20캠프%2016기%202차%20프로젝트&fontColor=ffffff&fontSize=50" />

## 📌 SKN-AI-16-2 - 당원 이탈 예측 프로젝트

🧪 본 프로젝트는 가상의 당원 데이터를 활용하여,  
머신러닝 ,딥러닝기법을 통해 이탈 여부를 예측하고  
그 과정에서 데이터 분석 및 모델링 전반을 실습하며 학습하는 것을 목표로 하였습니다.

## 👥 팀원 소개

<table>
  <tr align="center">
    <td><img src="https://raw.githubusercontent.com/sang-won-Park05/SKN-AI-16-2-/main/images/김민정.png" width="100"/></td>
    <td><img src="https://raw.githubusercontent.com/sang-won-Park05/SKN-AI-16-2-/main/images/박상원.jpeg" width="100"/></td>
    <td><img src="https://raw.githubusercontent.com/sang-won-Park05/SKN-AI-16-2-/main/images/신희석.png" width="100"/></td>
    <td><img src="https://raw.githubusercontent.com/sang-won-Park05/SKN-AI-16-2-/main/images/안주영.png" width="100"/></td>
    <td><img src="https://raw.githubusercontent.com/sang-won-Park05/SKN-AI-16-2-/main/images/원태식.png" width="100"/></td>
  </tr>
  <tr align="center">
    <td>김민정</td>
    <td>박상원</td>
    <td>신희석</td>
    <td>안주영</td>
    <td>원태식</td>
  </tr>
</table>

## 📅 업무 분담 일정표

| 8월 항목       | 1일(오전) | 1일(오후) | 2일(오전) | 2일(오후) | 3일(오전) | 3일(오후) | 4일(오전) | 4일(오후) | 5일(오전) | 5일(오후) | 6일(오전) |
|----------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
| 도메인 분석    | ✅        | ✅        |     ✅       |     ✅       |           |           |           |           |           |           |           |
| 데이터 분석    |           |           | ✅        | ✅        | ✅        |     ✅       |           |           |           |           |           |
| 모델 분석      |           |           |     ✅       |     ✅       | ✅        | ✅        | ✅        |         |         |         |         |
| 설계           |           |           |           |      ✅      |      ✅      |      ✅      |      ✅       |            |            |            |           |
| 개발           |           |           |           |           |           |           |           |     ✅       |      ✅      |     ✅       |           |
| 테스트         |           |           |           |           |           |           |           |           |           |     ✅       |     ✅       |


## 🔍 프로젝트 필요성 (배경)

조직(정당 또는 커뮤니티)에서는 당원의 유지율이 핵심 운영 지표가 됩니다.
그러나 많은 경우, 당원이 이탈하는 이유는 다양한 변수의 복합적인 영향으로 나타나며,
이를 사전에 예측하기 어렵습니다.
본 프로젝트는 이러한 문제를 데이터 기반으로 접근하여,
이탈 가능성이 높은 당원을 사전에 식별할 수 있는 예측 모델을 개발하고자 합니다.

## 🎯 프로젝트 목표

당원의 다양한 특성(소득, 직업, 가입기간 등)을 기반으로 이탈 여부 예측 모델 구축

머신러닝 기반 모델(CatBoost, XGBoost 등) 간의 성능 비교 및 최적화

피처 중요도 분석을 통해 주요 이탈 요인 도출

분석 결과를 통해 조직 유지율 향상을 위한 인사이트 제공


## 📄 데이터셋 정보
| No. | Column Name           | Non-Null Count | Dtype  | 설명 (선택)                           |
| --- | --------------------- | -------------- | ------ | --------------------------------- |
| 0   | MemberID              | 10000          | object | 회원 고유 ID                          |
| 1   | Age                   | 10000          | int64  | 나이                                |
| 2   | Gender                | 10000          | object | 성별                                |
| 3   | Region                | 10000          | object | 지역                                |
| 4   | Education             | 10000          | object | 교육 수준                             |
| 5   | Occupation            | 10000          | object | 직업                                |
| 6   | Income\_Decile        | 10000          | int64  | 소득 분위 (1\~10)                     |
| 7   | Income                | 10000          | object | 소득 범주                             |
| 8   | MembershipDuration    | 10000          | int64  | 가입 기간                             |
| 9   | MembershipType        | 10000          | object | 회원 유형                             |
| 10  | Primary\_Support      | 10000          | object | 주요 지지 정책                          |
| 11  | PoliticalActivity     | 10000          | int64  | 정치 활동 수준                          |
| 12  | PartyLoyalty          | 10000          | int64  | 당 충성도                             |
| 13  | PresidentApproval     | 10000          | int64  | 대통령 지지율                           |
| 14  | PolicySatisfaction    | 10000          | int64  | 정책 만족도                            |
| 15  | MediaConsumption      | 10000          | object | 주요 미디어 소비 채널                      |
| 16  | EventImpact           | 10000          | int64  | 특정 이벤트 영향 점수                      |
| 17  | PartyParticipation    | 10000          | int64  | 당 활동 참여 점수                        |
| 18  | FinancialContribution | 10000          | int64  | 정치 후원금                            |
| 19  | Churn                 | 10000          | int64  | 이탈 여부 (1 = 이탈)                    |
| 20  | **Date**              | 10000          | object | **데이터 수집 월 (2024-01 \~ 2025-07)** |


## 📊 수치형 변수 통계 요약
| 변수명                   | count   | mean    | std      | min  | 25%  | 50%  | 75%  | max    |
| --------------------- | ------- | ------- | -------- | ---- | ---- | ---- | ---- | ------ |
| Age                   | 10000.0 | 52.0493 | 16.8700  | 20.0 | 40.0 | 52.0 | 64.0 | 87.0   |
| Income\_Decile        | 10000.0 | 5.2784  | 2.5875   | 1.0  | 3.0  | 5.0  | 7.0  | 10.0   |
| MembershipDuration    | 10000.0 | 58.4032 | 60.4636  | 1.0  | 12.0 | 34.0 | 91.0 | 239.0  |
| PoliticalActivity     | 10000.0 | 2.2028  | 1.1335   | 1.0  | 1.0  | 2.0  | 3.0  | 5.0    |
| PartyLoyalty          | 10000.0 | 3.5716  | 0.8470   | 1.0  | 3.0  | 4.0  | 4.0  | 5.0    |
| PresidentApproval     | 10000.0 | 2.3837  | 1.0874   | 1.0  | 2.0  | 2.0  | 3.0  | 5.0    |
| PolicySatisfaction    | 10000.0 | 3.1481  | 0.7716   | 1.0  | 3.0  | 3.0  | 4.0  | 5.0    |
| EventImpact           | 10000.0 | 3.6861  | 1.0676   | 1.0  | 3.0  | 4.0  | 5.0  | 5.0    |
| PartyParticipation    | 10000.0 | 2.3022  | 1.3004   | 0.0  | 1.0  | 2.0  | 3.0  | 7.0    |
| FinancialContribution | 10000.0 | 54.5811 | 158.5193 | 0.0  | 0.0  | 5.0  | 45.0 | 2700.0 |
| Churn                 | 10000.0 | 0.4925  | 0.5000   | 0.0  | 0.0  | 0.0  | 1.0  | 1.0    |



