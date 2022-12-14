# ID 관련 용어

- `ID 표준 및 프로토콜`

    - ID 및 액세스 관리를 위한 업계 표준 및 프로토콜이 있기 때문에 사용자가 외부 웹사이트나 앱에 로그인할 필요 없이 사용자의 ID를 안전하게 유지할 수 있다
    - Salesforce 및 기타 ID 공급자가 ID 솔루션을 구현하기 위해 따르는 세 가지 프로토콜(SAML, OAuth 2.0, OpenID Connect)

- `SAML 프로토콜`

    - 사용자가 반복적으로 로그인하지 않고 Salesforce 조직과 애플리케이션 간에 원활하게 전환하도록 지원하려면 싱글사인온을 설정

- `SAML 어설션`

    - 동작방식
```
1. 사용자가 서비스에 액세스를 시도
2. 서비스 공급자는 액세스 허용 여부를 판단하기 위해 ID공급자에게 액세스 요청 전송
3. ID공급자는 데이터베이스 확인하여 허용 여부 전달
```

- `SAML 및 XML`

    - SAML은 XML 기반 프로토콜
    - 교환되는 정보 패키지가 XML로 작성
    - 즉, XML 형식으로 작성되어 정보가 전달

- `OAuth 2.0 프로토콜`

    - 애플리케이션 간의 안전한 데이터 공유를 위해 사용되는 개방형 프로토콜
    - 사용자는 한 앱에서 작업하지만 다른 앱의 데이터를 볼 수 있다
    - 보이지 않는 곳에서 앱은 서로 통신한 후 사용자에게 이 데이터 공유를 승인하도록 요청
    - 개발자는 앱을 Salesforce와 통합할 때 OAuth API를 사용

- `OpenID Connect`

    - OpenID Connect 프로토콜은 OAuth 2.0에 인증 계층을 추가하여 사용자 정보의 안전한 교환을 지원
    - SAML과 달리 OpenID Connect는 오늘날의 소셜 네트워크를 위해 개발

- `서비스 공급자와 ID 공급자`

    - 사용자를 인증하는 과정에서 SAML은 ID 공급자(IdP)라고 불리는 정보 소유자와 서비스 공급자라고 불리는 원하는 서비스 간에 ID 정보를 교환
    - 사용자가 Salesforce에 로그인한 후 Gmail에 액세스하는 경우 Salesforce가 ID 공급자이고 Google이 서비스 공급자이다
