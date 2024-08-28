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
