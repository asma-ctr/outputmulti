# outputmulti
selection 
#import sound pip into the system
import pyttsx3
import random


    #Print Main Menu

print("1: LOTTO ")
print("2: EUROJACKPOT ")
print("3: VIKING LOTTO ")



#Making Menu Selection for User 
lottonum = int(input("Choose Your Option Between 1 to 3: "))

engine = pyttsx3.init()

engine.say("You have choosen number")
engine.runAndWait()
print("You have choosen number:",lottonum)
    

#Functions for LOTTO, VIKING LOTTO and eurojackpot.
#The functions is for numbers and extra numbers
#And function for text spech library
def lotto():
    engine = pyttsx3.init()
    engine.say("How many row do you want")
    engine.runAndWait()

    rader= int(input("How many row do you want"))
    print("\n Lotto numbers is ", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,40), 7)
        x.sort()
        print(x)
    
def lottot():
    engine = pyttsx3.init()
    engine.say("extra numbers is")
    engine.runAndWait()
    
    rader= 1
    print("\n extra numbers is ", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,40), 1)
        x.sort()
        y = type(x)
        print(str(x),(y))

   
def euro():
    engine = pyttsx3.init()
    engine.say("How many row do you want")
    engine.runAndWait()
    
    rader= int(input("How many row do you want"))
    print("\n eurojackpot numbers", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,50), 5)
        x.sort()
        print(x)

def eurot():
    engine = pyttsx3.init()
    engine.say("extra numbers is")
    engine.runAndWait()
    
    rader= 2
    print("\n extra numbers is", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,12), 2)
        x.sort()
        y = type(x)
        print(str(x),y)
        
def viking():
    engine = pyttsx3.init()
    engine.say("How many row do you want")
    engine.runAndWait()
    
    rader= int(input("How many row do you want"))
    print("\n VIKINGLOTTO numbers", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,48), 6)
        x.sort()
        print(x)

def vikingt():
    engine = pyttsx3.init()
    engine.say("extra numbers is")
    engine.runAndWait()
    
    rader= 1
    print("\n extra numbers is", rader)
    for i in range(rader):
        x=arvonta = random.sample(range(1,5), 1)
        x.sort()
        y = type(x)
        print(str(x),y)
        

#Take Action On menu and selecting.

if lottonum == 1:
    
    print("LOTTO ", lotto(), lottot())
    

    
      
elif lottonum == 2:
    
        
    print("EUROJACKPOT ", euro(), eurot())


        
        
elif lottonum == 3:
            print("VIKING LOTTO ", viking(), vikingt())


#THE END
