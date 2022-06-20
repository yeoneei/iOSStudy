# Any, AnyObject, nil



* Any : Swift의 모든 타입을 지칭하는 키워드
* AnyObject : 모든 클래스 타입을 지칭하는 프로토콜
* nil : 없음을 의미하는 키워드

```swift
import Swift

// Any - 모든 타입을 수용할 수 있다
var someAny: Any = 100
someAny = "어떤 타입도 수용 가능합니다."
someAny = 123.12

let someDouble: Double = someAny // error

// AnyObject - class instance만 가능
class SomeClass {}

var someAnyObject: AnyObject = SomeClass()
someAnyObject = 123.12 // error

// nil - null과 유사
someAny = nil // error - Any 타입이여도 nil은 불가능

```

