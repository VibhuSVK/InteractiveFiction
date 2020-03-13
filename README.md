<iframe height="400px" width="100%" src="https://repl.it/repls/SelfishMinorModes?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>



# InteractiveFiction
#begining also most of the code is defining
def bedroom():
    
    print("Beep Beep Beep. You slam your alarm clock. The clock's display says, 'Fri - 8/6/97 - 5:30'. You have to be at work by seven.")
    sleep_answer = (input("Would you like to sleep in?"))
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
    hall_answer = str(input("Do you want to go the bathroom or go downstairs?"))
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
    bathroom_answer = str(input("Go downstairs?"))
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
    livingroom_answer = str(input("Do you want to turn off the TV, or go eat breakfast?"))
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
    television_answer = str(input("You hear an agressive knocking at the door. Do you ignore the knocking and eat your breakfast?"))
    print("")
    if television_answer == "door" or television_answer == "knocking" or television_answer == "front door" or television_answer == "no" or television_answer == "don't ignore":
        frontdoor()
    if television_answer == "yes" or television_answer == "eat" or television_answer == "breakfast" or television_answer == "kitchen" or television_answer == "eat breakfast" or television_answer == "ignore":
        breakfast()
    else:
        print("Word not recognized")
        television()
       
def breakfast():
    print ("You open your refrigerator. There is a cup of spoiled milk, some sliced ham, a bowl of cheerios, a head of lettuce, and some vegan sausages. You grab the bowl of cheerios and start eating them.")   
    breakfast_answer = str(input("As you stare blankly at your cheeriosm you hear an agressive knocking at the fromt door. The television is still on."))
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
    porch_answer = str(input("Do you tell the thugs that you will get them their money? Yes/No?"))
    print("")
    if porch_answer == "yes" or porch_answer == "y":
        car()
    if porch_answer == "no" or porch_answer == "n":
        die()
    else:
        print("Word not recognized")
        breakfast()

#universal death        
def die():
    print ("The man looks you in the eyes. He pulls out a revolver and points the barrel at you. BANG! You have died.")
    restart_answer = str(input("Would you like to restart?"))
    print("")
    if restart_answer == "yes" or  restart_answer == "restart" or  restart_answer == "y":
      bedroom()
    else:
        print("Word not recognized")
        die()

#first major split
def car():
  print("You run back into your house, and grab your car keys. As you enter the car, you begin to wonder where to go. You could go to the gang's base, the Twinkie Factory, or you could go to the other Rupert Mann's mansion, and ask him to solve this.")
  car_answer = str(input("Where would you like to go?"))
  print("")
  if car_answer == "twinkie" or car_answer == "twinkie factory" or car_answer == "gang" or car_answer == "factory":
    factory()
  if car_answer == "mann" or car_answer == "rupert" or car_answer == "mansion":
    print("You begin to drive yourself to the mansion.")
    mansion()
  else:
      print("Word not recognized")
      car()


def factory():
  print("You drive through the gang's territory, every building seems to have been broken into, as you haven't seen an unbroken window since entering the neighborhood. You pull up to the factory and get out of your car. The same three men from earlier stand there. 'That was fast' one says as he grabs your shirt, 'Wheres the money?')
  factory_answer = str(input("How would you like to respond to the question? Truthfully, or agressively?"))
  if factory_answer == "truth" or factory_answer == "truthfully":
    print("You tell them truthfully that they have the wrong person and that there's another Rupert Mann. The group doesn't believe you. The man in the suit says 'You're down to 8 hours boy, you better get us our money.' He then orders one of his minions to throw your back into your car.")
    money()
  if factory_answer == "agressive" or factory_answer == "agressively":
    print("You tell the three off. You yell about how they have the wrong person, and about how they're the reason the town has gone downhill. The man in the tux signals to one of his men. The man on his left begins to walk closer to you. He stops dead in his tracks.")
    die()
  else: 
    print("Word not recognized")
        factory()


def money():
  print("As you sit in your car you wonder how you're going to get the money to pay the mob. Your first thought is the lottery but that seems like a bad idea. You also have an idea to go to the Mann Mansion and possibly beg for the money.")
  money_answer = str(input("How will you get the money? Will you try the lottery or the mansion?"))
  if money_answer == "lottery"
    print ("You go to the nearest gas station, and run inside. You grab as many sets of the scratch offs that you can. You begin to scratch all of them off. This continues until midnight. As you sit in your car scratching away, you hear a bike pull up to you. You look out your car window and see one of the gangsters.")
    die()
  if money_answer == "mansion" or money_answer == "mann mansion"
    print ("You begin to drive to the mansion")
    mansion()
  else: 
    print("Word not recognized")
    money()


def mansion():
  print("As you pull into the mansion's driveway you notice the extreme defence measures this man has put in. There are all kinds of cameras and motion sensors, as well as three fences that you can't get over. You begin to yell at the house. You yell about how you know that the owner of this mansion is indebted to the mob. After about 20 minutes of yelling, a single man begins to walk out of the front door. He opens each fence one at a time, as he gets closer to you. He walks up to you and hands you a breifcase. 'You came here to collect the debt right? Well here's the money now leave me.' ")
  print("You get back into your car and begin to drive to the twinkie factory.")
  shortcut()

def shortcut():
  print("As you get closer to the heart of the city, you have a choice.")
  shortcut_answer = str(input("Will you take a short cut through the dangerous part of town or will you drive in the more safe business district?"))
  if shortcut_answer == "shortcut" or shortcut_answer == "short" or shortcut_answer == "cut" 
    print("As you start driving through the 'hood' you hit a red light. As you're waiting you see a small boy run fairly close to the left side of your car. The light turns green and your car starts to tilt to the left. You exit the car and see multiple slash marks on both of your left tires.")
    late()
  if shortcut_answer == "safe" or shortcut_answer == "district" or shortcut_answer == "business" or shortcut_answer == "business district" 
    traffic()
  else: 
    print("Word not recognized")
    shortcut()

def traffic():
  print("As you drive throug uptown you hit a traffic jam.")
  traffic_answer = str(input("Would you like to continue in the traffic or ditch the car and walk?"))
  if traffic_answer == "walk" or traffic_answer == "ditch the car"
    late()
  if traffic_answer == "traffic" or traffic_answer == "stay in car" or traffic_answer == "continue"
    biker()
  else: 
    print("Word not recognized")
    traffic()

def biker():
 print("The traffic jam takes too long. As you watch the clock tick away the remainder of your ten hours runs out. The problem is that you're still in the jam. You hear the sound of a bike. A bright light shines off of your rear view mirror. The light grows larger and eventually pulls up next to you. You unroll your window. Its one of the gangsters! He grunts, and you quickly hand him the briefcase. He grabs it, opens it and begins to drive off. (GOOD END) ")
  restart_answer = str(input("Would you like to restart?"))
  print("")
  if restart_answer == "yes" or  restart_answer == "restart" or  restart_answer == "y":
   bedroom()
  else:
      print("Word not recognized")
      biker()

def late():
  print("You look at your car and decide to ditch it. As you walk to the factory it becomes obvious as to how you aren't going to make it in time. Eventually, 3 hours after the deadline, you make it to the factory. As you walk up to the man in the tux you hold out the briefcase. He looks suprised, he snatches the case away and begins to walk off. As he's walking away one of his goons beginst to walk up to you. 'You're late. You broke the deal so you'll face the punishment.' ")
  die()



#start to run the code
bedroom()

