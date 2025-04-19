# Chapter 2-1. 클린코드와 리팩토링

## 기본과제: 더티코드 개선

이번 과제는 더티코드를 클린코드의 형태로 개선을 하는 과제입니다. 주어진 테스트를 통과하면서 원래 기능과 동일한 동작을 하는 코드를 만들어주세요. basic과제는 제공되는 더티코드를 클린코드와 리팩토링 원칙에 입각해서 더 나은 코드로 만들어보세요. 주어진 테스트를 참고삼아 좋은 이름, 좋은 모양, 좋은 구조를 가지는 코드로 만들어 보세요.

[필수조건]

- Prettier와 ESLint를 설치해서 적용할 것
- 테스트 코드 모두 통과할 것
- = 기존 기능과 동일하게 동작할 것
- = 어플리케이션 요구사항을 모두 만족할 것
    - 상품
        - 상품1 - 10,000원
        - 상품2 - 20,000원
        - 상품3 - 30,000원
    - 상품 관리
        - 상품을 장바구니에 추가할 수 있어야 한다.
        - 장바구니에서 상품을 제거할 수 있어야 한다.
        - 각 상품의 수량을 변경할 수 있어야 한다.
        - 재고가 부족한 상품은 장바구니에 담을 수 없습니다.
    - 가격 계산
        - 장바구니 내 모든 상품의 총액을 계산해야 한다.
        - 개별 상품의 가격과 수량에 따른 소계를 표시해야 한다.
        - 상품1 > 10개 이상 구매 시 10% 할인
        - 상품2 > 10개 이상 구매 시 15% 할인
        - 상품3 > 10개 이상 구매 시 20% 할인
        - 상품 종류와 상관 없이, 30개 이상 구매할 경우 25% 할인
        - 화요일에는 특별할인 10%
        - 임의의 시간마다 깜짝세일 20%, 추천세일 5%
    - 기본 기능
        - 장바구니에 상품 추가 기능
        - 장바구니에서 상품 제거 기능
        - 상품 수량 변경 기능
        - 장바구니 내역 조회 기능
        - 총액 계산 기능

## 심확과제: 유지보수 하기 좋은 코드만들기

심화과제는 **기본과제에서 작성한 코드를 기술고도화를 하는 것입니다.** 바닐라 자바스크립트로 되어 있는 코드를 유지보수하기에 유리한 기술스택(React + Typescript)으로 고도화 리팩토링을 진행해주세요.
우리의 목표는 앞으로 유지보수를 더 잘할 수 있도록 하기 위함입니다. 최소 React와 Typescript를 이용한 코드로 개선해주세요. 그 밖의 기술선택과 폴더/파일 구조, 테스트 코드등은 자유입니다.


## 요청사항

과제를 진행할 떄 AI를 쓰는 것은 자유입니다. 오히려 AI를 활용하는 연습을 해야하는게 시대의 흐름이겠지요.
다만 AI를 쓰더라도 최대한 조금씩 조금씩 이전 코드와 지금 코드를 그대로 유지하면서 리팩토링하는 감각을 기르기 위함이나,
AI에게 최대한 조금씩 그러나 구체적으로 요청하며 한번에 많은 코드를 바꾸지 않도록 하는 연습을 해보세요.


## 배포

- original: https://d5br5.github.io/front_5th_chapter2-1/
- basic: https://d5br5.github.io/front_5th_chapter2-1/index.basic.html
- advanced: https://d5br5.github.io/front_5th_chapter2-1/index.advanced.html

## 과제 체크포인트

### 기본과제

- [x] 코드가 Prettier를 통해 일관된 포맷팅이 적용되어 있는가?
- [x] 적절한 줄바꿈과 주석을 사용하여 코드의 논리적 단위를 명확히 구분했는가?
- [x] 변수명과 함수명이 그 역할을 명확히 나타내며, 일관된 네이밍 규칙을 따르는가?
- [x] 매직 넘버와 문자열을 의미 있는 상수로 추출했는가?
- [x] 중복 코드를 제거하고 재사용 가능한 형태로 리팩토링했는가?
- [x] 함수가 단일 책임 원칙을 따르며, 한 가지 작업만 수행하는가?
- [x] 조건문과 반복문이 간결하고 명확한가? 복잡한 조건을 함수로 추출했는가?
- [x] 코드의 배치가 의존성과 실행 흐름에 따라 논리적으로 구성되어 있는가?
- [x] 연관된 코드를 의미 있는 함수나 모듈로 그룹화했는가?
- [x] ES6+ 문법을 활용하여 코드를 더 간결하고 명확하게 작성했는가?
- [x] 전역 상태와 부수 효과(side effects)를 최소화했는가?
- [x] 에러 처리와 예외 상황을 명확히 고려하고 처리했는가?
- [x] 코드 자체가 자기 문서화되어 있어, 주석 없이도 의도를 파악할 수 있는가?
- [x] 비즈니스 로직과 UI 로직이 적절히 분리되어 있는가?
- [x] 코드의 각 부분이 테스트 가능하도록 구조화되어 있는가?
- [x] 성능 개선을 위해 불필요한 연산이나 렌더링을 제거했는가?
- [x] 새로운 기능 추가나 변경이 기존 코드에 미치는 영향을 최소화했는가?
- [x] 코드 리뷰를 통해 다른 개발자들의 피드백을 반영하고 개선했는가?
- [x] (핵심!) 리팩토링 시 기존 기능을 그대로 유지하면서 점진적으로 개선했는가?

### 심화과제

- [x] 변경한 구조와 코드가 기존의 코드보다 가독성이 높고 이해하기 쉬운가?
- [x] 변경한 구조와 코드가 기존의 코드보다 기능을 수정하거나 확장하기에 용이한가?
- [x] 변경한 구조와 코드가 기존의 코드보다 테스트를 하기에 더 용이한가?
- [x] 변경한 구조와 코드가 기존의 모든 기능은 그대로 유지했는가?
- [x] (핵심!) 변경한 구조와 코드를 새로운 한번에 새로만들지 않고 점진적으로 개선했는가?


## 과제 셀프회고

### 기본 정리

처음 코드를 열었을 때, 어디부터 손을 대야 할지 막막했습니다.
var, let, const가 여기저기 섞여 있었고, 변수명은 모호했고, 모든 코드 라인이 줄바꿈 없이 붙어있었습니다.
또 함수들간 전역 변수를 공유하고 있어서, 쉽게 분리할 수 없었습니다.
함수, 컴포넌트들을 각각 분리하기 전에, 기본적으로 정리하고자 했던 작업은 다음과 같습니다.

1. 적절한 줄바꿈
    - 어느 정도 맥락이 바뀌는 부분, 혹은 함수들 사이에 여백을 만들어 가독성을 높였습니다.
2. 변수명 구체화
    - q → quantity / tot → total / val → price 등
    - 축약어를 사용하면 코드는 줄지만, 오히려 가독성은 떨어질 수 있다는 것을 느꼈습니다.
3. var 근절하기
    - 변수 선언은 let, const로만 하도록 변경했습니다.
    - 되도록이면 const를 사용하고, 재할당이 꼭 필요한 부분에만 let을 사용했습니다.
    - 단순히 교체만하면 되는 것은 아니었습니다. 함수들끼리 서로 같은 전역변수를 바라보고 있는 경우가 많았습니다.
        - element 전역 변수(sel, addBtn 등)는, 참조하는 코드 직전에 매번 새롭게 탐색하는 구조로 변경하였습니다. 기존에는 변수 정의와 할당을 한번만 하고 계속 동일한 변수를 참조했는데, 이후에는 사용하고자 할때마다 최신의 요소를 조회하도록 했습니다.
        - 장바구니에서 사용할 number 변수들은, store 객체로 응집시켰습니다. 전역에 선언된 객체를 참조하지만, 변수 자체에는 불변성을 부여하여 single source of truth를 유지했습니다.
4. callback 함수를 화살표 함수 형태로 변경
    - map, forEach, find 등 배열 메서드 내부에서 사용하는 함수
    - 문법적으로 잘못된 것은 아니지만, 개인적으로 가독성이 더 좋다고 생각하는 방향으로 변경했습니다.
        - 기존: `prodList.find( function(p){ return p.id === selItem });`
        - 변경: `prodList.find( p ⇒ p.id === selItem )`
5. 변수가 포함된 문자열은 template literal 사용
    - + 연산으로 문자열을 합칠 경우, 내부 공백 위치 파악이 힘들고, 길이도 길어져 가독성이 떨어진다고 생각합니다.
    - 다음과 같이, 템플릿 리터럴을 사용하여 문자열의 가독성과 활용성을 높였습니다.
        - 기존: `'(' + (discRate * 100)*.toFixed*(1) + '% 할인 적용)'`
        - 변경 `(${(discRate*100).toFixed(1)}% 할인 적용)`
6. 유틸함수 분리
    - UI 에 직접적으로 영향을 주지 않는 데이터 가공함수들은 따로 정의하여 분리하였습니다.
    - 추후 파일로 분리하기 쉽도록, 순수함수 형태로 구성하였습니다
    - 예시
        
        ```jsx
        export const startRandomlyInMs = (ms) => (callback) => {
          const startsAt = Math.random(0) * ms;
          setTimeout(callback, startsAt);
        };
        ```
        
7. 매직 넘버 제거
    - 할인율, 할인적용상품수량, 추첨확률 등
    - 코드 라인 속에서 직접적으로 사용되고 있었던 매직 넘버를 상수 객체로 분리했습니다.
    - 숫자 변경이 필요할 경우, 한 곳만 수정해도 일괄 적용할 수 있습니다.
    - 숫자의 의미를 이름에서 유추할 수 있게 되었습니다.

### 컴포넌트 분리

기본 작업 이후, 컴포넌트로 분리하는 작업을 수행했습니다.

![image (12)](https://github.com/user-attachments/assets/11a40ba4-c085-44a5-9c18-04709bbd6bc5)

1. 컴포넌트 파악
    - 크게 위와 같이 나눠볼 수 있었습니다.
    - 더 세부적으로 나눌 수 있지만, 현재 코드에서는 여러 기능, 책임이 복잡하게 얽혀 있어 자잘하게 분리하는 것은 오히려 혼란스러울 것이라 판단했습니다.
2. template + onMount 구조로 분리
    - 각 컴포넌트의 UI를 그릴 html 문자열과, 이 컴포넌트가 렌더링된 이후 실행할 동작을 세트로 묶었습니다.
        - 예시, CartItemContainer
            
            ```jsx
            export const CartItemContainer = {
              template: () => `<div id="cart-items"></div>`,
              onMount: () => {
                const cartDisp = document.getElementById('cart-items');
                cartDisp.addEventListener('click', (event)=>{
            	    ...
                }
              },
            };
            ```
            
    - 컴포넌트를 사용하는 부모 위치에서는, 컴포넌트가 렌더링되어야 할 위치에 template을 호출하고, 그 부모의 onMount 메서드에서 컴포넌트의 onMount 메소드를 호출하도록 구성했습니다.
    - 이러면 DOM 요소를 트리 구조로 배치할 수 있고, mount시 실행할 동작 (이벤트 핸들러 부착)의 순서를 보장할 수 있습니다.
        - 예시, main.js
            
            ```jsx
            export const MainPage = {
              template: () => `
                <div class="bg-gray-100 p-8">
                  <div class="max-w-md mx-auto bg-white">
                    ${CartItemContainer.template()}
                  </div>
                </div>
              `,
              onMount: () => {
                CartItemContainer.onMount?.();
              },
            };
            ```
            
    - 렌더링 및 이벤트핸들러 부착 로직은 컴포넌트별로 깔끔하게 분리되었습니다.
3. update 함수 분리
    - web application은 1회성 렌더링보다, 이후 업데이트가 더 중요합니다.
    - select 후 버튼으로 제출하거나, 수량을 변경했을 때 그에 맞는 UI 업데이트가 필요합니다.
    - 변경된 데이터에 맞게 새로 UI를 업데이트하는 함수들을 따로 분리하였습니다
        - `updateStockInfo`, `updateBonusPoints` 와 같은 함수를 `updates` 폴더에 파일별로 구분했습니다.
    - 데이터 변경 로직을 수행하는 곳에, 위 업데이트 함수를 적절히 배치함으로써 UI가 적절히 반영되도록 했습니다.
4. 그 외 유틸 함수, store, constant 를 별도 파일로 분리했습니다. 

이렇게 정리를 하여, 다음과 같이 폴더를 구성할 수 있었습니다.

```jsx
components/
	add-to-cart-button.js
	cart-item-container.js
	stock-status.js
	...
lib/
	constants.js
	store.js
	utils.js
updates/
	bonusPoints.js
	selectOptions.js
	...
pages/
	main.js
main.basic.js
```

### 화요일 깜짝선물

화요일 00시가 되었을 때, 갑자기 테스트코드가 통과하지 않게 되었습니다.
코드를 잘못건든건가 싶어서 과거 커밋들로, 아예 태초 코드로 checkout해봐도 여전히 실패가 발생했습니다.
아니 분명히 됐었는데?! ㅜㅜ 멘붕이 왔지만 코드를 살펴보니 깜짝 선물이 숨어져 있었습니다. 

화요일인 환경과 아닌 환경을 구분해서 테스트할 수 있도록 테스트 날짜를 mocking했습니다. 
화요일인 경우의 테스트코드는 중간에 포함되어 있었으므로, 테스트 전체의 날짜를 화요일이 아닌 날짜로 고정해서 문제를 해결할 수 있었습니다.

```js
beforeEach(() => {
  // 날짜별 행사에 대응하기 위해 날짜 고정
  vi.useFakeTimers();
  const mockDate = new Date('2025-04-18');
  vi.setSystemTime(mockDate);
  vi.spyOn(window, 'alert').mockImplementation(() => {});
});
```

서비스 코드에 날짜 관련 내용이 포함되어 있을 때, 테스트 코드에서도 이를 잘 컨트롤해줘야 한다는 교훈을 얻었습니다..

### 팀별 컨벤션 정립 논의

수요일 멘토링이 끝난 후, 팀원들끼리 모여 컨벤션 논의를 했습니다. 
얘기해볼 포인트는 더 많지만, 우선 본 과제에 적용될 내용만 다루었습니다.

| 항목 | 규칙 |
|------|---|
| 변수명 | - 줄임말 사용 금지 (cnt, tot, subTot, Amt, q) <br> - camelCase <br> 복수형은 List 붙이기 |
| 상수명 | - UPPER_SNAKE_CASE <br> - 상수 객체: 이름 UPPER_SNAKE_CASE, 내부 key는 camelCase |
| 함수 | - 불필요하게 길어지지는 않도록, 하지만 최대한 구체적으로 작성 <br> - props 정의시 on[Event], 실제 함수 구현부는 handle[Event][Elem] <br> - arguments는 3개 넘어가면 객체 형태로 구성|
| 폴더, 파일명 | - 대부분 kebab-case <br> - 컴포넌트성 파일만 PascalCase.tsx|
| curly brace | - 사용한다! early return 등에서 조건 실행문이 짧거나 한줄이라도, 중괄호 무조건 포함 |
| 세미콜론 | - 사용|
| 함수 : function vs const | - const 화살표 함수를 지향한다. 하지만 function 형태로 만들어서 hoisting하는 것도 허용한다|
| single vs double quote | - 선호는 딱히 없음. 그래도 double로 통일 |

제일 뜨거웠던 항목은 "boolean 변수명" 이었습니다. 
쟁점 포인트는, boolean 변수명과, 어떤 대상이 boolean인지 체크하는 함수의 이름 구조였습니다.
isDisabled라는 이름은, 그 대상이 disabled 되었다는 변수로도 사용할 수 있지만 isDisabled(something) 와 같이 체크하는 함수로도 사용할 수 있습니다.

그래서 함수명에 checkIsDisabled로 구분하자니 예쁘지 않고 매번 번거로울 것 같기도 했습니다. 
변수, 함수명 모두 isDisabled를 쓸 수 있지만 함수와 변수가 같이 나오는 상황에서는 함수가 우선한다? -> 이런 방법도 얘기가 나왔지만, 매번 어떤 방식으로 사용될지 이름으로 구분할 수 없으면 더 헷갈릴것이라는 의견도 있었습니다. 

그래서 이 부분은 합의가 나지 않고, 일단 각자 프로젝트에 적용해보고 다시 논의해보기로 하였습니다 ㅜ 

### lucky draw 테스트 코드 보완

기존에 lucky draw 실행 함수를 다음과 같이 분리했습니다

```js
const startLuckyDraw = () => {
  const randomIndex = Math.floor(Math.random() * prodList.length);
  const luckyItem = prodList[randomIndex];

  const isLucky = Math.random() < LUCK_THRESHOLD;
  const hasStock = luckyItem.quantity > 0;

  // 당첨됐고 재고가 있는 경우
  if (isLucky && hasStock) {
    alert(`번개세일! ${luckyItem.name}이(가) 20% 할인 중입니다!`);
    // 해당 상품의 가격 할인, DB에 적용
    luckyItem.price = Math.round(luckyItem.price * (1 - DISCOUNT_RATE.lucky));
    // select, option 업데이트

    updateSelectOptions();
  }
};
```

나름 깔끔하게 분리했다고 생각했으나, 테스트 코드를 작성하려고 보니 숨이 턱 막혔습니다. 
랜덤 확률이야 함수 결과를 mocking하면 되니까 상관 없었지만, 
함수 수행 전후로 전역 변수에 있는 값을 변경해줘야 했습니다. 테스트 이후 다시 전역 변수를 초기화해줘야 했습니다.
'함수가 발동하면 할인이 적용되는가' 핵심 로직을 테스트하기 위해, 부가적으로 설정해줘야 하는 부분이 많았습니다. 

'테스트하기 쉬운 코드인가?' 의 뜻을 이제야 알 수 있었습니다.
**현재 코드는 테스트하기 어려운 코드였습니다.** 

그래서 할인이 적용되는지를 테스트하기 쉽도록, 다음과 같이 함수를 분리했습니다.

```
const applyDiscount = (product, discountRate) => {
  return {
    ...product,
    price: Math.round(product.price * (1 - discountRate)),
  };
};
```

순수 함수로 구성하여, 해당 로직의 input, output을 간단하게 처리할 수 있었습니다.
'운이 좋다 -> 할인이 적용되고 alert 가 표시되며 ui가 업데이트된다' 라는 긴 시나리오를 세분화하여, 
'운이 좋다 -> 할인이 적용된다 -> alert가 표시된다 -> ui가 업데이트된다' 각 동작을 테스트할 수 있게 되었습니다.


### 심화 과제

react 와 typescript로 migration 하는 작업을 진행했습니다. 
기본 과제에서의 구조를 기반으로, 점진적으로 고도화했습니다. 
신경쓴 부분은 다음과 같습니다.

1. context로 데이터를 공유하자
2. 컴포넌트의 책임을 최소화하자

context를 생성할 관심사는 크게 2가지라고 생각했습니다. 재고 상태와, select 상태입니다.
select context에서도 재고 상태를 참조하기 때문에 분리하는게 맞나 싶었지만, 
어느정도 구분될 수 있는 관심사라 생각하여 분리했습니다.

state를 변경하는 로직은 컴포넌트 단에 직접 작성하지 않고, reducer를 미리 생성해둠으로써 
action type과 id 만으로 순수 함수를 호출할 수 있도록 했습니다. 
state에 접근할 수 있는 훅, 유틸함수를 생성함으로써, 컴포넌트를 세밀하게 분리할 수 있었습니다.


#### 테스트 코드

심화과제용 테스트 코드를 작성하였습니다.
기본 구조는 basic의 테스트 코드와 동일합니다. (vite config에 react plugin을 추가했습니다.)
test시 요소 선택을 용이하게 하기 위해, data-testid 를 추가해서 사용했습니다. 

basic과 기능이 동일하게 동작함을 보장하고
코드 수정 전후 의도치 않은 기능 누락이 생기지 않도록 하였습니다.

저는 업무 진행할 때 시간이 여유롭지 않아 테스트 코드를 작성하지 않았었습니다. 
이번에 테스트 코드를 어느정도 만들어두고 나니, 왜 테스트 코드를 만드는지 그 중요성을 이해할 수 있었습니다.
간단한 수정이고 크게 구조를 건들지 않았다고 생각했던 작업에서도, 테스트 코드 결과가 달라진 적이 종종 있었습니다.
그럴 때마다 디버깅하면서 제가 미처 생각하지 못했던 부분을 찾을 수 있었고, 그렇게 성장해 나가면서도 기능의 완전성을 보장할 수 있었습니다.
(이런거는 추후 테스트코드 챕터에서 더 많이 느끼겠지만..!)

#### html 기본 태그 props 재활용

리팩토링을 진행하며, '재활용, 확장 가능한 컴포넌트 만들기' 에도 신경을 썼습니다. 
컴포넌트를 분할하면, 제일 leaf에 위치한 컴포넌트는 html 기본 tag로 이루어집니다. 
예전에 개발할 때에는, 실제로 해당 컴포넌트에서 사용할 속성만 props에 정의를 했었습니다.
하지만 시간이 지나며 기능이 하나둘 추가되고, 그럴때마다 props에 속성을 추가하고 있는 모습을 발견했습니다.
이는 html 태그의 기본 attribute(onclick, value ...)에도 해당이 됐습니다.
그래서 전달하는 props가 추가되더라도 컴포넌트의 props 정의는 수정하지 않도록, rest 문법을 사용해 나머지 모든 props를 그대로 전달하도록 구성했으며, props interface에 html 태그 기본 attribute를 확장하도록 하였습니다.

```tsx
interface SelectProps extends React.HTMLAttributes<HTMLSelectElement> {}

export const Select: React.FC<SelectProps> = ({ children, ...props }) => {
  const { selectedId, setSelectedId } = useSelect();

  return (
    <select
      id="product-select"
      data-testid="product-select"
      className="border rounded p-2 mr-2"
      value={selectedId}
      onChange={(e) => setSelectedId(e.target.value)}
      {...props}
    >
      {children}
    </select>
  );
};
```

### 과제를 다시 해보면 더 잘 할 수 있었겠다 아쉬운 점이 있다면 무엇인가요?

챕터1에서 준일 코치님이 올려주신 솔루션 코드를 봤을 때, 되게 리액트스럽다고 생각했었습니다.
이번 과제에서 저도 최대한 리액트스럽게 짜보려고 했지만, 많이 부족했던 것 같습니다. 
스토어를 만들어 구독하고, 스토어에 변경사항이 발생했을 때 그것을 구독하고 있던 컴포넌트가 업데이트 되는 구조로 짜보고 싶었는데,
그럴만한 시간과 능력이 없었던 것 같습니다. 천천히 시간을 갖고 다시 도전해보도록 하겠습니다. 

### 리뷰 받고 싶은 내용이나 궁금한 것에 대한 질문 편하게 남겨주세요 :)

- 기본과제를 수행할때, react의 구조를 생각하면서 작업했습니다. 리액트에서의 컴포넌트 구조, 데이터 변경시 UI가 반영되는 흐름, 이벤트 핸들링 등 리액트를 바라보고 나아갔습니다. 근데 이게 어떻게 보면 정답지를 머릿속에 넣고, 현재 구조를 거기에 맞추려고 하는 것과 같은데, 이게 정말로 올바른 과정인가? 싶은 의문이 조금 들긴 했습니다. 시야를 좁힌 채 앞만 보고 달리는 말과 같달까요.. ㅎㅎ 혹시 이런 부분에서 우려하셨던 점은 없으신가요?
- hook은 UI에 종속되어도 괜찮은가에 대한 질문입니다.
  - 여러 컴포넌트에서 공용으로 사용할 데이터 'A' 를 불러오는 hook인 useA() 가 있다고 가정하겠습니다.
  - 한 컴포넌트에서는, 'A'를 가공해서 'B'를 만들고, 이를 사용합니다. 
  - 이 컴포넌트에서 B를 사용하는 방법은 크게 두가지가 있다고 생각하는데,
     1. useA()를 호출해서 A를 얻고, 가공해서 B를 만들어 사용
       ```js
         const A = useA()
         const B = 가공(A)
       ``` 
     2. 가공해서 B를 만들어 리턴하는 useB hook을 별도로 만들어 사용
       ```js
         const useB = ()=>{
           const A = useA()
           const B = 가공(A)
         }
         const B = useB()
       ```
     - 코치님은 어떤 방식을 선호하시나요? 저는 사용하는 곳이 적더라도 2번 방식을 사용했습니다. 근데 만약 그 컴포넌트를 없애야 한다면 거기서만 사용하던 그 훅도 같이 없애야하는, 훅이 컴포넌트에 종속된 양상이 아닌가? 싶어서요. 훅은 컴포넌트와 상관없이 어떤 근원적인 데이터를 가져오는데에만 사용하고, 가공이 필요하다면 가공을 해서 사용하지 굳이 훅으로 만들면 안된다. 이런 입장도 본 것 같아서요. '컴포넌트가 사라진다고 훅이 사라지는게 말이되냐' 이런 입장을 들으니 공감이 되긴 해서.. 혹시 코치님은 이에 관해 어떻게 생각하시나요?
 
- boolean 관련 변수, 함수명 질문입니다.
  -  위에서 언급했듯이 isDisabled 라는 이름은 변수명으로도, 체크하는 함수명으로도 사용할 수 있을 것 같습니다. check를 붙일 수 있지만 뭔가 안예뻐지는 것 같아서요. 혹시 이런 상황을 코치님은 어떻게 구분하고 계신지 궁금합니다.
