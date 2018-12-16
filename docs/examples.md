# Examples
## Example 1
This example displays the player name in the console in the color green. The current time and date are also displayed.
After that the player will be kicked.
```python
class Events:
	def OnPlayerConnected(self, player):
		ragepy.Utils().Log("Hello, " + player.Name, True, 10)
		ragepy.Kick(player, "Bye!")
```

