            ### Bye ###
from typing import Text
import pyttsx3 
engine = pyttsx3.init()  # object creation
########################## Details #################
###### RATE
rate = engine.getProperty('rate')   # getting details of current speaking rate

engine.setProperty('rate', 150)     # setting up new voice rate

####### VOLUME
volume = engine.getProperty('volume')   #getting to know current volume level (min=0 and max=1)
engine.setProperty('volume',1)    # setting up volume level  between 0 and 1

###### VOICE
voices = engine.getProperty('voices')       #getting details of current voice
#engine.setProperty('voice', voices[0].id)  #changing index, changes voices. o for male
engine.setProperty('voice', voices[1].id)   #changing index, changes voices. 1 for female

### sey ###
text1 = ("nok nok....")
print(text1)
engine.say(text1)
engine.runAndWait()
#_________________________X________________________#
### name ###
text2 =("what's your name?")
print(text2)
engine.say(text2)
engine.runAndWait()
n = input("Enter only name :")
#_________________________X________________________#
### hey ###
text3 = ('Hey',n,'How are you?')
print("Hey",n,"How are you ?")
engine.say(text3)
engine.runAndWait()
ad = input("ans in(fine /quite well) :",)
#_________________________X________________________#

######## AD ##########
     ### fine ###
if (ad=="fine"):
    text4 = ("That's good")
    print (text4)
    engine.say(text4)
    engine.runAndWait()
      ### Quite well ###
elif (ad=="quite well"):
    text5 = ("Are you sick")
    print = (text5)
    engine.say(text5)
    engine.runAndWait()
      ### nathing ###
else :
     print ()
#_________________________X________________________#
text = ("ok,Bye .  Wish you good luck")
print("ok!Bye. Wish you good luck" )
engine.say(text)
engine.runAndWait()
#_________________________X________________________#

engine.runAndWait()
engine.stop()
print("<<<----------End---------->>>")
