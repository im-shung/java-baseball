# 미션 - 숫자 야구
1부터 9까지 서로 다른 수로 이루어진 3자리의 수를 맞추는 게임

## 🚀 기능 목록

1. 입력
   - 사용자 number
2. 입력 검증
   ```
      ⅰ. 서로 다른 3자리의 수: 게임 진행
      ⅱ. 1: 게임 재시작
      ⅲ. 2: 게임 종료
      ⅳ. 3자리의 수가 아님: IllegalArgumentException 발생시킨 후 애플리케이션 종료
      ⅴ. 서로 같은 수가 있음: IllegalArgumentException 발생시킨 후 애플리케이션 종료
      ```
3. 컴퓨터 number 생성
4. 게임
   - 컴퓨터 number와 사용자 number를 비교한다. 
   ```
     같은 수가 같은 자리에 있으면 1스트라이크
     같은 수가 다른 자리에 있으면 1볼
     같은 수가 전혀 없으면 낫싱
   ```
   - 3스트라이크가 나올 때 까지 '1.입력'->'2.입력 검증'->'4.게임'을 반복한다.
5. 게임 종료
  - 게임 재진행 여부 묻기
  - 만약 재시작이라면 '1.입력'으로 돌아간다.