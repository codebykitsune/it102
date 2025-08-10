# this is pseudocodes about Rock Paper Scissors Game.

Begin
1. Make variables:Rock Paper Scissors
   - "choices" = ["Rock", "Paper", "Scissors"]
   - "yourChoice" = User's input (Rock Paper Scissors)
   - "npcChoice" = Randomly selected choice from choices
   - "result" = output of the game
   
2. Rules:
    - Rock is stronger than Scissors
    - Scissors is stronger than Paper
    - Paper is stronger than Rock
  
3. Ask the user to select one:Rock Paper Scissors. - save the user's choice in a variable: "Yourchoice"

4. Use a random method to decides one choice for computer. - save the computer's choice in a variable: "npcChoice"
   
5. Check if the user lose, draw, or win.And store your result into a variable "result"
   - if "yourChoice" == Rock and "npcChoice" == Scissors, then "result" == "win"
   - else if "yourChoice" == Scissors and "npcChoice" == Paper, then "result" == "win"
   - else if "yourChoice" == Paper and "npcChoice" == Rock, then "result" == "win"
   - else if "yourChoice" == NPC choice, then "result" == "draw"
   - else, "result" == "lose"

6. show your result
   -show "yourchoice", "npcChoice" and "result"

End