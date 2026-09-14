# DEVLOG for Stack assignment

## September 13th, 2026 at 11:15 pm   
I have been working on getting the general format for how the stack will work down. I did that by figuring out that topIndex should refer to the last variable added to the array. I worked on creating the push, pull, isEmpty, isFull, and the size methods. I decided to make it so that a statement saying "Can't add to a full stack" or "Stack is empty, can't remove from it" when pushing to a full stack or popping from an empty stack respectively. I also wrote this DEVLOG and worked on one of the errors in the error log


## September 14th, 2026 at 1:51 pm
I updated the ERRORLOG with another error I recently got due to accidentally forgetting a colon in the code for printing, and updated the DEVLOG with this . I made the peek function functional and also altered the way the pushing to a full array/stack and the popping from/ peeking into an empty array/stack so that it now explicity states that the value returned is only to indicate the error. Finally, I tested the code by peeking and popping from the empty array/stack, then adding 100 elements and trying to push another one in. All 3 cases correctly displayed error messages.