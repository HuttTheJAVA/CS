# URL의 구성

* **프로토콜**: URL은 자원을 접근하는 방법인 스킴scheme으로 시작한다. 스킴보다는 프로토콜이라고 부르는게 일반적이므로 앞으로는 프로토콜이라고 쓰겠다.

* **사용자정보**: 사용자 아이디와 비밀번호를 사용자정보userinfo로 부른다. 잘 사용하지 않기 때문에 따로 설명하지 않겠다. (예: https://username:password@www.example.com/)

+ **호스트**: 그리고 호스트 주소가 나온다. IP 또는 www.example.com과 같은 도메인명을 쓴다. 호스트명:포트번호 형태로 포트번호를 쓸 수 있는데 선택사항이다.

+ **경로**: 호스트 주소 다음에 /으로 시작하는 경로가 나온다. 윈도우의 디렉토리나 폴더와 비슷하다고 보면 된다. 루트 디렉토리가 /으로 시작하는 것이 윈도우와 다르다 (예: https://www.example.com/).

- **매개변수**: 그 다음은 웹서버에 보내는 추가 매개변수(Query 또는 Parameters)가 온다.

- **부분식별자**: 마지막으로 #으로 시작하는 부분 식별자(fragment identifier)가 온다.

![url_image](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-768x69.png)<br/><br/><br/><br/>


* **프로토콜**

![protocol](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-protocol-300x42.png)
-----
프로토콜은 웹에서 서버와 클라이언트간에 어떤 방법으로 자원을 접근할지 알려준다. 웹브라우저에서 가장 많이 사용되는 https/http외에도 mailto: (이메일 주소를 지정하는 프로토콜), ftp: (파일을 주고받는 프로토콜) 등 다양한 프로토콜이 존재한다.

우리가 가장 많이 사용하는 HTTP는 Hyper Text Transfer Protocol이라는 어려운 이름의 약자인데 쉽게 설명하면 웹브라우저와 웹서버 사이에서 웹 문서와 그것을 구성하는 자원을 전송하기 위한 프로토콜이다. 요즘은 HTTPS를 기본 프로토콜로 쓰는데, (https를 지원하지 않는 웹사이트는 여전히 http를 쓴다) HTTP에 보안이 강화된 버전이다.  <br/><br/><br/><br/>
* **호스트**

![host](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-host-400x51.png)

URL에서 웹서버의 위치를 지정한다. 도메인 이름(예: www.example.com)이나 IP 주소(예: 127.0.0.1)를 사용할 수 있다.

도메인 이름 뒤에 오는 :80는 포트번호다. 웹서버에서 자원을 접근하기 위해 사용하는 관문(gate)을 가리키는데, 표준 HTTP 포트는 80번 HTTPS는 443이다. 표준 포트를 사용한다면 포트번호는 보통 생략한다.<br/><br/><br/><br/>

* **경로**

![path](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-path-300x73.png)

웹서버에서 자원에 대한 경로다. 실제 물리적 경로가 아니고 웹서버에서 추상화한 경로다(물론 웹서버 설정에서 물리적 경로를 추상화 경로로 사용할 수 있다).

루트 자원을 나타내려면 “/”을 사용한다. 예) https://www.example.com/

루트의 robots.txt를 지정한다면 다음과 같다. 예) https://www.example.com/robots.txt<br/><br/><br/><br/>

* **매개변수 (Query 또는 Parameters)**

![parameters](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-parameters-400x47.png)

웹서버에 보내는 추가 파라메터다. 파라메터 하나는 키와 값으로 짝을 이룬다. 파라메터가 여러개면 &문자로 구분한다. 키와 값은 =문자로 구분한다. 웹서버에서 어떤 파라메터를 실제로 지원하는지는 웹서버마다 다르다. 웹서버는 지원하지 않는 파라메터는 무시한다.<br/><br/><br/><br/>

* **부분 식별자 (Fragment identifier)**

![fragment](https://www.betterweb.or.kr/wp-content/uploads/2020/09/url-colored-fragment-150x46.png)

URL이 지정하는 자원의 세부 부분을 지정할때 쓴다. 부분 식별자가 없어도 그 앞에 오는 URL만으로도 웹의 어떤 자원을 정확히 지정할 수 있다. 부분 식별자는 자원 안에서 어떤 부분을 가르키는 역할을 한다. 부분 식별자가 쓰이는 대표적인 사례는 위키피디어 백과사전이다. 부분 식별자를 세부항목에 대한 책갈피bookmark로 쓸 수 있어서 어떤 글에서 특정 항목으로 바로 이동할 수 있다.

예) https://ko.wikipedia.org/wiki/대한민국#문화 : 위키피디어 “대한민국” 문서에서 “문화” 세부주제로 바로 갈 수 있다.<br/><br/>

# 출처(https://www.betterweb.or.kr/blog/url%EC%9D%B4%EB%9E%80/)
