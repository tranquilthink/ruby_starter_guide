# 기본 문법

Ruby의 기본 문법에 대해 알아보겠습니다. 기본 문법은 Ruby 코드를 작성하는 데 필요한 핵심 요소들을 다룹니다. 아래는 다양한 주제를 다루는 세부 섹션들로 구성된 목차입니다:

- [[변수와 데이터 타입]](basic-syntax.md#변수와-데이터-타입)
- [[연산자]](basic-syntax.md#연산자)
- [[조건문]](basic-syntax.md#조건문)
- [[반복문]](basic-syntax.md#반복문)
- [[함수와 메서드]](basic-syntax.md#함수와-메서드)

각 섹션에서는 해당 주제에 대한 설명과 예제 코드를 제공하여 Ruby의 기본 문법을 이해하고 활용할 수 있도록 도와줍니다. 아래에서 각 섹션에 대한 간략한 소개와 예시 코드를 제공합니다:

## 변수와 데이터 타입

변수는 값을 저장하는 데 사용되며, Ruby에서는 변수의 타입을 사전에 선언할 필요가 없습니다. 다음은 변수와 데이터 타입에 대한 예시 코드입니다:

```ruby
# 변수 선언과 할당
name = "John"
age = 30
is_student = true

# 데이터 타입
puts name.class # String
puts age.class # Integer
puts is_student.class # TrueClass
```

## 연산자

Ruby에서는 다양한 연산자를 사용하여 산술, 할당, 비교 등의 작업을 수행할 수 있습니다. 다음은 연산자에 대한 예시 코드입니다:

```ruby
# 산술 연산자
result = 10 + 5
puts result # 15

# 할당 연산자
x = 10
x += 5
puts x # 15

# 비교 연산자
is_equal = 10 == 5
puts is_equal # false
```

## 조건문

조건문은 프로그램의 실행 흐름을 제어하는 데 사용됩니다. Ruby에서는 `if`, `elsif`, `else`와 같은 키워드를 사용하여 조건문을 작성할 수 있습니다. 다음은 조건문에 대한 예시 코드입니다:

```ruby
# if문
x = 10
if x > 5
  puts "x는 5보다 큽니다."
elsif x < 5
  puts "x는 5보다 작습니다."
else
  puts "x는 5입니다."
end
```

## 반복문

반복문은 특정한 작업을 반복하여 수행하는 데 사용됩니다. Ruby에서는 `while`, `for`, `each`와 같은 반복문을 사용하여 반복 작업을 처리할 수 있습니다. 다음은 반복문에 대한 예시 코드입니다:

```ruby
# while문
x = 1
while x <= 5
  puts x
  x += 1
end

# for문
for i in 1..5
  puts i
end

# each문
[1, 2, 3, 4, 5].each do |num|
  puts num
end
```

## 함수와 메서드

함수와 메서드는 코드의 재사용성을 높이고 프로그램의 구조를 모듈화하는 데 사용됩니다. Ruby에서는 `def` 키워드를 사용하여 함수와 메서드를 정의할 수 있습니다. 다음은 함수와 메서드에 대한 예시 코드입니다:

```ruby
# 함수 정의와 호출
def greet(name)
  puts "안녕, #{name}!"
end

greet("John") # 안녕, John!

# 메서드 정의와 호출
class Person
  def initialize(name)
    @name = name
  end

  def say_hello
    puts "안녕, 나는 #{@name}이야!"
  end
end

person = Person.new("Alice")
person.say_hello # 안녕, 나는 Alice이야!
```

각 섹션에서는 상세한 내용과 함께 예제 코드를 제공하여 Ruby의 기본 문법을 학습할 수 있도록 안내합니다.