# ClojureStudy
2017.7.15
- 컴파일하는법
- 4clojure약간

2017.7.17
- 파이썬스터디에서하는_백준문제_클로저로풀기

2017.7.22
- 개발환경세팅
- 웹개발도전하기

2017.7.29
- 함수에 대해 실습을 조금 해봤다.
- 재밌는 것은 함수를 파라미터로 넘겨줄 수 있다는 것!
<예제>
(defn apply-one-two [f] (f 1 2))
(defn add [x y] (+ x y))
(apply-one-two add)
-> 3

1 2 말고 매번 새로 값을 넣고 싶어서 여러 시도를 해봤더니

(defn apply-one-two [f x y] (f x y))
(defn add [x y] (+ x y))
(apply-one-two add 10 20)
-> 30

그리고 함수를 여러 번 인자로 넘기고 싶을 때에는
(appy-one-two add 5 (add 10 20))
-> 35

 세 개도 되는지 해봐야 겠당.
