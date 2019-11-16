---
title: "preonic 언박싱, 조립"
permalink: /docs/preonic/assembly/
excerpt: ""
last_modified_at: 2019-11-14T23:00:00
# redirect_from:
#   - /docs/intro/
toc: true
---
<br>이 문서에서는 최초 조립 과정을 나열해보았다.<br>

### 1. Shipping<br>
[mass drop](https://drop.com/buy/preonic-mechanical-keyboard)에서 구입한 preonic 키보드가 드디어 도착했다.<br><br>
키보드의 재고가 미국에 쌓여 있고<br>
한국으로 직접 배달을 시킬 수 있다.<br>
문제는 배달비가 만원 이하로 붙는데,<br>
배로 오기 때문이다...<br>
그런고로 주문한 후 오랜기간이 지나서야 도착하였다.<br><br>
그래도 지금은 상황이 나은 편이다.<br>
같은 키보드를 2019년 4월에 먼저 주문 했었는데,<br>
프로젝트 시작 초창기라 9월이 도착 예정이었고<br>
실제로는 10월 중순에야 왔다.<br>
프로젝트가 매니아층 사이에서는 아주 흥한 편이기 때문에<br>
[OLKB 홈페이지](https://olkb.com/)에서도 쉽게 구할 수 있을 것이다.<br><br>
조립과정은 유튜브에도 자료가 아주 많다.<br> 
대부분 영어라는 점이 걸리는 사용자도 많겠지만<br> 
요는 별로 어렵지 않으며 누구나 할 수 있고<br> 
그러므로 그리 중요한 내용은 아니다.<br><br>
대신 다른 문서에서 다룰 qmk 오픈소스 펌웨어 프로젝트가<br>
이 커스텀 키보드 프로젝트의 핵심이다.<br><br>
아래의 기록에서 보다시피 tracking에 3주가 넘는 내용이 남아있고,<br> 
특히 항구에서 출발한 후로는 아무 소식 없이 열흘이 걸렸다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68869872-3a419f00-073d-11ea-89d2-7ff627c01892.png)<br><br>
기다림 끝에 심플하게 생긴 택배물이 찾아왔다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866640-17f95280-0738-11ea-94df-e752e3823cc1.jpg)<br><br>
### 2. 구성
preonic 프로젝트에 대한 전반적인 느낌은 정갈하다는 것이다.<br>
키보드 모양은 목적에 따라 명확하고<br>
부품들도 정밀하면서 간단하고<br>   
박스마저 정직하다.<br>
굳이 화려한 데코레이션을 추가할 생각을 안한 것이 마음에 든다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866641-17f95280-0738-11ea-94ce-38c31b72d8f7.jpg){:height="400px" width="300px"}<br><br>
![](https://user-images.githubusercontent.com/55048882/68866642-17f95280-0738-11ea-8efb-e47c246b71e2.jpg){:height="400px" width="300px"}<br><br>
간단한 매뉴얼이 동봉되어 있고<br>
그것만 정확히 따라해도 문제 없이 조립할 수 있다.<br><br>
이번에 받은 택배구성은 다음과 같다.<br>
그리고 '이번에'라고 말하는 이유는<br>
mass drop에서 preonic이 올 때마다 구성이 상이하게 달랐기 때문이다.  
이번엔 키보드 보관용 백이 없는게 아주 아쉬웠다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866644-1891e900-0738-11ea-8904-246c86856d8c.jpg)<br><br>
- 스위치 플레이트 (MIT Top Plate)
- 스크류, 너트 등등
- 키캡
- 받침판
- 연결선
- PCB
<br>
부품들 중 가장 중요한 것은 역시 검은 봉투에 쌓여있는 PCB 기판이다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866645-1891e900-0738-11ea-9575-e8eae545f805.jpg)<br><br>
[olkb 홈페이지](https://olkb.com/group-buys)에서 볼 수 있듯이 PCB만 따로 팔기도 하는데,<br> 
프로젝트 자체가 사실상 순수하게 이 PCB 기판에 관한 것이라 볼 수도 있다.<br>
mass drop에서 살 때도 다른 모든 부품은 제외하고 PCB만 살 수도 있다.<br>
이는 키보드의 가장 핵심이 되는 부분 외에는<br>
모두 customize할 수 있도록 하는 목적을 잘 보여주며,<br> 
그 외 키캡 등등 디자인들은 리뷰어와 커뮤니티의 반응에 따라 계속 바뀌고 있기도 하다.<br><br>
부품 사진을 보면 또다른 중요한 항목인 스위치가 빠졌다는 것을 볼 수 있다.<br> 
Mass drop에서 주문 할 때 옵션으로 선택할 수 있었는데,<br> 
지난번의 제품에서 왔던 적축이 내게는 너무 무겁게 느껴져서 그냥 주문하지 않았다.<br> 
대신 따로 국내에서 미리 저소움 백축(키압 30g) 체리 MX 스위치를 주문해 놓은 상태였다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866646-1891e900-0738-11ea-9925-36a747911371.jpg)<br><br>
PCB의 설계상 최대한 많은 종류의 기계식 스위치에 대해서<br>
모두 인터페이스가 가능하도록 되어있다.<br>
그래서 구멍이 아주 많다.<br>
기본적인 체리/가테론/카일 스위치는 당연히 쓸 수 있고,<br>
그 외 납땜이 필요한 모델에 대해서도 고려해놓았다.<br>
아마 점점 더 다양한 모델을 받아들일 수 있도록 넓히지 않을까 싶다.<br><br>

### 3. 조립<br><br>
- 방향<br><br>
![](https://user-images.githubusercontent.com/55048882/68866647-1891e900-0738-11ea-9c43-5138ed6b9bd6.jpg)<br><br>
위와 같이 방향이 있음을 확인해본다. usb를 꼽을 위치가 뒤로 가면 되고, PCB 및 플레이트는 12x5의 구성인데, 플레이트는 스페이스 바를 두 개 쓸 수 있도록 하려고 스테빌라이저를 꼽을 수 있게 길쭉하게 구멍이 뚫려있다. 내 경우는 스페이스 하나 즉, 2개의 범위에 대해서만 세팅하였다.<br><br>
- 받침+PCB<br><br>
![](https://user-images.githubusercontent.com/55048882/68866649-192a7f80-0738-11ea-91aa-a3b1de97081d.jpg)<br><br>
스크류와 너트를 이용해 PCB와 받침을 합체시킨다.<br><br>
- PCB+플레이트<br><br>
![](https://user-images.githubusercontent.com/55048882/68866651-192a7f80-0738-11ea-9349-0880af4d7e7e.jpg)<br><br>
플레이트를 위에 올린다. <br>
그런데 이렇게 조립해버리면<br> 
횡으로 공간을 넓게 차지하는 스테빌라이저를 꽂지 못하는 구조로 되어있다.<br>
매뉴얼에 정확하게 나오지 않아 많은 사람들이 시행착오를 겪을 부분이다.<br>
따라서 아래와 같이 스테빌라이저를 먼저 설치해야한다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866652-19c31600-0738-11ea-8800-051f6160ff8a.jpg)<br><br>
![](https://user-images.githubusercontent.com/55048882/68866653-19c31600-0738-11ea-9db7-0c9ad2566d54.jpg)<br><br>
위와 같이 세팅하고 플레이트도 알맞은 너트로 조여주면 사실상 조립은 완료다.<br><br>
### 4. 스위치 결합<br>
자세히 플레이트 사이를 보면, 격자가 정확하게 한 스위치를 꼽을 수 있도록 설계되어 있음을 볼 수 있다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866654-19c31600-0738-11ea-86c5-d565e2f33730.jpg)<br><br>
그 사이사이에 스위치를 잘 꽂아 넣으면 된다. 사실 플레이트는 무게도 무겁고 preonic에 기능적으로 꼭 필요한 것이 아니다. 그럼에도 들어있는 이유는 스위치를 잘 설치하고 고정해주는 헬퍼 역할을 하고 있기 때문이다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866656-1a5bac80-0738-11ea-9ee4-3123523565c4.jpg){:height="400px" width="300px"}<br><br>
![](https://user-images.githubusercontent.com/55048882/68866655-19c31600-0738-11ea-90ad-5ac249db8d6f.jpg){:height="400px" width="300px"}<br><br>
![](https://user-images.githubusercontent.com/55048882/68866660-1af44300-0738-11ea-8834-6187d0cbe97a.jpg)<br><br>
스위치가 모두 결합 되었다면<br>
기능적으로 키보드 역할을 할 수 있는 상태가 된 것이다.<br> 
컴퓨터와 연결해서 모든 스위치가 잘 동작하는지 체크해보면 된다.<br><br>
### 5. 키캡 결합<br>
키캡은 간단히 결합하면 된다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866661-1af44300-0738-11ea-92b8-51b818d8cb80.jpg)<br><br>
![](https://user-images.githubusercontent.com/55048882/68866662-1af44300-0738-11ea-851f-9710f4fb2272.jpg)<br><br>
이미 디자인에서부터 인지되듯이 키캡의 구성이 꽤나 특이하다.<br> 
이해할 수 없는 기호의 modifier가 보이는데<br>
수학과 컴퓨터의 논리게이트를 형상화한 듯하다.<br>
그러나 결국 기호와 실제 기능은 하등 상관이 있을 수는 없다.<br> 
그저 60% 이하의 키보드지만 얼마든지 기능을 넓힐 수 있는 유연성을 가졌다고<br> 
좀 어필하려고 한 것이라 생각이 든다.<br><br>
처음부터 충분히 예쁜 디자인이라고 생각하기는 했지만<br> 
미리 사뒀던 업무용 키보드는 결국 다른 무각 키캡을 사서 끼울 수 밖에 없었다.<br><br>
**위에서 얘기했듯 이 키보드는 커스텀 레이아웃 세팅이 가능해서 키캡과 전혀 상관 없는 구성을 가져가게 될 수도 있기 때문이다.**<br><br>
업무용 키보드는 '시간'을 컨셉으로 한 키캡을 끼웠고, 아래와 같은 모양으로 사용하고 있다.<br><br>
![](https://user-images.githubusercontent.com/55048882/68866637-1760bc00-0738-11ea-9a16-8488291b41ce.jpg)<br><br>
이렇게 조립하는 과정은 당연하게도 흥미롭고 재밌다.<br>
그리고 이 단순한 구조 속에 얼마나 많은 기능이<br>
직관적으로 잘 표현되는지를 생각해보면<br>
뒤에서 거쳐온 많은 고민과 발전과정을 조금 느낄 수 있다.<br>