# 📍commit msg를 잘 작성해야 하는 이유.

1. 간결하고 일관적일 때 가독성이 좋고.
2. 이 또한 개발자의 역량이라 생각 됨.


# 👉commit msg를 작성하는 7가지 규칙

## 1. 제목과 본문으로 나누고 빈 줄로 구분한다.

commit msg가 단순한 경우는 그냥 쓰면 된다.
그러나 commit msg를 길게 써야하는 경우 제목과 본문으로 나누고, 이를 구분하기 위해 제목과 본문 간에 공백을 넣어 구분해준다🙌

_**실제 git에서 커밋메시지를 확인할 때, 제목과 본문으로 구분지어져서 확인할 수 있다.**_
<img 추가 - git에서의 커밋메시지>

### 🔹why?
1. 터미널에서 _'--oneline' 및 'shortlog'_ 옵션으로 커밋 로그를 볼 때, 보기 좋지 않음..
(**사진1.** 커밋메시지,  **사진2.** 콘솔창 확인)
![](https://images.velog.io/images/jppark/post/d46bd180-c4c9-4ca0-b0c7-684070205a95/50%EC%9E%90%EC%9D%B4%EC%83%81-%EC%A0%9C%EB%AA%A9%EB%B3%B8%EB%AC%B8%EC%82%AC%EC%9D%B4%EA%B3%B5%EB%B0%B1%EC%97%86%EC%9D%B4.PNG)![](https://images.velog.io/images/jppark/post/87a911d2-e774-47de-a04b-279646ed0509/50%EC%9E%90%EC%9D%B4%EC%83%81-%EC%A0%9C%EB%AA%A9%EB%B3%B8%EB%AC%B8%EC%82%AC%EC%9D%B4%EA%B3%B5%EB%B0%B1%EC%97%86%EC%9D%B4-%EC%BD%98%EC%86%94%EB%A1%9C%EA%B7%B8.PNG)


### 🔹how?
본문이 있는 경우 '-m' 을 통해 커밋메시지를 작성하기 어려움이 있기에, 메모장과 같은 텍스트 편집기를 활용하여 커밋 메시지를 작성하는 것이 좋겠다.

## 2. 제목은 50자 이내로!
엄격한 제한이 아닌 서로 묵인하는 룰 같다.
github UI에서도 50자가 넘어가면 경고를 해준다니, 50자 이내로 간결하게 하기로!

## 3. 제목의 시작은 대문자로(영어의 경우)

## 4. 제목을 마침표로 끝내지 않는다.
굳이 필요도 없을 뿐더러, 50자는 생각보다 짧습니당😂

## 5. 제목에 명령적인 뉘앙스를 사용한다.

## 6. 본문을 한 줄은 72자를 넘기지 않는다(권장)
git은 전체적으로 80자 미만으로 텍스트를 유지하게 한다네용🤷‍♂️

## 7. 본문의 내용을 이용하여 '무엇을, 왜, 어떻게'에 대한 내용을 보충한다.
변경이유, 변경 전 동작 방식, 변경 후 동작 방식 등에 대한 내용을 자세히 적어둔다면 
함께 일하는 동료 및 커미터들이 보고 이해하기 수월하겠죠?

# 자주 쓰는 커밋 keyword
* FIX
  * 올바르지 않은 동작을 수정하는 경우에 사용.
  ex) fix A where B, fix A when B ...
* ADD
  * 예제, 코드, 기능 등을 추가할 때 사용.
  ex) Add A for B ..
* MAKE
  * 기존 동작의 변경에 대한것을 명시할 경우 사용.
  * Add는 새롭게 무엇인가를 만들고 추가할 때 사용한다면, make은 기존의 동작을 바꿀 때 사용.
* REMOVE
  * 불 필요한 부분을 삭제할 때 사용.
  * 보통 A 앞에 ‘unnecessary’, ‘useless’, ‘unneeded’, ‘unused’, ‘duplicated’가 붙는 경우가 많습니다.
  * ex) Remove A from B .. 
* USE
  * 뜻 그래도 무언가를 사용하였음을 명시하기 위해 사용하겠죠?
  ex) Use A for B, Use A to B(a가 b가 되도록 사용한다), Use A in B, Use A instead of B
* REFACTOR
  * 전반적인 수정, 리팩토링 했음을 보이는데 사용.
* SIMPLIFY
  * 리팩터 보다는 약한, 코드를 단순화 하거나 수정의 정도가 적은 경우 사용.
* UPDATE
  * 버전 업데이트가 있는 경우 사용. 
  * FIX와 다른 점은 fix는 잘못된 부분을 수정하거나 하는 것을 의미하나, update의 경우에는 기존의 것에 추가, 보완 한다는 느낌으로 생각하시면 됩니다. 그렇기 때문에 코드 내용보다는 문서나 리소스, 라이브러리 등을 업데이트할 때 사용한다고 합니다.👀
  * ex) Update A to B
* CORRECT, SET ( 수정하는 범주의 크기: CORRECT > SET )
  * 주로 문법의 오류나 타입 변경 등을 적용할 때 사용.
* 그 외에도 종종 쓰이는 표현들
  * IMPORVE, IMPLEMENT, REVISE, ENSURE, PREVENT, AVOID, MOVE, RENAME .. 등

# 👏참고링크 및 출처
[Link 1](https://blog.ull.im/engineering/2019/03/10/logs-on-git.html) <br>
[Link 2](https://chris.beams.io/posts/git-commit/) <br>
[Link 3](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#heading=h.greljkmo14y0) <br>
[Link 4](https://doublesprogramming.tistory.com/256)
