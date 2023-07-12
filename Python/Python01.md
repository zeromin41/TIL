#### 함수의 매개변수

매개 변수(=Parameter)는 함수를 선언할 때 사용되는 변수를 가르킴.

매개 변수는 함수를 호출할 때 지정되는 인자를 함수의 본문에 전달하는 역할을 수행함.

매개 변수는 함수를 정의할 때 사용되는 특별한 변수이며, 함수 내부에서만 의미를 갖기에 대표적인 지역 변수이다.

위치인자
>인자를 지정된 위치에 사용해야 함.

키워드 인자 
>키워드와 함께 지정되는 인자. 해당 인자의 기본값을 미리 지정한 후에 상황에 따라 다른 인자를 사용하는 것을 허용하고자 할 때 사용하는 인자. 위치 인자를 받는 매개 변수는 키워드 인자를 받는 키워드 매개 변수보다 먼저 선언되어야 함.

※반드시 위치인자 먼저 지정후 키워드 인자 지정해야함
```
Help on built-in function print in module builtins:

print(...)
    print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
    
    Prints the values to a stream, or to sys.stdout by default.
    Optional keyword arguments:
    file:  a file-like object (stream); defaults to the current sys.stdout.
    sep:   string inserted between values, default a space.
    end:   string appended after the last value, default a newline.
    flush: whether to forcibly flush the stream.
```
위에서 print()함수는 4개의 키워드 인자를 가짐.

#### 객체

파이썬이 다루는 대상(값)은 모두 객체(object), 즉 특정 클래스의 인스턴스임. 따라서 값과 관련된 적절한 메서드를 활용할 수 있어야 함.

#### 객체의 속성과 메서드

모든 객체는 속성과 메서드를 갖음.

속성
> 객체 안에 포함된 값 또는 해당 값에 대한 정보

메서드
> 객체 안에 포함된 값을 조작하는 함수

#### 동적참조

변수에 할당된 값은 심지어 다른 자료형의 값으로 변경될 수 있으며, 그에 따른 자료형의 정보도 함께 변경되어 저장됨.
