# care_system_for_elder
care system with embedded software for elder who lives alone

# - 개요
 갈수록 대두되는 고령화 문제에 의해 매년 늘어나는 독거노인과 이에 따른 사고사에 효율적으로 대비하기 위하여 독거노인 케어 시스템을 개발하였다. 해결하고자 한 주요 문제는 노인분들의 열사병 및 저체온증과 같은 체온으로 인한 사고예방, 실족사 예방 그리고 고독사 감지이다.

# - 구성 및 개발환경
## 하드웨어 구성
- Arduino UNO

- Raspberry pi 3b+

- sensors(TMP36, MPU-6050, GY-NEO6MV2)

## 개발환경
| <center>Language</center> | <center>FrameWork</center> | <center>Tool</center> |
|:--------:|:--------:|:--------:|
| C, Python | OpenCV, SMTPlib | Raspbian, Visual Studio 2015, Visual Studio Code, Arduino IDE |

# HW 구성도
![hw 구성도](https://user-images.githubusercontent.com/48172859/70374833-906bc180-193a-11ea-8394-1b4911822483.png)

# SW 알고리즘 흐름도
![sw 알고리즘](https://user-images.githubusercontent.com/48172859/70374856-db85d480-193a-11ea-81f1-a5ce261c3b71.png)

# 기능
## 스마트 지팡이

- [체온 감지 기능](https://github.com/artiiicy/Care_system_for_elder/blob/master/README.md#%EC%B2%B4%EC%98%A8-%EA%B0%90%EC%A7%80-%EA%B8%B0%EB%8A%A5)

- [쓰러짐 감지 기능](https://github.com/artiiicy/Care_system_for_elder#%EC%93%B0%EB%9F%AC%EC%A7%90-%EA%B0%90%EC%A7%80-%EA%B8%B0%EB%8A%A5)

- [안심 귀가 서비스](https://github.com/artiiicy/Care_system_for_elder#%EC%93%B0%EB%9F%AC%EC%A7%90-%EA%B0%90%EC%A7%80-%EA%B8%B0%EB%8A%A5)

## 스마트 카메라

- [고독사 감지 기능](https://github.com/artiiicy/Dictionary_using_IDF/blob/master/README.md#고독사감지기능)

-----

### 체온 감지 기능
사용자의 체온을 매 초마다 실시간으로 감지한다. 5분 동안의 체온 데이터를 모아서 평균을 내고, 그 값을 정상 체온과 비교하여 사용자가 현재 안전한 상태에 있는지 판단한다. 현 프로그램에서는 임의로 사용자 평균 체온이 38.5도 이상 혹은 35도 미만이면 사용자가 위험한 상태에 있다고 판단하여 사용자에게 위험 감지 문자를 발송한다. 문자가 발송된지 10분이 지나도 사용자의 체온이 여전히 위험한 상태에 있다면 사용자의 가족에게도 연락을 취하도록 하였다.

### 쓰러짐 감지 기능


### 안심 귀가 서비스

### 고독사 감지 기능
