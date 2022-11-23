### Variables란?
- 값을 저장하고, 이를 참조할 수 있다(필요할 때 꺼내쓸 수 있다)

#### 선언 방식
> Type 지정, 초기화
> - ex) val appName : String = “TaeHoon”


- val : 변수 키워드
- appName : 변수명
- String : 변수 타입
- Shoppi : 변수에 저장할 값

>Type 생략, 초기화
> - ex) val userName = “ivy”

- val : 변수 키워드
- userName : 변수명
- ivy : 저장할 값

예시1과 다른점 : 변수 타입이 생략된 것
타입을 생략할 수 있다 == 타입이 무엇인지 추론할 방법이 있다

위 2개 변수의 공통점 : 키워드 val을 사용한다

#### 키워드
- val : 변경이 불가능한 변수, immutable

``` kotlin
val appName : String = “Shoppi”
appName = “KotlinApp”
#이렇게 코딩을 하면 에러가 발생하겠죠?
#이유 : appName을 val로 선언했기 때문에 
```

- var : 변경 가능한 변수, mutable

``` kotlin
var userName = “ivy“
userName = “1234”
```

변수명을 짓는 규칙
- 변수명은 Camel case를 따른다 (lower camel case)

예시
> - val variable = “var”
> - val nonConstScalar = “non-const”
> - val mutableCollection: MutableSet = HashSet()
> - val mutableElements = listOf(mutableInstance)
> - val mutableValues = mapOf(“Alice” to mutableInstance, “Bob” to mutableInstance2)
> - val logger = Logger.getLogger(MYClass::class.java.name)
> - val nonEmptyArray = arrayOf(“these”, “can”, “change”)

규칙
1. 변수의 시작은 늘 소문자
2. nonConstScalar, mutableCollection처럼 새로운 단어와의 연결은 대문자
3. 명사, 명사구로만 변수를 짓는다
4. 변수의 용도를 명확히 드러내는 이름으로 짓는다
