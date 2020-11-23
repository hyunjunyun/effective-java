# 클래스와 인터페이스 (4장)

## #21 : 인터페이스는 구현하는 쪽을 생각해 설계하라

> 인터페이스에 디폴트 메서드 추가는 기존의 구현되어있는 구현체에 오류를 가져올 수 있으므로 되도록 피하며, 불가피한 상황에서는 주의를 기울여 설계해야 한다.
>

### 요약

- 디폴트 메서드를 선언하면, 그 인터페이스를 구현한 후 디폴트 메서드를 재정의하지 않은 모든 클래스에서 디폴트 구현이 쓰이게 된다.
- 모든 상황에서 불변식을 해치지 않는 디폴트 메서드를 작성하는 것은 어렵다.
  - 자바 8에서 컬렉션 인터페이스들에 람다를 활용하기 위해 다수의 디폴트 메서드가 대부분의 상황에 잘 작동하도록 설계되어 추가되었다.
- 디폴트 메서드는 컴파일에 성공하더라도 기존 구현체에 런타임 오류를 일으킬 수 있다.
- 기존 인터페이스 디폴트 메서드로 새 메서드를 추가하는 일은 꼭 필요한 경우가 아니면 피해야 한다.
- 이처럼 이미 작성된 구현체에 예측 불가능한 오류를 가져올 수 있으므로 인터페이스 설계 시 주의를 기울여야 한다.



## References

- Effective Java 3/E - Joshua Bloch
- [JavaSquid Issue-21](https://github.com/java-squid/effective-java/issues/21)

-----

## QNA

- [JavaSquid Issue-21](https://github.com/java-squid/effective-java/issues/21)

<img width="927" alt="21-1" src="https://user-images.githubusercontent.com/58318041/99638372-79f64180-2a89-11eb-86bd-8f841902d004.png">
