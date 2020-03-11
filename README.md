# InteractiveFiction
#begining also most of the code is defining
def bedroom():
    
    print("Beep Beep Beep. You slam your alarm clock. The clock's display says, 'Fri - 8/6/97 - 5:30'. You have to be at work by seven.")
    sleep_answer = (raw_input("Would you like to sleep in?"))
    print ("")
    if sleep_answer == "yes" or sleep_answer == "sleep in" or sleep_answer == "sleep" or sleep_answer == "keep sleeping":
        print("You drift back to sleep")
        print("")
        print("")
        print("You wake to the feeling of your arm being grabbed. You try to fight back against the large man, but he swiftly drags you towards the stairs and throws your body down the stairs. After you hit the floor at the bottom, another man picks you up and drags you out to the front porch.")
        porch()
    elif sleep_answer == "no" or sleep_answer == "get up" or sleep_answer == "wake up" or sleep_answer == "stop sleeping":
        hall()
    else:
        print("Word not recognized")
        bedroom()

def hall():
    print("You get up and yawn. As you get up your nakedness becomes apparent. You open your closet and put on the pink bath robes. Your stomach gargles but at the same time your bladder feels full.")
    hall_answer = str(raw_input("Do you want to go the bathroom or go downstairs?"))
    print("")
    if hall_answer == "bathroom" or hall_answer == "go to the bathroom" or hall_answer == "pee":
        bathroom()
    elif hall_answer == "downstairs" or hall_answer == "go downstairs" or hall_answer == "stairs":
        downstairs()
    else:
         print("Word not recognized")
         hall()

def bathroom():
    print("As you relieve yourself you look in the mirror. You see the bags underneath your eyes. You aren't quite sure what happened last night, but based on the smell of your breath it probably happened at the bar.")
    bathroom_answer = str(raw_input("Go downstairs?"))
    print("")
    if bathroom_answer == "yes" or bathroom_answer ==  "downstairs" or bathroom_answer ==  "go downstairs":
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
    print("")
    if livingroom_answer == "TV" or livingroom_answer ==  "television" or livingroom_answer ==  "tv" or livingroom_answer ==  "turn off TV" or livingroom_answer ==  "turn TV off":
        television()
    if livingroom_answer == "food" or livingroom_answer ==  "eat" or livingroom_answer ==  "breakfast" or livingroom_answer ==  "kitchen" or livingroom_answer ==  "eat breakfast":
        breakfast()
    else:
        print("Word not recognized")
        downstairs()

def television():
    print("As you walk towards your television you hear the name 'Rupert Mann' spoken. You stop for a moment as that is your name. The newscaster says that Rupert Mann has just become the richest man in Los Angeles.")
    television_answer = str(raw_input("You hear an agressive knocking at the door. Do you ignore the knocking and eat your breakfast?"))
    print("")
    if television_answer == "door" or television_answer == "knocking" or television_answer == "front door" or television_answer == "no" or television_answer == "don't ignore":
        frontdoor()
    if television_answer == "yes" or television_answer == "eat" or television_answer == "breakfast" or television_answer == "kitchen" or television_answer == "eat breakfast" or television_answer == "ignore":
        breakfast()
    else:
        print("Word not recognized")
        television()
       
def breakfast():
    print ("You open your refrigerator. There is a cup of spoiled milk, some sliced ham, a bowl of cheerios, a head of lettuce, and some vegan sausages. You grabthe bowl of cheerios and start eating them.")   
    breakfast_answer = str(raw_input("As you stare blankly at your cheeriosm you hear an agressive knocking at the fromt door. The television is still on."))
    print("")
    if breakfast_answer == "door" or  breakfast_answer == "knocking" or  breakfast_answer == "front door" or  breakfast_answer == "open door":
        frontdoor()
    if breakfast_answer == "TV" or  breakfast_answer == "turn off" or breakfast_answer == "turn off TV" or breakfast_answer == "turn TV off" or breakfast_answer == "television":
        television()
    else:
        print("Word not recognized")
        breakfast()
      
def frontdoor(): 
    print ("As you slowly open your front door, a man grabs the door and slams it open. As you look foreward you see three men. Two of them are wearing biker-esque clothing while the other wears a tuxedo. The two men slam you to the ground.") 
    porch()
        
def porch():
    print ("The man wearing the tuxedo says, 'Mann, you've got 10 hours to get us the 50 million, you'd better have it. After all you're the richest man in Los Angeles.'")
    porch_answer = str(raw_input("Do you tell the thugs that you will get them their money? Yes/No?"))
    print("")
    if porch_answer == "yes" or porch_answer == "y":
        car()
    if porch_answer == "no" or porch_answer == "n":
        die()
    else:
        print("Word not recognized")
        breakfast()
      
def die():
    print ("The man looks you in the eyes. He pulls out a revolver and points the barrel at you. BANG
    
    
    
#start to run the code
bedroom()
