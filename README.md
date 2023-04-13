
importimportimportimport time

def display_intro():
    print("Welcome to Adventure Quest!")
    time.sleep(1)
    print("You find yourself in a dark forest with no memory of how you got there.")
    time.sleep(1)
    print("Suddenly, a path appears before you.\n")

def follow_path():
    print("You follow the path and come across a river.")
    time.sleep(1)
    print("You can see a small boat tied up to the shore.\n")
    time.sleep(1)
    choice = input("What would you like to do?\n1. Cross the river in the boat\n2. Try to swim across the river\n3. Explore the area around the river\n\n> ")
    if choice == "1":
        print("You untie the boat and begin to row across the river.")
        time.sleep(1)
        print("Suddenly, a large creature rises from the water and attacks you!")
        time.sleep(1)
        choice = input("What would you like to do?\n1. Fight the creature\n2. Try to flee\n\n> ")
        if choice == "1":
            print("You engage in a fierce battle with the creature, but manage to defeat it.")
            time.sleep(1)
            print("Congratulations, you have completed the first part of Adventure Quest! Stay tuned for more adventures.")
        else:
            print("You try to flee, but the creature catches up to you and attacks you.")
            time.sleep(1)
            print("Game over.")
    elif choice == "2":
        print("You try to swim across the river, but the current is too strong and you get swept away.")
        time.sleep(1)
        print("Game over.")
    elif choice == "3":
        print("You explore the area around the river and find a hidden treasure chest!")
        time.sleep(1)
        print("Congratulations, you have completed the first part of Adventure Quest! Stay tuned for more adventures.")
    else:
        print("Invalid choice.")
        follow_path()

def main():
    display_intro()
    follow_path()

if __name__ == "__main__":
    main()

