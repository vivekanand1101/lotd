* ```git bisect``` helps in debugging and finding the culprint commit
* It's like you do binary search between the current commit which you
  know is bad and the other commit which you know is good
* ```git bisect bad``` - mark the current commit as bad
* ```git bisect good <sha>``` - mark this one as good
* After the two steps, git will land you in the middle commit
  between the two and there you test your s/w and accordingly
  mark it good or bad. Once you do this, git will come to know
  which side to search for the bad commit. 
* Finally, there will be no more commits to search and you will 
  you will mark the last commit on which you are as bad.
* To start bisecting: ```git bisect start``` and ```git bisect reset```
  to go back to the original commit 
