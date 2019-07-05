### 1. 변수와 함수명은 camelCase (단, 상수는 UPPER_CASE, 클래스는 PascalCase)
```js
// good
let myName = 'itholic';

function printMyName(name) {
    console.log(myName);

class SsafySeoul1 extends object {
    
}
};

// bad
let my_name = 'itholic';

function print_my_name(name) {
    console.log(my_name);
};
```

### 2. 상수(const)는 UPPER_CASE로 명확히 표현
```js
// good
const NAME = "itholic";

// bad
const name = "itholic";
```

### 3. 변수 선언시 var대신 let이나 const를 사용
```js
// good
let a = 1;

// bad
var a = 1;
```

### 4. 한 번에 하나의 변수만 선언
```js
// bad
let a = 1,
    b = 2,
    c = 3;

// good
let a = 1;
let b = 2;
let c = 3;
```

### 5. 파일명은 lower-case로 작성 (혼재해서 사용하지 말것)
```js
// good
coding-convension.js
coding-style-guide.js

// bad
codingConvension.js
coding_style-guide.js
```

### 6. 들여쓰기는 2칸 공백
```js
// good
function foo() {
  var a
}

// bad
function foo() {
    var a
}
```

### 7. 문장의 끝에 세미콜론 기재를 권유 (자바스크립트는 세미콜론이 강요되지 않음)
```js
var a1 = 10;

functions foo() {
    var a2 = 20;
};
```

### 8. Arrow Function으로 표현할 수 있는 부분은 가급적 Arrow Function으로 표현할 것
```js
// good
[1, 2, 3, 4, 5].map((x) => x * x);

//bad
[1, 2, 3, 4, 5].map(function(x) {
    return x * x; 
});
```

### 9. 문자열 연결시 + 보다는 탬플릿 문자열로 표현 (따옴표 모양 유심히 볼 것)
```js
let name = "itholic";

// good
console.log(`My name is ${name}`);

// bad
console.log("My name is " + name);
```

### 10. 문자열은 큰따옴표(“) 보다는 작은따옴표(‘)를 사용, 문자열에 작은따옴표 포함시 탬플릿 문자열 사용 (`)
```js
// bad
let introduce = "i am itholic"

// good
let introduce = 'i am itholic' 

// good
let introduce = `i'm itholic`
```