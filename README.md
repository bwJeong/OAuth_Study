# OAuth_Study

## OAuth

### 개요
>타서비스 API 기능을 활용한 서비스를 개발하고 싶다! 하지만, 어떻게..?

타서비스 사용자의 정보(Id, Password)를 직접 요청받아 사용한다는 것은 불가능한 일, 이러한 문제를 해결할 수 있는 것이 바로 **OAuth**이다. 타서비스에서는 OAuth를 활용해 Client에게 직접적인 사용자의 정보를 전달해주는 대신 Access Token을 발급해 줌으로써 문제를 해결할 수 있다!

### Client, Resource Owner, Resource Server
>3자간의 관계이기 때문에, 철저한 인증(Authentication)과 허가(Authorization)가 필요하다!

- Client: 사용자가 사용하고자 하는 서비스
- Resource Owner: 사용자
- Resource Server: API를 제공하는 타사 서비스

### 과정

#### 1. Client 등록
- 타사 서비스의 API를 이용하기 위해 Resource Server에 Client를 등록하고, **Client Id & Secret**를 발급받음

#### 2. 사용자 정보 접근 권한 요청
- 사용자가 Client 서비스에서 '타사 서비스 로그인' 기능을 사용하고자 할 경우, Client는 타사 서비스의 로그인창을 띄워주게 됨
- Resource Server에서는 사용자에게 'Client에 대한 사용자 정보 접근 권한'을 요청함

#### 3. Access Token 발급
- 이에 사용자가 승락할 경우, Resource Server에서는 Client의 고유정보인 Id & Secret의 대조를 통해 Client 확인 절차를 수행함
- 모든 것이 일치할 경우, Resource Server에서는 Client에게 최종적으로 **Access Token**을 발급하게 됨
