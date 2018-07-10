### THIS IS A SAMPLE CODE FOR PYTHON LEARNING FOR NEW BEES ###

import mysql.connector

#single line comment - my first python
""" multiline comment
This is just a filing sentence
"""
if 5 > 2:
    print("Greater")
    __variable='vivek'
    print(__variable)
    print("contatenation done with:" + __variable)
    print(type(__variable))
    __variable=1
    print(type(__variable))
    __variable=1.8
    print(type(__variable))

    __type=1
    print(int(__type))
    __type=1.8
    print(str(__type))
    __type="1"
    print(float(__type))


    __string="vivek"
    print(__string[0])
    print(__string[0:4])
    print(len(__string))
    print(__string[0:len(__string)])
    print(__string[0:3])

    __string="        Vivek"
    print("Before removing white space:" + __string)
    print("After removing whitespace:" + __string.strip())


    __string="VIVEK"
    print(__string.lower())
    __string="vivek"
    print(__string.upper())


    __string="This is a string"
    print(__string)
    print(__string.replace("string","replacedstring"))


    __string="This, is, a, string"
    print(__string.split(","))

##    print("Input a string")
##    __inputstring=input()
##    print("You entered : " + __inputstring)
    
    __integer=3
    print("* operated result of 3 with 3: " + str(__integer*3))
    print("** operated result of 3 with 3: " + str(__integer**3))
    print("// operated result of 3 with 2: " + str(__integer//2))
    print("& operated result of 3 with 2 : " + str(__integer&2))
    print("| operated result of 3 with 2 : " + str(__integer|2))
    print("^ operated result of 3 with 4 : " + str(__integer^4))    
    print("<< operated result of 3 with 3 : " + str(__integer<<3))
    print(">> operated result of 3 with 3 : " + str(__integer>>3))
    

    __integer1=1
    __integer2=2
    print(not(__integer1>1))
    print(not(__integer1>0 or __integer2>__integer1))
    print(__integer1>__integer2 and __integer2>__integer1)
    print(__integer1<__integer2 or __integer2<__integer1)


    __identityobject1=['sun','moon']
    __identityobject2=['sun','moon']
    __identityobject3 = __identityobject1
    print(__identityobject1 is __identityobject2)
    __identityobject1 = __identityobject3
    print (__identityobject1 is __identityobject3)
    print(__identityobject1 is not __identityobject2)
    print(__identityobject1 is not __identityobject3)
##    print(__identityobject1 <> __identityobject3)

    __mylist=['sun','moon','star1','star2']
    print(__mylist)
    print("Fist in list 0 value is: " + __mylist[0])
    print("Append star3 to __mylist")
    __mylist.append("star3")
    print(__mylist)
    print("Remove star2 from __mylist")
    __mylist.remove('star2')
    print(__mylist)
    print("Length of list: " + str(len(__mylist)))
    __mylistcopy = list(__mylist)
    print("My list copy: " + str(__mylistcopy))
    print(__mylistcopy.count('moon'))
    __mylistcopy.append('star4')
    print("mylistcopy after append : " + str(__mylistcopy))
    __mylistcopy.extend(__mylist)
    print("mylistcopy after extended to mylist : " + str(__mylistcopy))
    __mylistcopy.insert(0, 'zero')
    print("mylistcopy insert 0 at first : " + str(__mylistcopy))
    __mylistcopy.remove('star1')
    print("mylistcopy after removed from star1 : " + str(__mylistcopy))
    print("mylistcopy index of star1" , __mylistcopy.index('star1'))
    print("mylistcopy count of sun" , __mylistcopy.count('sun'))
    __mylistcopy.pop(0)
    print("mylistcopy after pop of 0th element zero", __mylistcopy)
    __mylistcopy.reverse()
    print("mylistcopy reverse" , __mylistcopy)
    __mylistcopy.sort()
    print("mylistcopy sorted" , __mylistcopy)
    __mylistcopy.sort(reverse=True)
    print("mylistcopy sorted reverse" , __mylistcopy)
    __mylistcopy.sort(key=len)
    print("mylistcopy sorted by len of item" , __mylistcopy)
##    __mylistcopy.clear()
##    print("mylistcopy cleared and items now are" , __mylistcopy)



    __mytuple = ('ball','bat','stump')
##    __mytuple[1]='balls'
##    print('my tuple updated', __mytuple)

##    __myset = {"ball1","bat1","stump1"}

    __mydict = {'apple':'greeen', 'banana':'yellow', 'cherry':'red'}
    print(__mydict)
    __mydict['apple']='yellow'
    print(__mydict)
    
    __mydict1 = dict({'apple':'greeen', 'banana':'yellow', 'cherry':'red'})
    del(__mydict1['banana'])
    print(__mydict1)

    print(len(__mydict1))

__i = 1
while __i < 5:
    if __i ==4:
        break
    print(__i)
    __i+=1
    

__string='For loop string'
for __i in __string:
    print("This is for loop string ripped:", __i)
    
for __string in range(0, len(__string)):
    print("This is for loop string ripped by range:", __string)

for __i in range(0,16,3):
    print(__i)
    
def func1():
    print("First Function")
func1()

def func2(__param1="defaultvalueParameter1"):
    print("First Function with parameter", __param1)
func2("P1")
func2()

def myfunc(__n):
  return lambda __i: __i*__n

__myfuncoutput = myfunc(2)
print(__myfuncoutput)
__val=11
print(__myfuncoutput(__val))


__array = ["Ford", "Volvo", "BMW"]


__db=mysql.connector.connect(
    host='localhost',
    user='root',
    passwd='dell123'
    )

print(__db)
