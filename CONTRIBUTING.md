Artists:

- Any items to be integrated into the Source Code >MUST< be in the git repo
- In terms of how to properly use git with art assets ... Jess?


Programmers:

- Rule #1 : don't. f#$! up. master.
  - Conduct your testing in a different branch (make a new branch for every feature add and test)
    - MANDATORY
    - For features, bugfixes, and other permanently useful things
      -  for example: new branch -> feature_HUD   this would take the latest working code from master 
          so that you can open the project in /SourceCode and add your feature to the game on top of 
          a functional project.
      - This is because ideally you get your feature to work and we integrate it back into master 
          for everyone else to use! =D
    - For learning / fiddling
      -  for example: new branch -> test_RoomRotation -> mkdir /SourceCode/Elena_Test
          Conduct your testing in a different UE4 project (i.e. in a different folder under SourceCode)
      - This is because once you're through with that learning experiment the folder will be deleted
          or possibly the branch will be deleted.
          
- Rule #2 : use readable naming conventions.
  - For example: 
     - classes can have names that are "_" separated. (i.e. platform_BP)
     - variables should be camel case (i.e. platformPlaySpeed)
     - nothing should EVER be space separated. makes things difficult when you use command line. Plz avoid.
     - variable names should never. ever. not once ever. contain any variant of "fu" "bar" or combinations of such.
        - #triggered #notinmyhouse
        
- Rule #3 : if possible, package complicated blueprints into functions.
   - The hope is to prevent spaghetti blueprints.
