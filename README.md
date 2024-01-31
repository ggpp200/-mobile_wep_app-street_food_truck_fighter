# 🚚 Street Foodtruck Fighter

푸드트럭을 쉽게 접근할 수 있는 서비스

![스푸파](https://user-images.githubusercontent.com/99133426/202908973-43099654-321b-499e-b24d-fb48b61a23ea.png)

## 🍔 서비스 소개

**Street Foodtruck Fighter**는 사업자와 사용자를 구별하여 제작이 되었습니다.  
위치와 영업시간의 정보가 잘 등록되어 있는 가게들과는 달리, 유동적인 영업 위치와 영업시간 때문에 정보가 부족해 쉽게 소통하지 못한 사업자와 사용자 간에 불편함을 해소하고자 하는 서비스입니다.
1. **사업자**는 자신의 푸드트럭과 메뉴를 쉽게 등록할 수 있고, **스케줄 관리**와 **영업 시작/종료 기능**, **주문 접수 및 결제** 등 영업에 필요한 기능들을 제공합니다. 또, 푸드트럭 영업할 위치를 고민하는 사업자들을 위해서 **원해요 푸드트럭**을 통해서 어느 지역에서 무슨 음식을 선호하는지 확인할 수 있는 정보도 제공합니다.  
2. **사용자**는 자신의 위치 근방에 있는 푸드트럭을 **지도**를 통해서 **쉽게 찾아볼 수** 있고, 스푸파를 통해 **미리 주문을 하고 결제**를 함으로써 **웨이팅**에 대한 걱정을 줄여줍니다. 그리고 우리 지역에 왔으면 하는 푸드트럭을 **원해요 푸드트럭** 설문 조사를 통해서 사업자들이 확인할 수 있게 도와줍니다.

## 🍕 프로젝트 멤버

### BE

윤일준(팀장)

박범수

이주희

### FE

안태환(파트장)

이성훈

박승주

## ⏱ 프로젝트 진행 기간


> 22/10/10 ~ 22/11/25

## 🛠 기술 스택

### 클라이언트

- Vue 3.2.13
- JavaScript 
- jQuery 3.6.1
- Axios 1.1.3
- Pinia 2.0.23
- Fullcalender 5.11.2
- Chart.js 3.9.1
- Splide.js 0.6.12

### 백엔드

- Java 1.8
- Spring Boot 2.7.4
- Spring Date JPA 2.7.4
- Spring Security 2.7.4
- Swagger2 3.0.0
- MySQL 8.0.31
- Redis 5.0.7

### 인프라

- AWS EC2 ubuntu : 20.04 LTS
- Docker 20.10.20
- Jenkins image : jenkins/jenkins:lts
- NGINX image : stable-alpine

## 🍖 주요 기능

| 기능                  | 내용                                                         |
| --------------------- | :----------------------------------------------------------- |
| 푸드트럭 정보 제공     | **내 주변에 위치한 푸드트럭의 정보를 제공합니다.**<br /><br />사업자들이 스케줄 관리에 등록해 놓은 정보를 토대로 사용자들은 지도를 통해서 내 주변 푸드트럭들을 쉽게 조회할 수 있습니다. 또, 푸드트럭 조회 간에 음식별 카테고리를 통해서 내가 원하는 푸드트럭만 확인할 수 있는 필터링 기능이 있습니다. |
| 주문 및 결제 시스템    | **스푸파를 통해 주문 및 결제 시스템을 제공합니다.**<br /><br />사용자가 주문하고자 하는 푸드트럭에서 메뉴들을 주문을 하고 카카오페이를 통해서 쉽게 결제를 할 수 있습니다. 해당 푸드트럭 사업자가 주문 수락을 하면 음식 완료 시간을 사용자에게 보내주는데, 음식 완료 시간에 음식을 수령하러 가게 된다면 푸드트럭의 긴 줄에서 더 이상 웨이팅을 하지 않아도 됩니다. |
| 설문 조사             | **원해요 푸드트럭을 통해 수요조사를 할 수 있습니다.**<br /><br />사용자는 현재 위치한 위도, 경도 좌표를 통해서 "원해요 푸드트럭" 설문 조사를 할 수 있습니다. 설문조사에는 여러 음식 카테고리들이 있어 카테고리를 선택하고 설문조사를 완료하게 된다면, 사업자들은 설문 조사 통계를 통해서 어느 지역에서 영업하면 좋을지 참고할 수 있는 정보를 제공해 줍니다. |
| 스케줄 관리           | **영업시간 스케줄을 관리할 수 있습니다.**<br /><br />사업자는 언제, 어디에서 몇 시부터 몇 시까지 영업을 할지 스케줄 관리 탭에서 영업 기간을 등록할 수 있습니다. 사용자들은 사업자가 스케줄을 등록해놓은 정보를 통해 푸드트럭을 쉽게 이용할 수 있습니다.  |
| 매출 통계 확인        | **오늘의 매출과 일자별 매출을 확인할 수 있습니다.**<br /><br />매출 통계 페이지에서는 오늘 하루 판매한 메뉴들과 수입을 확인할 수 있습니다. 일자별로도 매출 확인을 할 수 있는데, 달력을 통해서 날짜를 선택하면 선택한 날에 해당하는 매출을 확인할 수 있습니다. |

## 🍤 주요 기능

### 사용자
- 메인화면

![사용자 메인화면](https://user-images.githubusercontent.com/99133426/202927894-b803b711-c51c-43f9-8d16-c4febd878597.png)

- 내 주변 푸드트럭 찾기

![내 주변 푸드트럭](https://user-images.githubusercontent.com/99133426/202927991-9b4bbc10-6aa7-4c85-936e-4f4a597a41b2.png)

![푸드트럭 찾기](https://user-images.githubusercontent.com/99133426/202928825-7c6fe4b0-a652-4481-b1f2-a8da07f6a188.png)

- 주문하기

![주문하기1](https://user-images.githubusercontent.com/99133426/202929102-61fc011f-b08c-4073-a2e7-8cad9c194497.png)

![주문하기2](https://user-images.githubusercontent.com/99133426/202929101-8162f86e-2ec9-48bf-9469-4932db2471ec.png)

![주문하기3](https://user-images.githubusercontent.com/99133426/202929099-feb40dc9-abba-4833-a056-363541b47d81.png)

![주문하기4](https://user-images.githubusercontent.com/99133426/202929098-56fb4d2d-e366-41a2-ac8b-f15756ac5f20.png)

- 원해요 푸드트럭

![원해요 푸드트럭 사용자](https://user-images.githubusercontent.com/99133426/202928023-74266b7f-847c-4409-9a5d-8b076059113b.png)

### 사업자
- 메인화면

![사업자 메인화면](https://user-images.githubusercontent.com/99133426/202927863-a5bae8cc-50c4-4ea9-bbda-1510756ab91d.png)

- 매출통계

![매출통계](https://user-images.githubusercontent.com/99133426/202928074-d5e50674-8f73-406c-8958-8beb51f29414.png)

![매출통계2](https://user-images.githubusercontent.com/99133426/202934934-fbf3f415-8dbe-48f5-be30-46ad826753ef.png)

- 스케줄 관리

![스케줄 등록](https://user-images.githubusercontent.com/99133426/202928106-9e6dd738-54d7-4f5e-9293-98b69c3f3021.png)

- 수요조사

![수요조사 확인](https://user-images.githubusercontent.com/99133426/202934910-482b85b5-99a3-426b-b882-c67c6376aea2.png)

- 마이푸드트럭

![마이푸드트럭 등록](https://user-images.githubusercontent.com/99133426/202928167-c1c5d94e-ff8b-4d07-9ad5-026e1fc0a34e.png)

![메뉴 등록](https://user-images.githubusercontent.com/99133426/202928171-eb706aab-8abf-4ab7-83f5-1b56bed2be13.png)

## 📚 산출물

[와이어 프레임](https://www.figma.com/file/5wfH0Qpq21ki0rBAyIyi5A/%EC%8A%A4%ED%8A%B8%EB%A6%AC%ED%8A%B8-%ED%91%B8%EB%93%9C%ED%8A%B8%EB%9F%AD-%ED%8C%8C%EC%9D%B4%ED%84%B0_B206_%EC%9E%90%EC%9C%A8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8?node-id=0%3A1&t=PTcmkGYpTGvPth2h-0)  
  
[기능명세서](https://www.notion.so/3a665dc16e5942219d083fd0e053c76e)  
  
[ERD](https://www.erdcloud.com/d/wkHDpQmGCtkvGzMZQ)  

[API 명세서](https://k7b206.p.ssafy.io/api/swagger-ui/)  

## 💻 시스템 아키텍처

![스푸파 아키텍처](https://user-images.githubusercontent.com/99133426/202916867-defbf547-6ac6-48cc-91dc-f075727933b0.png)
