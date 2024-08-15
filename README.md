# lab-20240815

## 실험 동기
[Spring DI. Multiple Interface Implementations with Strategy Pattern](https://medium.com/spring-boot-tips-and-tricks/spring-di-multiple-interface-implementations-with-strategy-pattern-eac54a029102)
글에서 설명하는 내용을 스프리에서 제공하는 기본 기능으로 더 쉽게 구현할 수 있을 것 같아 검증을 시작한다.

## 실험 가설
인터페이스 A를 구현한 B, C 빈을 서비스에서 주입 받아 MAP에 넣으려한다. Key는 빈의 이름으로 Value는 빈을 저장한다.
위 글에서는 List 형태로 B, C 빈을 일단 주입 받고 이후 순환하면 수동으로 Map에 빈을 설정하고 있다.
하지만 내가 기억하기로는 스프링 명세에서 Map에 자동으로 위 방식으로 주입이 가능하다고 설명하였다.
