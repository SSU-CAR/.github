# 안전운전 피드백 서비스
### 현대모비스 2024 Mobility SW HACKATHON 
> **2024.01.18~2024.02.23**
> 
> Frontend [@jwo0o0](https://github.com/jwo0o0) Backend [@0woogie](https://github.com/0woogie) [@Seohyun Back](https://github.com/Seohyun-Back) Embedded[
@byungjikim](https://github.com/byungjikim)

## 프로젝트 소개

전방 주시 태만을 비롯한 안전운전 불이행은 교통사고의 주 원인이다.<br>
또한, 현재 상용화된 자율주행 레벨2, 레벨3에서 운전자는 여전히 시스템의 직접 운전 요구에 대응해야 할 의무가 있다. <br>
따라서 <b>사용자의 안전운전을 위해 운전 습관을 피드백해주는 모빌리티 SW를 기획</b>하였다.<br> 

차량 센서와 내부 카메라로 <b>차량 내/외부의 위험한 운전 상황과 운전자 자세 (e.g. 실선에서의 차선변경, 전방 주시 태만 등)를 감지</b>한다. <br>
이 데이터를 바탕으로 <b>운전 점수를 산정하고, 주행 리포트를 제공</b>한다. <br>
추가적으로 다양한 운전 배지 획득을 통해 안전 운전에 대한 성취감과 동기 부여를 제공하는 모바일 웹 서비스를 기획했다. 

<img width="600" alt="img1" src="https://github.com/SSU-CAR/.github/assets/70098708/44b829cc-cd47-434a-b9f5-b22f7da318bf">

<img width="600" alt="img2" src="https://github.com/SSU-CAR/.github/assets/70098708/3a59922c-b9fa-4486-9a1c-ba1d0b5401ff">

## 화면 구성 및 기능

### 시연 영상
https://github.com/SSU-CAR/.github/assets/70098708/da9842e9-05d1-4aa0-b273-bea88a6baa1e



## Stacks
### Front
<img src="https://img.shields.io/badge/Typescript-3178C6?style=flat&logo=typescript&logoColor=white"/> <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=white"/> <img src="https://img.shields.io/badge/chart.js-FF6384?style=flat&logo=chartdotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Styled Components-DB7093?style=flat&logo=styled-components&logoColor=white"/> <img src="https://img.shields.io/badge/S3-569A31?style=flat&logo=amazons3&logoColor=white"/>
<img src="https://img.shields.io/badge/GithubActions-2088FF?style=flat&logo=githubactions&logoColor=white"/> 
### Back

### Embedded
![ROS2](https://img.shields.io/badge/ros-foxy-444444?style=flat&logo=ros)
![Python](https://img.shields.io/badge/Python-444444?style=flat&logo=Python)
![Docker](https://img.shields.io/badge/Docker-444444?style=flat&logo=Docker)
![C++](https://img.shields.io/badge/C++-444444?style=flat&logo=c%2B%2B)
![Python](https://img.shields.io/badge/Python-444444?style=flat&logo=Python)

## 상황 판단 알고리즘 구현
#### Detail information in this link: [Here](https://github.com/SSU-CAR/SSU-CAR_Embeded)
Monitor the driver's forward attention by pupil, head pose and phone detection.  
Three evaluation factors - Closed eye detection, Head pose estimation, Phone detection    
![image](https://github.com/SSU-CAR/SSU-CAR_Embeded/assets/107911398/3e5b8ff1-3ff0-49f1-a111-0ddbeedbca80)  
Monitor the illegal lane change like changing in solid line and without direction light.  

DrivenDist - Report driving distance and current veloicity.  
Joystick_usb - Control RC car with joystick.  
LaeDetection, lane_ex - Lane detetction with HSV(HSL) filtering.  
![image](https://github.com/SSU-CAR/SSU-CAR_Embeded/assets/107911398/f5f10145-ed10-4ec9-9722-8f5671cca517)

## 트러블 슈팅
