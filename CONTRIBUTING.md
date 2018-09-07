Artists:

- Any items to be integrated into the Source Code >MUST< be in the git repo
- In terms of how to properly use git with art assets ... Jess?


Programmers:

- Rule #1 : don't. f#$! up. master.
  1. Conduct your testing in a different branch (make a new branch for every feature add and test)
    a) MANDATORY
    b) For features, bugfixes, and other permanently useful things
      i)  for example: new branch -> feature_HUD   this would take the latest working code from master 
          so that you can open the project in /SourceCode and add your feature to the game on top of 
          a functional project.
      ii) This is because ideally you get your feature to work and we integrate it back into master 
          for everyone else to use! =D
    c) For learning / fiddling
      i)  for example: new branch -> test_RoomRotation -> mkdir /SourceCode/Elena_Test
          Conduct your testing in a different UE4 project (i.e. in a different folder under SourceCode)
      ii) This is because once you're through with that learning experiment the folder will be deleted
          or possibly the branch will be deleted.
          
- Rule #2 : use readable naming conventions.
  1. For example: 
     a) classes can have names that are "_" separated. (i.e. platform_BP)
     b) variables should be camel case (i.e. platformPlaySpeed)
     c) nothing should EVER be space separated. makes things difficult when you use command line. Plz avoid.
     d) variable names should never. ever. not once ever. contain any variant of "fu" "bar" or combinations of such.
        i) #triggered #notinmyhouse
        
- Rule #3 : if possible, package complicated blueprints into functions.
   1. The hope is to prevent spaghetti blueprints.
