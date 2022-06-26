chapter 7: Making Decisions
==============================

이 장에서는 다음을 배우게 된다.

.. sourcecode:: pycon

    ▶ Using the if statement to make simple decisions
    ▶ Performing more advanced decision making with the if...else statement
    ▶ Creating multiple decision levels by nesting statements


인간은 자연적으로 판단을 하게 되지만 컴퓨터는 매번 판단을 하기 위하여 다음의 임무를 수행한다.

.. sourcecode:: pycon

    1. Obtain the actual or current value of something.
    2. Compare the actual or current value to a desired value.
    3. Perform an action that corresponds to the desired outcome of the
    comparison.




7.1 Making Simple Decisions Using the if Statement
---------------------------------------------------

다음을 출력해 보자.

.. code-block:: python

    TestMe = 6
    if TestMe == 6:
       print("TestMe does equal 6!")


.. code-block:: python


    TestMe = 6
    if TestMe == 6:
       print("TestMe does equal 6!")
       print("All done!")

다음 코드는 입력된 값에 따라 해당 값을 프린트 하는 조건문이다.

.. code-block:: python

    Value = int(input("Type a number between 1 and 10: "))

    if (Value > 0) and (Value <= 10):
       print("You typed: ", Value)



7.2 Choosing Alternatives Using the if...else Statement
---------------------------------------------------------

선택의 상황이나 2가지 이상의 조건이 붙었을경우 처리하는 구문이다.
기본적 형태는 다음과 같다.

.. sourcecode:: pycon

    if  조건    :
        print("xxxx")
    else
        print("yyy")

다음 예제를 출력해 보자.

.. code-block:: python


    Value = int(input("Type a number between 1 and 10: "))

    if (Value > 0) and (Value <= 10):
       print("You typed: ", Value)
    else:
       print("The value you typed is incorrect!")




다음은 여려 조건이 있을경우 elif을 쓰는 법을 나타낸다.


.. code-block:: python

    print("1. Red")
    print("2. Orange")
    print("3. Yellow")
    print("4. Green")
    print("5. Blue")
    print("6. Purple")

    Choice = int(input("Select your favorite color: "))

    if (Choice == 1):
       print("You chose Red!")
    elif (Choice == 2):
       print("You chose Orange!")
    elif (Choice == 3):
       print("You chose Yellow!")
    elif (Choice == 4):
       print("You chose Green!")
    elif (Choice == 5):
       print("You chose Blue!")
    elif (Choice == 6):
       print("You chose Purple!")
    else:
       print("You made an invalid choice!")



7.3 Using Nested Decision Statements
----------------------------------------


조건이 2개 이상 발생할때 먼저 조건이 해결된후 다음 조건이 생겼을때 표현이다.
이럴경우는 if문 안에 다시 if문을 넣어 처리하게 된다.


다음 예제를 출력해 보자.

.. code-block:: python


    One = int(input("Type a number between 1 and 10: "))
    Two = int(input("Type a number between 1 and 10: "))

    if (One >= 1) and (One <= 10):
       if (Two >= 1) and (Two <= 10):
          print("Your secret number is: ", One * Two)
       else:
          print("Incorrect second value!")
    else:
       print("Incorrect first value!")

다음은 복합적인 if,elif 조건문 예제이다.


.. code-block:: python

    print("1. Eggs")
    print("2. Pancakes")
    print("3. Waffles")
    print("4. Oatmeal")
    MainChoice = int(input("Choose a breakfast item: "))

    if (MainChoice == 2):
       Meal = "Pancakes"
    elif (MainChoice == 3):
       Meal = "Waffles"

    if (MainChoice == 1):
       print("1. Wheat Toast")
       print("2. Sour Dough")
       print("3. Rye Toast")
       print("4. Pancakes")
       Bread = int(input("Choose a type of bread: "))

       if (Bread == 1):
          print("You chose eggs with wheat toast.")
       elif (Bread == 2):
          print("You chose eggs with sour dough.")
       elif (Bread == 3):
          print("You chose eggs with rye toast.")
       elif (Bread == 4):
          print("You chose eggs with pancakes.")
       else:
          print("We have eggs, but not that kind of bread.")

    elif (MainChoice == 2) or (MainChoice == 3):
       print("1. Syrup")
       print("2. Strawberries")
       print("3. Powdered Sugar")
       Topping = int(input("Choose a topping: "))

       if (Topping == 1):
          print ("You chose " + Meal + " with syrup.")
       elif (Topping == 2):
          print ("You chose " + Meal + " with strawberries.")
       elif (Topping == 3):
          print ("You chose " + Meal + " with powdered sugar.")
       else:
          print ("We have " + Meal + ", but not that topping.")

    elif (MainChoice == 4):
       print("You chose oatmeal.")

    else:
       print("We don't serve that breakfast item!")


Algorithms Train
--------------------------------------------

01-01.IfElif.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-02.IfElse.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-03.MultipleIfElif.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-04.MultipleIfElse.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-05.SimpleIf1.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-06.SimpleIf2.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


01-07.SimpleIf3.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


02.detect_anagram.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


03.remove_nth_Index.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


04.form_new_string.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


05.count_number.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


06.take_in_string.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


07.calculate_string.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


08.function_composition.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


09.generating_numbers_from_digits_number_1.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


10.get_your_steppin_on_son.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


11.grouped_by_commas.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


12.help_the_bookseller.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


13.how_much.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


incrementCipher.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


isCryptSolution.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


isIdentityMatrix.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


isIPv4Address.py
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




