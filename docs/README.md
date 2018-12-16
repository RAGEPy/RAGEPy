# Howdy!

Nice to see you here if you like the programming language Python.  
In this Wiki you should find everything you need to run your RAGE Multiplayer server with Python.

Otherwise you can contact us in Discord (but please only on the server and not via dm).


## Helpful links

### Learn Python:

* [Learn Python](https://www.learnpython.org/)
* [codeacademy](https://www.codecademy.com/learn/learn-python)
* [Official Python website](https://www.python.org/about/gettingstarted/)

* [Python documentation](https://docs.python.org/2.7/)

### RAGEPy quick start:

Its very easy to start with RAGEPy.  
By default, all events are stored in the Events class. This keeps your code clean.

```python
class Events:
```

Let's take the *OnPlayerConnected* event as an example.

```python
class Events:
	def OnPlayerConnected(self, player):
		ragepy.Utils().Log("Hello, " + player.Name, True, 10)
```
**What happens in this case?**  
A green text will be displayed in the console with the player name that has just connected.  
Why green? We will explain to you.  
The parameters of *ragepy.Utils().Log* are:
```python
Log(self: Utils, text: str, printDate: bool, color: int, *args: Array[object])
```
* *self* you can always ignore
* *text* is the message that should be displayed in the console
* *printDate* specifies the current date and time before the actual message is to be output
* *color* defines the color of the text. all colors can be found here:  [Colors](./colors)
* *args* are arguments
