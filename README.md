import random

number_generated = random.randint(0, 9)


print (' >>>>>>  you have three attepts only in this game. Guess well <<<<<<< ')

# first guess

guess = int(input('Guess the first number from 0 to 9:: '))

if number_generated == guess:
    print( 'Great, you won.')
    exit()
else:
    if number_generated > guess:
        print('the correct numer is higher. ')
    else:
        print( 'the correct numer is lower.')

# second guess
second_guess = int(input('Guess the second number from 0 to 9:: '))

if number_generated == second_guess:
    print( 'Great, You won')
    exit()
else:
    if number_generated > second_guess:
        print('the correct numer is higher. ')
    else:
        print( 'the correct numer is lower.')

# last guess

last_guess = int(input('Guess the last number from 0 to 9:: '))

if number_generated == last_guess:
    print( 'Great, you won')
    exit()
else:
    print( 'You lost the game. Better Luck next time. ')

