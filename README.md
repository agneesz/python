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

CODES FROM CLASS DATORIUM

```py
# defining a class Client, which will store all data and methods clients
class Client:
  number_of_clients = 0  

  def __init__(self, id, name):
    self.id = id
    self.name = name
    self.accounts = []
    Client.number_of_clients += 1

  def add_account(self, account):
    self.accounts.append(account)

# defining a class Account, which will store all data and methods of any account
class Account:
  def __init__(self, number, currency):
    self.number = number
    self.currency = currency

# now, let us work using those classes
# adding clients to a list
clients = []
clients.append(Client('123456', 'Anna'))
clients.append(Client('987654', 'Oskar'))
clients.append(Client('456123', 'Jenifer'))

# adding accounts to clients
clients[0].add_account(Account('EE654987564321', 'EUR'))
clients[0].add_account(Account('JP582147859635', 'JPY'))
clients[0].add_account(Account('US654987643214', 'USD'))


# printing some data
print(f'We have {Client.number_of_clients} clients in our bank:')

print(clients[1].name)

for client in clients:
  print(client.name)

```

CORRELATION

The correlation coefficient indicates the strength and direction of the statistical relationship between two variables. The coefficient ranges from -1 to 1, with a value of 0.43 signifying a positive but moderately strong relationship between the two variables.

A positive correlation coefficient means that the variables increase together. Therefore, as one variable increases, the other also tends to increase, and vice versa.
The closer the correlation coefficient is to 1, the stronger the positive relationship.
A correlation coefficient of 0.43 is not very high, but it indicates a moderately positive relationship.
If the correlation coefficient were negative, it would suggest that as one variable increases, the other variable decreases.
A correlation coefficient of -1 indicates a perfect negative relationship.
Thus, a correlation coefficient of 0.43 might suggest that, for example, as Pokémon's Attack values increase, their Defense values tend to increase as well, but the relationship is not very strong.


REGULAR EXPRESSIONS


[I'm an inline-style link]([(https://docs.python.org/3/library/re.html)])

https://docs.python.org/3/library/re.html

[
]([https://docs.python.org/3/library/re.html])



