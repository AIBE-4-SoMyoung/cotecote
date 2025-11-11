# Java Stream & Lambda Roadmap

## Ⅰ. Stream 완전 정복

| 번호 | 문제명 | Stream 포인트 | 학습 포인트 |
|:----:|:----------|:--------------------------|:-------------------------------------------|
| #2910 | 빈도 정렬 | groupingBy, counting, sorted | Map → Stream 변환 및 빈도 정렬 패턴 숙달 |
| #19636 | 요요 시뮬레이션 | map, reduce | 누적 계산 로직 및 함수형 사고 확립 |
| #1181 | 단어 정렬 | distinct, sorted, thenComparing | 중복 제거 + 다중 정렬 체인 |
| #5635 | 생일 | min, max, Comparator | 객체 리스트의 최소/최대 비교 연습 |

Stream의 핵심 연산(map, filter, reduce, collect, min/max)을 실전 예제 중심으로 학습합니다.

---

## Ⅱ. Lambda 완전 정복

| 번호 | 문제명 | 난이도 | 람다 포인트 | 요약 |
|:----:|:-----------:|:------------:|:-----------------------------|:-------------------------------------------|
| #10814 | 나이순 정렬 | Silver V | (a, b) -> a.age - b.age | Comparator를 람다식으로 표현, 코드 간결화 |
| #1181 | 단어 정렬 | Silver V | thenComparing() 체인 | 길이 → 사전순 정렬을 람다식으로 구현 |
| #2751 | 수 정렬하기 2 | Silver V | list.sort((a, b) -> a - b) | Comparator 기본 람다식 문법 연습 |
| #5635 | 생일 | Silver V | Comparator.comparing((p) -> p.year) | 객체 정렬 시 Comparator.comparing() 직접 활용 |

람다 문법, 메서드 레퍼런스(::), Comparator 체인을 완벽히 익히는 구간입니다.

---

## Ⅲ. Stream + Lambda 통합 실습

| 문제 | 연습 방식 | 학습 포인트 |
|:------|:--------------|:-------------------------------|
| #1181 단어 정렬 | 두 가지 버전으로 구현 | 람다 vs Stream 비교 (sorted(Comparator.comparing(...))) |
| #5635 생일 | 두 가지 버전으로 구현 | Comparator.comparing() + stream().min() 응용 |

동일 문제를 람다 버전과 스트림 버전으로 각각 구현해보며  
함수형 사고와 선언적 코딩 스타일의 차이를 체득합니다.

---

## 핵심 학습 맵

| 문법 요소 | 커버 문제 |
|------------|------------|
| Comparator.comparing, thenComparing | #10814, #1181, #5635 |
| map, filter, reduce | #19636 |
| groupingBy, counting, sorted | #2910 |
| distinct | #1181 |
| min, max | #5635 |
