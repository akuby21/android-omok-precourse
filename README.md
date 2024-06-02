# 오목 어플리케이션

카카오 테크 캠퍼스 2기 Android 트랙 2nd 미니과제
## 기능 요구사항
오목은 두 사람이 번갈아 돌을 놓아 가로나 세로, 대각선으로 다섯 개의 연속된 돌을 먼저 만들면 승리하는 게임이다. ***안드로이드 프레임워크를 사용하여 모바일 앱으로 구현한다.***
- 6목 이상의 장목도 착수 가능하며 승리 조건으로 인정한다.
- 렌주 룰과 같은 복잡한 룰은 고려하지 않는다

## 프로그래밍 요구 사항
- ***Java 코드가 아닌 Kotlin 코드로만 구현해야 한다.***
- `build.gradle.kts` 파일은 변경할 수 없으며, ***제공된 라이브러리 이외의 외부 라이브러리는 사용하지 않는다***.
- 프로그램 종료 시 `System.exit()` 또는 `exitProcess()`를 호출하지 않는다.
- indent depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
- 함수(또는 메서드)가 한 가지 일만 하도록 ***최대한 작게*** 만들어라.
- `JUnit 5`와 `AssertJ`를 이용하여 정리한 기능 목록이 정상적으로 작동하는지 테스트 코드로 확인한다.
- 함수(또는 메서드)의 길이가 ***15라인***을 넘어가지 않도록 구현한다
- 예외 처리를 통해 프로그램이 강제 종료되는 것을 방지한다
  - 논리 오류가 있는 경우에만 예외를 던진다.
  - 논리 오류가 아닌경우 예외가 아닌 `null`을 반환한다
  - 실패 사례가 복잡하여 null로 처리할 수 없는 경우 `sealed class`를 반환한다.
  - 일반적인 코틀린 코드에서는 `try-catch`를 사용하지 않는다.



## 구현한 기능 목록
- [x] 번갈아가며 흑색, 백색 돌이 착수되도록 하기
- [x] 이미 착수된 공간에는 착수 못하게 하기
- [x] 착수 가능한 공간 클릭 시 차례에 맞는 돌 그리기
- [x] 착수 후 가로, 세로, 대각선중 승리 요건이 있는지 확인하기
- [ ] 다시 시작 