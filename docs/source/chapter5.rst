chapter 5: Storing and Modifying Information
================================================

이 장에서는 다음을 배우게 될것이다.

.. sourcecode:: pycon

    ▶ Understanding data storage
    ▶ Considering the kinds of data storage
    ▶ Adding dates and times to applications



5.1 Storing Information
----------------------------

데이터를 저장하는 방법들은 많다.
파이썬도 여러가지 데이터 타입이 있는데 앞으로 데이터 타입을 공부하게 될것이다.


.

5.2 Defining the Essential Python Data Types
-----------------------------------------------

모든 프로그램에서는 변수(variables)들을 사용한다.
변수의 종류를 데이터 타입이라고 한다.
많은 연습을 통해 변수의 정확한 개념을 이해하는것이 중요하다.
단지 어떤 양을 저장하기 위한 그릇이라고 생각하면 된다.
그런데 그 그릇이 다양한 형태로 존재 하는것이다.
양에 따라서 저장하는 여러가지 그릇이 존재한다고 생각하면 쉽다.

다음을 실행해 보자.

.. code-block:: python

    Myvar=5

위에서 =는 할당 연산자로 한다. Myvar에 5를 넣으라는 것이다.


Understanding the Numeric types
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
숫자만을 넣는 데이터 타입들이 있다.

Integer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

integer 데이터 타입은 –9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807 숫자를 넣을 수 있다.

int 타입은 2(binary),8(octet),16(hex) 형태로 표현을 할 수 있다.

.. sourcecode:: pycon

    ✓ Base 2: Uses only 0 and 1 as numbers.
    ✓ Base 8: Uses the numbers 0 through 7.
    ✓ Base 10: Uses the usual numeric system.
    ✓ Base 16: Is also called hex and uses the numbers 0 through 9 and the letters
    A through F to create 16 different possible values.



그리고 출력 표현도 다음과 같이 할 수 있다.

.. sourcecode:: pycon

    ✓ b: Base 2
    ✓ o: Base 8
    ✓ x: Base 16

예를 들면 integer 4 는 0b100 (2 binary)

다음을 출력해 보자.

.. code-block:: python

    test=0b100
    print(test)
    test2=0o100
    print(test2)
    test3=0x100
    print(test3)


Floating-point values
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

정수를 포함한 소스까지 확대된 숫자의 데이터 타입이다.

±1.7976931348623157 × 10308 ~  ±2.2250738585072014 × 10-308

다음을 출력해 보자.

.. code-block:: python

    test=255
    print(test)
    test2=2.55e2
    print(test2)
    test3=2.55e-2
    print(test3)

Complex numbers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

복소수이다.

복소수가 쓰이는 분야는 다양하다.

.. sourcecode:: pycon

    ✓ Electrical engineering
    ✓ Fluid dynamics
    ✓ Quantum mechanics
    ✓ Computer graphics
    ✓ Dynamic systems

다음을 출력해 보자.

.. code-block:: python

    myComplex=3 + 4j
    print(myComplex.real)
    print(myComplex.imag)


Understanding Boolean values
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

True or False 값을 리턴하거나 할당하는데 쓰인다.


Understanding strings
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

사람이 인식하는 문자를 담는 변수를 string이라고 한다.

myString ="Python is a great language."

string을 int,float 타입으로 변환하려면 int(),float() 함수를 쓰면 된다.

myInt=int("123")

myInt 값은 Integer 변수이다.

다음을 출력해 보자.

.. code-block:: python

    myInt=int("123")
    print(myInt)
    print(type(myInt))

.. code-block:: python

    myStr=str(123.56)
    print(myStr)
    print(type(myStr))

5.3 Working with Dates and Times
-----------------------------------

시간 모듈을 import하여  시간을 출력하는 예제를 실행해 보자.


.. code-block:: python

    import datetime
    print(datetime.datetime.now())
    print(str(datetime.datetime.now().date()))



Algorithms Train
--------------------------------------------


01.Codeforces_L01P01_1118A.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


02.Codeforces_L01P02_677A.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


03.Codeforces_L01P05_673A.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


04.complete_the_pattern_number_8_number_pyramid.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


05.complete_the_pattern_number_9_diamond.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


06.count_the_smiley_faces.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


07.detect_pangram.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


08.duplicate_encoder.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


