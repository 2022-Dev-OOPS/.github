# Open API를 이용한 차수 자동화 시스템
### 해당 프로젝트는 K-Hackathon11 참여 영남 예선 200팀 중 영남 본선 14팀 선정 프로젝트인</br> Dev.OOPS!팀의 Open API를 이용한 차수 자동화 시스템 소개 페이지입니다.
![image](https://github.com/user-attachments/assets/addf208f-8c83-44b1-9481-4b4d33a5cde3)
(프로토 타입)
## Youtube 소개 영상
[소개 영상](https://youtu.be/IpPB2t-BAdE)
# 팀원 구성
<div align="center">
  
|<a href="https://github.com/JBumLee"><img src="https://github.com/JBumLee.png" width="100px"><br>이정범</a>|<a href="https://github.com/HyeokBro"><img src="https://github.com/HyeokBro.png" width="100px"><br>신동혁</a> |<a href="https://github.com/GIHng"><img src="https://github.com/GIHng.png" width="100px"><br>현기홍</a> |<a href="https://github.com/junjaehong"><img src="https://github.com/junjaehong.png" width="100px"><br>전재홍</a>|
|-----|-----|-----|----|
|PM, 기획, FE개발, HLS개발|CV개발, IoT개발, RTSP개발|BackEnd개발, HLS개발|BackEnd개발|
|[FE Repo로 이동](https://github.com/2022-Dev-OOPS/Front_End)|[IOT Repo로 이동](https://github.com/2022-Dev-OOPS/IoT), [CV Repo로 이동](https://github.com/2022-Dev-OOPS/CV)|[BE Repo로이동](https://github.com/2022-Dev-OOPS/Back_End)|[BE Repo로이동](https://github.com/2022-Dev-OOPS/Back_End)|
 
</div>

# 프로젝트 개발 배경
2022년 9월 한반도를 강타한 태풍 힌남노는 해안가 지역에 막대한 피해가 예상된 태풍이었다.</br>
특히 2003년 태풍 매미의 최대 피해지 중 하나인 마산시 역시 힌남노 태풍에 큰 피해를 볼 것으로 예상되었다. 하지만 태풍이 끝난 시점에 통계를 낸 결과 마산시는 태풍에 피해가 크지 않았다. 그 이유는 바로 기립식 차수벽이 설치되어 있었기 때문이다. 
기존에 설치되어 있는 차수벽은 해안가에 설치가 되는 것이기 때문에 효과는 우수하지만, 미관을 해친다는 단점이 명확하였다. 그래서 설치된 것이 평시에는 사람이 다니는 길이 되는 기립식 차수벽이다.

2023년 현재 정부는 기립식 차수벽을 핵심 과제로 지정하여 설치를 늘리고 있는 추세이다. 이에 Dev.OOPS!는 마산시 태풍 예방 우수사례인 기립식 차수벽에 단점을 보완한 서비스를 제시한다. 

(+추가) 2024년 현재 부산지역 마린시티에서는 상습적으로 해일에 피해를 입고있지만 미관을 해친다는 이유로 차수벽의 설치를 거절하고 있다. 그렇기에 기립식 차수벽 더 나아가 좀 더 안전한 차수 시스템이 필요할 것이다. 

# 프로젝트 목적
Dev.OOPS!에서 조사한 기존 기립식 차수 시스템의 문제는 다음과 같다.
#### 첫째는 태풍 경보에 대한 반응이 느리다는 문제이다. 
현재의 태풍 경보에 대한 대응과정은 담당자가 차수벽 작동 지시를 받아 직접 동작시켜야 한다는 번거로움이 있다. 심지어 현재 기립식 차수벽은 버튼을 눌러야 작동되며. 이 버튼은 차수벽 제어소마다 설치되어 있으며, 각 제어소는 3KM 간격으로 배치되어 있다. 이는 담당자의 안전과 효율성에 대한 문제를 제시해 볼 수 있다.
#### 둘째는 수동적인 주변 안전 확보이다. 
안전을 위해 안전하지 않은 곳에 사람을 배치해야 한다는 문제가 있다. 앞서 설명했듯이 3KM 간격으로 제어소가 있기 때문에 소수의 사람 배치로는 해결되지 않는 문제이다.
#### (+추가) 마지막으로 동작 확인이다. 
현재는 현장에 있는 사람이 모든 것을 판단하고 동작시켜야 하는 책임이 있다. 

이에 따라 Dev.OOPS!의 서비스 목적은 Open API를 이용한 차수 자동화 시스템 서비스를 제시한다.
# 전체 시스템 아키텍처
![image](https://github.com/user-attachments/assets/929f40f9-b88f-47e8-bbf6-9d1f04c1f8c2)
# 서비스 기능
Dev.OOPS!에서 선정한 서비스 기능들은 다음과 같다.
#### 1. 공공데이터 포털에서 제공하는 Open API를 이용한 기상 확인
#### 2. 해당 기상 정보를 이용하여 각각의 차수벽을 동작시키는 동작
#### 3. 실시간으로 상황을 볼 수 있는 CCTV
#### 4. CCTV를 이용한 신체 인식
#### 5. 신체가 인식될 시 경보
#### 6. 신체를 인식하는 동안도 대시보드에서 볼 수 있는 HLS서버

# 기대효과
서비스 개발시 예상되는 기대효과는 다음과 같다.

#### 1. 차수벽 가동에 필요한 비용 감축
##### Dev.OOPS!의 자동화 시스템을 도입함으로써, 기존 수동적인 차수벽 가동 프로세스에서 인적 자원을 절약할 것을 기대한다. 
- 자동화된 시스템은 자동으로 태풍 예보를 분석하고 차수벽을 가동하므로, 인력에 대한 의존성을 줄이고 비용을 기대한다.

#### 2. 신속한 대응
##### Dev.OOPS!의 자동화 시스템을 도입함으로써, 기존의 수동적인 차수벽 가동 방식에서 담당자가 연락받은 시점에 차수벽을 가동시키는 작업보다 신속하게 대응 할 수 있을 것을 기대한다. 
- 자동화된 시스템은 Open API로부터 실시간으로 데이터를 받아와 자동으로 차수벽을 가동할 수 있다. 이를 통해 보다 신속하게 태풍에 대응할 수 있을 것을 기대한다.

#### 3. 향상된 보고체계
##### Dev.OOPS!의 자동화 시스템을 도함으로써, 기존에는 현장에 있는 사람만이 아닌 지휘층까지 손쉽게 정보 전달이 될 것을 기대한다.
- 대시보드를 통해 태풍 관련 데이터와 정보를 시각화하여 제공한다. 이를 통해 관련 정보를 쉽게 파악할 수 있으며, 실시간으로 상황을 모니터링할 수 있다. 이는 보고체계를 향상시키고 의사 결정에 필요한 정확한 정보를 제공함으로써 태풍 대응 능력을 향상될 것을 기대한다.

##### 최종적으로 Dev.OOPS!에서 개발하는 자동화 시스템은 주변 안전 확보와 관련된 다양한 프로세스에서 활용될 것으로 기대한다. 주변 안전을 보장하고 향상하는 자동화 시스템은 인적 자원을 효율적으로 활용하며, 생산성과 효율성을 향상하는 동시에 안전성을 강화할 수 있다. 이는 사회 전반적인 안전 수준 향상과 함께 4차 산업혁명의 발전에 이바지할 것을 기대한다.


### 아래부터는 프로젝트 이해를 돕기 위한 참고 자료들입니다.
# 실제 애플에서 사용하고 있는 HLS 아키텍처
![image](https://github.com/user-attachments/assets/5d96fcc4-1162-4070-91b4-2825c69b758f)

# Dev.OOPS! 팀의 HLS 아키텍처
![image](https://github.com/user-attachments/assets/25515379-e014-47ea-81a7-aa866fdd7220)

### 프로젝트 회고
서버가 많이 들어간 과제인 만큼 ‘어떻게 동시성을 지원할까?’가 아주 큰 과제였다. </br>
일부에서는 비동기를 지원하는 모델을 사용하였고 일부에서는 순서대로 제한 시간을 걸어 동시성이 있게 보이게도 하였다. </br>
모든 것을 로컬(전시환경 특성상)에서 했기 때문에 더욱 힘들었던 것도 있는 거 같다.</br>
</br>
과제를 진행하면 할수록 설계에 생각했던 동시성보다 실제 동시에 동작해야 하는 것이 많다는 것을 알게 되었다.</br>
특히 Docker의 중요성을 깨달았다. 한가지 기능을 하는 역할에 서버를 컨테이너화 하였다면 조금이라도 비동기를 덜 생각 할 수 있었을텐데</br>
지금와서 생각해보면 RTSP를 도입하는 거보다 WebRTC등을 도입하는 것이 프로젝트 진행에 있어 쉽지않았을까? 라는 아쉬움도 있다.</br>
</br>
그동안 고생해준 팀원들에게 고맙고 앞으로 프로젝트에서 있었던 좋은경험들 힘들었던경험들 잊지 않고 모두 개발자라는 꿈을 위해 화이팅!