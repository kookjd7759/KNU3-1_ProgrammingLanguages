# Kangwon national university

3nd year 1nd semester

## Programming Languages
#### Second Homework
Grade : 100.00 / 100.00

Grade on : 2022-04-11 16:29

Graded by	: KimSeongU

### Ocaml 연산

Question 1. [10점] 1에서 n까지의 정수의 합을 구하는 함수 sum을 작성하라.
(타입) int -> int
(설명) sum n은 n ≤ 0인 경우 0을, n > 0인 경우
n(n+1)
2 을 반환한다.
(실행 예)
# sum;;
- : int -> int = <fun>
# sum (-10);;
- : int = 0
# sum 100;;
- : int = 5050
Question 2. [10점] 반지름이 r인 원의 넓이를 구하는 함수 circle을 작성하라.
(타입) float -> float
(설명) circle r은 r ≤ 0.0인 경우 0.0을, r > 0.0인 경우 3.14r
2을 반환한다.
(실행 예)
# circle;;
- : float -> float = <fun>
# circle (-10.1);;
- : float = 0.
# circle 4.2;;
- : float = 55.3896
Question 3. [10점] 문자열의 앞에 “Hello ”를 삽입하는 함수 concat을 작성하라.
(타입) string -> string
(설명) concat s는 문자열 s의 앞에 "Hello "를 삽입한 문자열을 반환한다. (Hello 뒤에 공백문자가
있음에 유의하라.)
(실행 예)
# concat;;
- : string -> string = <fun>
# concat "Bob!";;
- : string = "Hello Bob!"
# concat "Alice!";;
- : string = "Hello Alice!"
Question 4. [10점] 논리연산자 xor를 계산하는 함수 xor를 작성하라.
(타입) bool -> bool -> bool
(설명) xor x y는 불린형 값 x와 y중 하나만 true일 경우에 true를, 이외의 경우 false를 반환한다.
(실행 예)
# xor;;
- : bool -> bool -> bool = <fun>
# xor true true;;
- : bool = false
# xor true false;;
- : bool = true
# xor false true;;
- : bool = true
# xor false false;;
- : bool = false
Question 5. [10점] 세 정수를 변의 길이로 가지는 삼각형이 존재하는지 확인하는 함수 triangle을
작성하라.
(타입) int -> int -> int -> bool
2
(설명) triangle x y z는 x, y, z중 하나라도 0 또는 음수인 경우 false를, x, y, z가 모두 양수인 경우
x, y, z를 세 변으로 가지는 삼각형이 존재하면 true를, 존재하지 않으면 false를 반환한다.
(실행 예)
# triangle;;
- : int -> int -> int -> bool = <fun>
# triangle (-3) 3 1;;
- : bool = false
# triangle 3 4 5;;
- : bool = true
# triangle 100 1 2;;
- : bool = false
Question 6. [10점] 두 정수의 합과 차 중 하나를 선택하는 함수 int if then else를 작성하라.
(타입) bool -> int -> int -> int
(설명) int if then else b x y는 b가 true이면, x + y를 false이면 x − y를 반환한다.
(실행 예)
# int_if_then_else;;
- : bool -> int -> int -> int = <fun>
# int_if_then_else true 2 100;;
- : int = 102
# int_if_then_else (100 < 2) 2 (-2);;
- : int = 4
Question 7. [10점] 임의의 2차 함수에 대하여 두 함수 값의 합을 구하는 함수 sum of fun val를 작성하라.
(타입) int -> int -> int -> int -> int -> int
(설명) sum of fun val a b c d e는 a, b, c를 각각 2차항, 1차항, 상수항의 계수로 갖는 2차 함수
f(x) = ax2 + bx + c에 대하여 f(d) + f(e)의 값을 반환한다.
(실행 예)
# sum_of_fun_val;;
- : int -> int -> int -> int -> int -> int = <fun>
# sum_of_fun_val 1 2 1 3 4;;
- : int = 41
# sum_of_fun_val 1 (-3) (-1) 200 123;;
- : int = 54158
Question 8. [10점] 정수를 임의의 2차 함수에 세번 적용한 값을 계산하는 함수 comp3를 작성하라.
(타입) int -> int -> int -> int -> int
(설명) comp3 a b c d는 a, b, c를 각각 2차항, 1차항, 상수항의 계수로 갖는 2차 함수 f(x) = ax2 + bx + c
에 대하여 f(f(f(d)))의 값을 반환한다.
(실행 예)
# comp3;;
- : int -> int -> int -> int -> int = <fun>
# comp3 1 1 1 1;;
- : int = 183
# comp3 1 (-2) 1 3;;
- : int = 64
Question 9. [10점] 두 번 반복된 문자열을 계산하는 함수 string2를 작성하라.
(타입) string -> string
(설명) string2 s는 문자열 s가 두 번 반복된 문자열을 반환한다.
(실행 예)
3
# string2;;
- : string -> string = <fun>
# string2 "hi";;
- : string = "hihi"
# string2 "abcde";;
- : string = "abcdeabcde"
Question 10. [10점] 2
8
(= 256)번 반복된 문자열을 계산하는 함수 string256을 작성하라.
(타입) string -> string
(설명) string256 s는 문자열 s가 2
8
(= 256)번 반복된 문자열을 반환한다.
(힌트) 9번에서 작성한 함수를 활용한다.
(실행 예)
# string256;;
- : string -> string = <fun>
# string256 "a";;
- : string =
"aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaa"
# string256 "ab";;
- : string =
"ababababababababababababababababababababababab
abababababababababababababababababababababababa
bababababababababababababababababababababababab
abababababababababababababababababababababababa
bababababababababababababababababababababababab
abababababababababababababababababababababababa
bababababababababababababababababababababababab
abababababababababababababababababababababababa
bababababababababababababababababababababababab
abababababababababababababababababababababababa
bababababababababababababababababababababab"
