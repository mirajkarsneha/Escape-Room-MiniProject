# Escape Room 🧩🔒🗝️🧠🏃‍♂️🚪💡

## 📒 Description 
Welcome to Escape Room game, the goal of this game is to escape from the starting room (Game Room) to the end (Outside).

## 💡 Prerequisites 
- Jupiter
- Python

## 🧠 Game Narrative 
- Suddenly, you find yourself waking up on an unfamiliar couch, in an eerie house devoid of windows. Your memory fails to provide any explanation about how you ended up here, or what transpired previously. You can sense an imminent threat lurking somewhere - your gut tells you to escape the house immediately!

- You look around and realize you’re in a game room.

- “What should I do?” you ponder.

- You decide to explore the room, which uncovers a couch, a piano, and a locked Door A. The couch appears mundane and unexciting. However, examining the piano rewards you with a key for Door A. With the newfound key, you manage to unlock Door A.

- Will you step into the unknown through Door A?

#### 🚪🗝️ Bedroom 1 
- You step into Bedroom 1.

- Again, you find yourself contemplating - to explore or examine?

- Your exploration reveals a queen bed, Doors A, B, and C. Underneath the queen bed, you find a key for Door B. Door C remains an impenetrable barrier as it’s locked and you lack the key. But with the key you found under the bed, you manage to unlock Door B.

- Is it time to venture through Door B?

#### 🚪🗝️ Bedroom 2
- Your journey leads you to Bedroom 2.

- “What now?” you think.

- A thorough exploration uncovers a double bed, a dresser, and Door B. Hidden in the double bed, you discover a key for Door C, and within the dresser, a key for Door D awaits. Equipped with the key for Door B, you decide to unlock it.

- Shall you retrace your steps through Door B?

#### 🚪🗝️ Bedroom 1
- Once again, you find yourself in Bedroom 1.
 
- “What’s the next move?” you wonder.

- With the key for Door C in your possession, you manage to unlock it.

- Are you ready to brave the unknown behind Door C?

#### 🚪🗝️ Living Room
- Stepping through Door C, you find yourself in the living room.

- “What secrets does this room hold?” you muse.

- Exploration reveals a dining table, Door C, and Door D. With the key for Door D in your grasp, you unlock it.

- Is it time to step through Door D and see what lies beyond?

#### 🎉 Outside 
- Freedom! You’ve managed to escape the room! Congrats on your successful adventure! Now, can you recount the thrilling journey and the clever strategy that got you here?

## 🏃‍♂️ How to run the game 
- Run the main.ipyb file to start the game.

## 🏃‍♂️ What happens next at the backend
- When the game starts function start_game() is called.
- start_game() function calls play_room(room) function
- play_room(room) function, first checks if the room being played is the target room. If it is, the game will end with success. Otherwise, let player eitherexplore (list all items in this room) or examine an item found here.
- Next explore_room(room) function is executed. This function explore a room and list all items belonging to this room.
- get_next_room_of_door(door, current_room) function is executed. This function finds the two rooms connected to the given door from object_relations and return the room that is not the current_room.
- examine_item(item_name) this function examine an item which can be a door or furniture. First make sure the intended item belongs to the current room. Then check if the item is a door. Tell player if key hasn't been collected yet. Otherwise ask player if they want to go to the next room. If the item is not a door, then check if it contains keys. Collect the key if found and update the game state. At the end, play either the current or the next room depending on the game state to keep playing.
