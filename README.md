# system-design-interview

### 1. 사용자 수에 따른 규모 확장성

Failover / redunduncy: 장애 상황에 의해 서버가 다운될 수 있다. 서버가 다운되어도 서비스가 정상적으로 동작하는 것을 failover, 데이터가 사라지지 않는 것을 redunduncy(다중화) 다.

단일 장애 지점 (SPOF): 특정 지점의 장애가 서비스를 다운시킨다.

Stateless 웹 계층: 사용자 session 등의 상태 정보를 데이터베이스나 NoSQL 등에 저장하고 웹 계층에서 제거한다.

데이터 센터: 여러 곳에 서비스를 두어 (웹 계층, 데이터베이스, 등등) 지리적으로 로드밸런싱 한다. 데이터 동기화가 필요하므로 데이터를 데이터센터에 다중화한다.

Redis 는  in memory key value data storage 로 1ms 미만의 R/W 기능을 제공한다.

### 2. 개략적인 규모 측정

엔지니어의 가장 중요한 역량 중 하나는 올바른 질문을 하는 것이다.


