# 컬렉션 타입 (Array, Dictionary, Set)

* 컬렉션 타입 : 여러 값들을 묶어 하나의 변수로 표현하게 해줌
* Array : 순서가 있다. index 존재
* Dictionary : 해쉬랑 비슷, 키 + 값 존재
* Set : 집합, 한 요소들의 집합, 순서 없음

```swift 
var integers: Array<Int> = Array<Int>()
integers.append(1) // [1]
integers.append(100) // [1, 100]
integers.append(101.1) // error

integers.contains(100) // true
integers.contains(99) // false

integers.remove(at: 0) // 1
integers.removeLast() // 100
integers.removeAll() // []

integers.count // 0

var doubles: Array<Double> = [Double]() // Array<Double>과 [Double]은 같은 표현
var characters: [Character] = [] // []은 빈 array

let immutableArray = [1,2,3] // 변경 불가능 append remove 불가

var anyDictionary: Dictionary<String, Any> = [String: Any]()
anyDictionary["someKey"] = "value"
anyDictionary["anotherKey"] = 100

anyDictionary.removeValue(forKey: "anotherKey")
anyDictionary["someKey"] = nil

anyDictionary // 빈 Dictionary

let emptyDictionary: [String: String] = [:] // 빈 상수 dictionary

// Set - 축약 문법이 없다!!
var integerSet: Set<Int> = Set<Int>()
integerSet.insert(1)
integerSet.insert(100)
integerSet.insert(99)
integerSet.insert(99)

integerSet // {100, 99, 1} - 중복된 값이 없다
integerSet.contains(1)
integerSet.contains(2)

integerSet.remove(100)
integerSet.removeFirst()

integerSet.count 

let setA: Set<Int> = [1, 2, 3, 4, 5]
let setB: Set<Int> = [3, 4, 5, 6, 7]

let union: Set<Int> = setA.uion(setB) // intersection (교집합), subtraction(차집합)
let sortedUnion: [Int] = uion.sorted() // Set은 정렬이 안됌. array로 정렬된 객체 생성


```

