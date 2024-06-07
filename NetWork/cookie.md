# 쿠키(Cookie)란?
------
쿠키는 유저들의 효율적이고 안전한 웹 사용을 보장하기 위하여 웹사이트에 널리 사용되고 있습니다. 쿠키는 웹사이트 접속시 접속자의 개인장치에 다운로드 되고 브라우저에 저장되는 작은 텍스트 파일입니다. 웹사이트는 쿠키를 통해 접속자의 장치를 인식하고, 접속자의 설정과 과거 이용내역에 대한 일부 데이터를 저장합니다.

일반적으로 쿠키에는 만료일이 있습니다. 예를 들어, 브라우저를 닫는 경우 자동으로 삭제되는 쿠키도 있으며(세션 쿠키), 일부는 수동으로 삭제되기 전까지 남아있는 등 더 오랜기간 동안 컴퓨터에 저장되는 쿠키도 있습니다(지속적 쿠키). 본 웹사이트는 세션 및 지속적 쿠키의 사용을 통해 유저들에게 일관성 있고 간소화된 웹 경험을 제공합니다.

![cookie](https://t1.daumcdn.net/cfile/tistory/25020637595F1C9619)

------
# 생각 정리...<br/><br/>

## 쿠키 왜 쓸까?
> http 통신 규약은 모든 요청자에 대해 연결을 유지하게 될 경우 유지비용 오버헤드가 매우 크다. 따라서 요청자가 서버에 요청 -> 서버가 요청자에게 응답 -> 연결 종료로 이루어지는데, 그냥 연결을 종료 하지 않고
쿠키를 이용해 요청자 브라우저 정보를 저장시켜 요청자 구분 및 과거 정보를 식별한다.(나중에 요청자 또한 서버에게 요청이 있을 때 서버에게 같이 전송된다.)
나는 쿠키가 운영체제에서 프로세스의 PCB역할과 비슷하다고 느꼈다.

## 쿠키의 예

* **1.로그인 상태**
> 쿠키 정보에 사용자 로그인 상태가 담겨져 사용자가 로그인 상태라면 서버는 로그인 요구를 전송하지 않는다.

* **2.광고**
> 사용자의 요청 정보 및 언어를 고려해 그에 맞게 광고를 띄운다.
> 
> 사용자의 광고보기 상태가 7일간 보지 않기이면, 7일동안 광고를 띄우지 않는다.

# 출처
* https://kobrekim.com/footer-ko-kr/cookie-policy-ko-kr/what-are-cookies-and-why-we-use-them-ko-kr/