# DNS란?
--------
사전적인 정의 부터 보자.

> **도메인 네임 시스템(Domain Name System, DNS)은 호스트의 도메인 이름을 호스트의 네트워크 주소로 바꾸거나 그 반대의 변환을 수행할 수 있도록 하기 위해 개발되었다.**

위키백과에서는 DNS를 이렇게 설명하고 있다.

예를 들면 우리가 자주 접하는 naver.com , google.com 모두 DNS을 가진 DN(Domain Name)이라고 할 수 있다.

이들은 사실 문자열의 탈을 쓴 IP라고 볼 수 있다.

cmd에서 구글과 naver의 DN을 적어 ping을 확인해 보자

![google_ip](https://velog.velcdn.com/images%2Fgoban%2Fpost%2Fc78b8302-78f0-4578-845b-61174a1912c4%2FDNSgoogleip.PNG)

![naver_ip](https://velog.velcdn.com/images%2Fgoban%2Fpost%2F220ca502-8897-4f46-a10f-cab744b4c27e%2FDNSnaverIp.PNG)

이렇게 DN을 통해 자기 컴퓨터가 사이트의 어느 IP 주소로 연결 되는지 확인 할 수 있다. (자신과 가까운 DNS서버를 통해 IP주소를 받아온다.)

-------

# DNS의 작동원리
아래는 그림은 DNS가 어떻게 작동하는지 보여준다.

![dns_mechanism](https://velog.velcdn.com/images%2Fgoban%2Fpost%2F5717ceb7-79f2-41d3-86e5-7e48bfd6ac58%2FDNSLogic.png)

1.웹 브라우저에 www.naver.com을 입력하면 먼저 Local DNS에게 "www.naver.com"이라는 hostname"에 대한 IP 주소를 질의하여 Local DNS에 없으면 다른 DNS name 서버 정보를 받음(**Root DNS** 정보 전달 받음)

Root DNS란?

> **Root DNS** (루트 네임서버) 는 인터넷의 도메인 네임 시스템의 루트 존이다. 루트 존의 레코드의 요청에 직접 응답하고 적절한 최상위 도메인에 대해 권한이 있는 네임 서버 목록을 반환함으로써 다른 요청에 응답한다. 전세계에 961개의 루트 DNS가 운영되고 있다.

2.Root DNS 서버에 "www.naver.com" 질의

3.Root DNS 서버로 부터 "com 도메인"을 관리하는 **TLD (Top-Level Domain)** 이름 서버 정보 전달 받음

> 여기서 TLD는 .com을 관리하는 서버를 칭함

4.TLD에 "www.naver.com" 질의

5.TLD에서 "name.com" 관리하는 DNS 정보 전달

6."naver.com" 도메인을 관리하는 DNS 서버에 "www.naver.com" 호스트네임에 대한 IP 주소 질의

7.Local DNS 서버에게 "응! www.naver.com에 대한 IP 주소는 222.122.195.6 응답

8.Local DNS는 www.naver.com에 대한 IP 주소를 캐싱을 하고 IP 주소 정보 전달



TLD의 구조는 어떻게 구성되어 있을까?

![TLD](https://velog.velcdn.com/images%2Fgoban%2Fpost%2F679d8a2b-1933-4850-95b9-c13765b9ff6c%2FTLD.jpg)

![TLD2](https://t1.daumcdn.net/cfile/tistory/232A484D5905623334)

최상위 ICANN 아래에 REGISTRY, NIC이 있고 REGISTRY 아래에 우리가 흔이 보는 gTLD 그리고 new gTLD가 있고 NIC아래에는 공공사이트에서 쓰는 ccTLD 도메인 주소가 있다.

--------

# **출처** 
* (https://velog.io/@goban/DNS%EC%99%80-%EC%9E%91%EB%8F%99%EC%9B%90%EB%A6%AC)
* (https://xn--3e0bx5euxnjje69i70af08bea817g.xn--3e0b707e/jsp/resources/domainInfo/domainInfo.jsp)
