# StarFight- Comp313

Name : Leong Dong ( dongpham ) <br />
Assignment 1 <br />
Title of game : Star Fight <br />

 # Game Description 
 
 1/ What is the main action in the game? <br />
 
 The main action in the game is surviving while you are in a starship trying to survive the enemies as long as possible. The enemies will constantly shooting at you and the longer you survive the higher the score is. You can shoot the enemies for some extra point but remember, the enemies is moving faster and stronger over time. <br />
 
 2/ What was the hardest part of the game to get working in Unreal? <br />
 Unreal is very hard to get started with. For me the hardest part of the game is acctually about the audio of the game. At first, I think mp3 is fine but it turns out I need to use .wav file. Then when I implement a slider in settings so that player can control the sound, it turns out to be very difficult because transferring a a value from a slider to a sound class contain in the map is broken because the slider is remove ( i use removefromparent ) so the change is not saved. Then after that the sound value from the sound class is not changed. All takes me hours to try and fix. Luckily, it turns out I have to use a sound class mix to host a sound class which host the actual sound and then change volumn inside the sound class mix to change the corresponding volume and push the change which fix the previous problem as well ( bc the change gets pushed by getsoundmixmodifier )so it sovle the other problem as well   <br />
 
 3/ What is the most interesting part of the game? <br />
 The most interesting part of the game is actually to design to  balance the game (the speed of the game, feature, power ,... ) to give the user have the best experiences. Because this mini game is intended to  be played when the users having some free time( wait for bus, train, ... ) I don't want to make the game escalated very fast but not slow which will ruin the game. I decide to implement the enemies moving faster quickly but the enemy can also block the bullet from another enemy. This give the user the feeling: " This thing was getting harder real fast, I am so good at the game bc the enemies are so fast but i still make it " while (in reality ) the difficuty is not increasing much because the faster the enemies go, the higer chance they block a bullet from another enemy ( player will hardly notice this bc I make the background distracted so they have to move their the focus to the bullet, not the enemy). Also I want to give the user the feeling " how do I escape that " so I introduce a new feature that the spaceship actually reduce the hitbox when it is in turn animation( i will talk more about this in the video ). This hopefully will give the player some suprised time by saving them.
