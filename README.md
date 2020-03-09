# InteractiveFiction

def bedroom():
    print("Beep Beep Beep. You slam your alarm clock. The clock's display says, 'Fri - 8/6/97 - 5:30'. You have to be at work by seven. Sleep in? ")
    sleep_answer = str(raw_input(" "))
    if sleep_answer == "yes" or "sleep in":
        print("")
    if sleep_answer == "no" or "get up" or "wake up":
        print
bedroom()
