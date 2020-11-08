def turn_right():
    repeat(turn_left,3)
def front():
    if front_is_clear():
        move()
def left():
    while left_is_clear():
        if on_beeper():
                turn_off()
        turn_left()
        move()
        if front_is_clear():
            move()
        if left_is_clear():
            turn_left()
            move()
        if right_is_clear():
            turn_right()
            move()
def right():
    while right_is_clear():
        if on_beeper():
                turn_off()
        turn_right()
        move()
        if front_is_clear():
            move()
        if left_is_clear():
            turn_left()
            move()
        if right_is_clear():
            turn_right()
            move()
left()
right()
front()
left()
turn_left()
left()
front()
front()
front()
right()
turn_off()
