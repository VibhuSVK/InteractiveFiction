# InteractiveFiction
#begining also most of the code is defining
def bedroom():
    print(" 
 __________________________
|  ______________________  |
| |   ___    ___   ___   | |
| |  | __)()(__ ) / _ \  | |
| |  |__ \   (_ \( (_) ) | |
| |  (___/()(___/ \___/  | |
| |______________________| |
|__________________________|
")
    print("Beep Beep Beep. You slam your alarm clock. The clock's display says, 'Fri - 8/6/97 - 5:30'. You have to be at work by seven.")
    sleep_answer = str(raw_input("Would you like to sleep in?"))
    if sleep_answer == "yes" or "sleep in" or "sleep" or "keep sleeping":
        print("")
    if sleep_answer == "no" or "get up" or "wake up" or "stop sleeping":
        hall()
    else:
        print("Word not recognized")
        bedroom()

def hall():
    print("You get up and yawn. As you get up your nakedness becomes apparent. You open your closet and put on the pink bath robes. Your stomach gargles but at the same time your bladder feels full.")
    hall_answer = str(raw_input("Do you want to go the bathroom or go downstairs?"))
    if hall_answer == "bathroom" or "go to the bathroom" or "pee":
        bathroom()
    if hall_answer == "downstairs" or "go downstairs" or "stairs":
        downstairs()
    else:
         print("Word not recognized")
         hall()

def bathroom():
    print("As you relieve yourself you look in the mirror. You see the bags underneath your eyes. You aren't quite sure what happened last night, but based on the smell of your breath it probably happened at the bar.")
    bathroom_answer = str(raw_input("Go downstairs?"))
    if bathroom_answer == "yes" or "downstairs" or "go downstairs":
        downstairs()
    if bathroom_answer == "no":
        print ("You hear agressive knocking at your front door. You ignore it as you are in the middle of releasing a big one. A few minutes later, as you are cleaning up, you hear a large bang at the front door. As you exit the bathroom two men grab your arm and drag you down the stairs out to the front porch.")
        porch()
    else:
        print("Word not recognized")
        bathroom()

def downstairs():
    print("As you walk down the stairs you see that your living room is a mess. You left the TV on, you curse yourself. The bills are going to be much higher this month.")
    livingroom_answer = str(raw_input("Do you want to turn off the TV, or go eat breakfast?"))
    if livingroom_answer == "TV" or "television" or "turn off" or "turn off TV" or "turn TV off":
        television()
    if livingroom_answer == "food" or "eat" or "breakfast" or "kitchen" or "eat breakfast":
        breakfast()
    else:
        print("Word not recognized")
        downstairs()

def television():
    print("As you walk towards your television you hear the name 'Rupert Mann' spoken. You stop for a moment as that is your name. The newscaster says that Rupert Mann has just become the richest man in Los Angeles.")
    television_answer = str(raw_input("You hear an agressive knocking at the door. Do you ignore the knocking and eat your breakfast?"))
    if television_answer == "door" or "knocking" or "front door" or "open door" or "don't ignore":
        frontdoor()
    if television_answer == "food" or "eat" or "breakfast" or "kitchen" or "eat breakfast" or "ignore":
        breakfast()
    else:
        print("Word not recognized")
        television()
       
def breakfast():
    print ("You open your refrigerator. There is a cup of spoiled milk, some sliced ham, a bowl of cheerios, a head of lettuce, and some vegan sausages. You grabthe bowl of cheerios and start eating them.")   
    breakfast_answer = str(raw_input("As you stare blankly at your cheeriosm you hear an agressive knocking at the fromt door. The television is still on."))
    if breakfast_answer == "door" or "knocking" or "front door" or "open door":
        frontdoor()
    if breakfast_answer == "TV" or "turn off" or "turn off TV" or "turn TV off" or "television":
        television()
    else:
        print("Word not recognized")
        breakfast()
        
        
#start to run the code
bedroom()
