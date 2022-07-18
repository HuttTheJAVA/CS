## Database의 리플리케이션(Replication)이란?

### 배경

아주 단순한 Database를 구성할때에는 아래의 그림처럼 하나의 서버와 하나의 Database를 구성하게 된다.

<p align="center"><img src="https://nesoy.github.io/assets/posts/20180216/1.png"></p>   

하지만 사용자는 점점 많아지고 Database는 많은 Query를 처리하기엔 너무 힘든 상황이 오게 된다.

Query의 대부분을 차지하는 Select를 어느 정도 해결하기 위해 Replication이란 방법이 나오게 되었다.
<br></br>
### Replication이란?
> * 두 개의 이상의 DBMS 시스템을 Mater / Slave로 나눠서 동일한 데이터를 저장하는 방식이다.
<br></br>
### 방식

<p align="center"><img src="https://nesoy.github.io/assets/posts/20180216/2.png"></p>

**Master DBMS**에는 데이터의 수정사항(데이터 등록/수정/삭제)을 반영만하고 Replication을 하여 **Slave DBMS**에 실제 데이터를 복사한다.
<br></br>
### Replication 장점

<p align="center"><img src="https://nesoy.github.io/assets/posts/20180216/3.png"></p>

언급했던 것처럼 Query의 대부분은 **Select**가 차지하고 있다.

이 부분의 부하를 낮추기 위해 많은 **Slave Database**를 생성하게 된다면 **Read(Select)** 성능 향상 효과를 얻을 수 있다.

**Master Database** 영향없이 로그를 분석할 수 있다.

# 출처
* https://nesoy.github.io/articles/2018-02/Database-Replication
