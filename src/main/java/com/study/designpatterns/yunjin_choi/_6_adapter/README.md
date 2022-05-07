## 어댑터 패턴

---

> 기존 코드를 클라이언트가 사용하는 인터페이스의 구현체로 바꿔주는 패턴 <br>
> 클라이언트가 사용하는 인터페이스를 따르지 않는 기존 코드를 재사용할 수 있게 해준다.

조금더 쉽게 정리해보면 서로 호환성이 없는 인터페이스때문에 함께 동작할 수 없는 클래스들이 함께 작동할 수 있도록 해주는 패턴이라고 보면 편하다.

### Client
써드파티 라이브러리나 외부 시스템을 사용하는 쪽을 의미

### Target
Adapter가 구현하는 인터페이스이며, Client는 해당 Target Interface를 통해 Adaptee인 써드파티 라이브러리를 사용한다.

### Adaptee
써드 파티 라이브러리나 외부 시스템을 의미

### Adapter
Client와 Adapter 중간에서 호환성이 없는 둘을 연결시켜주는 역할을 담당.<br>
Target Interface를 구현하며, Client는 TargetInterface를 통해 어댑터에 요청을 보낸다.
클라이언트의 요청을 Adaptee가 이해할 수 있는 방법으로 전달하고 처리는 Adaptee가 진행한다.

