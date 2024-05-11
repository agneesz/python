# python

```python
while True: #city != "stop"
  city = input('What cities have you been to in LV or EE? T stop write "stop".')

  if city == 'stop': 
    print('You have written "stop".') #run the code until user has written STOP
    break
  else:
    print(f'I se you have to been to the {city}.')

```


```python

x = []
counter = 0
while True: #city != "stop"
  city = input('What cities have you been to in LV or EE? T stop write "stop".')
  
  if city == 'stop': 
    print('You have written "stop".') #run the code until user has written STOP
    break
  else:
    counter = counter + 1
    print(f' {counter}. I se you have to been to the {city}.')
    x.append(city)

print(f'You have been to {len(x)} cities')


```
```python
import random
random_number = random.randint(0, 101) 

lis = []
counter = 0 
while True:
  guess = input('Guess the number between 1 and 100, sto quite write "stop"!')

  if guess == 'stop':
    print('The game has been stopped.')
    break
  try: 
    guess = int(guess)
  except:
    print("you need to input integer")
    continue
  #EXCEPT
  counter = counter + 1
  lis.append(guess)

  if guess == random_number:
    print('Congratulations. You have guessed the correct number.')
    break
  else:
    if guess > random_number:
      print('try lower!')
    else:
      print('try higher!')

print(f' You have ben trying {len(lis)} times')
print(f"You guessed {counter} times before finding the right number. ")

```


```python
import random

def coin_toss_game():
    print("Welcome to the Coin Toss Game!")
    print(" ")
    print(" ")
    correct_guesses = 0
    total_guesses = 0
  
    while True:
      answer = input("Enter your guess (heads or tails), or 'quit' to exit: ")
      total_guesses += 1
      if answer == 'quit':
        break

      if answer != 'heads' and answer != 'tails':
        print("Invalid input. Please enter 'heads', 'tails', or 'quit'.")
        print(" ")
        continue
      random_number = random.randint(0,1)
      if random_number == 0:
        result = 'heads' 
      else:
        result = 'tales'


      if answer == result:
          print("Congratulations! You guessed correctly!")
          correct_guesses += 1
      else:
          print("Sorry! You guessed incorrectly.")
      
      
      print(f' You have ben trying {total_guesses} times')
      print("Correct guesses:", correct_guesses)
      print(" ")
      print(" ")

coin_toss_game()
```
