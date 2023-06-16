# Assignment-PetDog
class Pet:
    # define constructor with name and age as parameters
    def __init__(self, name, age):
        self.name = name
        self.age = age
    # create display method fro Pet class
    def display(self):
        print("Pet name : ", self.name)
        print("Pet age = ", self.age)
    
# create child class Dog of Pet class
class Dog(Pet):
    # define constructor of Dog class with section additional parameters 
    def __init__(self, name , age , section):
        Pet.__init__(self,name, age)
        self.section = section
    
    # Create display method for Dog class
    def displayDog(self):
        print("Dog name : ", self.name)
        print("Dog age = ", self.age)
        print("Dog breed= ", self.breed)

class JackRussellTerrier(Dog):
    pass

class Dachshund(Dog):
    pass

class Bulldog(Dog):
    pass
def bark(self):
        print("Woof!")

my_dog = Dog("Rex", "SuperDog")
# Remember python implicitly passes in "self",
# so we don't need to pass it in when we call the function!
my_dog.bark()
# Testing Pet class
P = Pet("Dog", 7)
P.display()
print("-------------------------------")
S = Dog("JackRussellTerrier", 9,)
S.display()
