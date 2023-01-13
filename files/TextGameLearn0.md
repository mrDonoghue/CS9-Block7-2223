```python
import replit


def beach():
  # replit.clear()
  while True:
    print("You're on a sandy beach")
    print(
      "You see an X on the ground.\nYou\n suspect there is buried treasure")
    print("In the water, you see a partially submerged shipwreck")
    print("Say 'shipwreck', or 'x'")
    ans = input()
    if ans == "shipwreck":
      shipwreck()
    elif ans == "x":
      print("You try to dig with your hands, but you give up soon")
    else:
      print("I didn't understand that.")
      print("Try again. This time, read better.")
      print()


def shipwreck():
  replit.clear()
  while True:
    print("You're on a shipwreck")
    print("You see the beach in the distance.")
    if not has_shovel:
      print("There is a shovel lying on the deck")
      print("Mysterious...")
      print("Say 'beach' or 'shovel'")
    else:
      print("Say 'beach'")
    ans = input()
    if ans == "beach":
      beach()
    elif ans == "shovel":
      has_shovel = True
    else:
      print("That's not an option. STOP TRYING TO CHEAT")


has_shovel = False
beach()
```