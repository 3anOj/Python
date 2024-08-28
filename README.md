# Python

# Generator
def cinema(hero,heroine,comedian):
    yield hero                     # # yield is a keyword
    yield heroine
    yield comedian
en=cinema("Nagarjuna","Anushka","Ali")
print(next(en))
print(next(en))
print(next(en))

Output:-
Nagarjuna
Anushka
Ali

# Iterator
groceries=["tomato","Apple","Ariel"]
md=iter(groceries) #here iter is a method
print(next(md))
print(next(md))
print(next(md))

output:-
tomato
Apple
Ariel

# Decorator
def greet(func):
    def md():
        print("Hello")
        func()
        print("see you soon")
    return md
@greet
def name():
    print("I am manoj nice to meet you")
@greet
def city():
    print("I am from HYD")
    
name()
city()

output:-
Hello
I am manoj nice to meet you
see you soon
Hello
I am from HYD
see you soon

# Exceptions
# 1
a = 10
b = 2
try:
    result = a / b
except ZeroDivisionError:
    print("Cannot divide by zero!")
else:
    print("Division successful:", result)
finally:
    print("This will always run.")

output:- 
Division successful: 5.0
This will always run.
# 2
a = 10
b = 0
try:
    result = a / b
except ZeroDivisionError:
    print("Cannot divide by zero!")
else:
    print("Division successful:", result)
finally:
    print("This will always run.")

Output:-
Cannot divide by zero!
This will always run.

