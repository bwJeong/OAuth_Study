# OAuth_Study

## OAuth

### 개요
>타서비스 API 기능을 활용한 서비스를 개발하고 싶다! 하지만, 어떻게..?

타서비스 사용자의 정보(Id, Password)를 직접 요청받아 사용한다는 것은 불가능한 일, 이러한 문제를 해결할 수 있는 것이 바로 **OAuth**이다. 타서비스에서는 OAuth를 활용해 Client에게 직접적인 사용자의 정보를 전달해주는 대신 Access Token을 발급해 줌으로써 문제를 해결할 수 있다!

### Client, Resource Owner, Resource Server
- Client: 사용자가 사용하고자 하는 서비스
- Resource Owner: 사용자
- Resource Server: API를 제공하는 타사 서비스

