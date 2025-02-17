# 로또
## 진행 방법
* 로또 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nexts tep-docs/tree/master/codereview)

## 요구사항
* 로또 구입 금액을 입력하면 구입 금액에 해당하는 로또를 발급해야한다.
* 로또 한장의 가격은 1,000원이다. 


## 기능구현
* [x] 로또 번호 하나에 해당하는 객체(`LottoNumber`) 만들기.
  * [x] 이 객체는 1~45 숫자 중 하나이다. 
  * [x] 1~45 중에 6개의 값을 뽑아 shuffle 한다.
* [x] `LottoNumber` 객체가 6개가 모이면 `LottoNumbers`가 된다. 
  * [x] `LottoNumber`의 size 는 6이여야 한다.
  * [x] `LottoNumber` 안에서 중복은 허용하지 않는다. 
* `controller` 만들기
  * [x] 입력된 구매 금액 / 1000 = 로또 구매 갯수
  * [x] 지난 주 당첨 번호 입력 
  * [x] 당첨통계 만들기 <- 객체로 생성