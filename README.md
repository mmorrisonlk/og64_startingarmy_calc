# og64_startingarmy_calc
    What is the point of this? Ogre Battle 64 for (shock) the Nintendo 64 is a unique tacital strategy RPG. Relevant to our purposes is that your starting army is determined by how you answer a series of questions. This information was shoddy, had some errors and unfortunately took a non trivial amount of time to verify that your inputs had resulted in the players desired set up.

    Let's first start by defining the problem. How is your starting army determined? There are 6 questions. Each of the answers to these questions have a value corresponding to each of the 4 army categories: Warrior, Magic, Healer and Trainer. For example, answering "Ardor" to the first question adds 12 value to "Warrior", 16 to "Magic", 4 to "Healer" and 8 to "Trainer". It is possible for an answer to increase a category by 0. The first option just doesn't have that option.

    Once you have answered the 6 questions the game sums the values in each category. Then it looks for the highest value. And the unit at the first position for that category is chosen as the 1st of 4 slots. Then the total that was used is subtracted by 32 and the calculation is done again until all 4 slots are filled. Ties are broken in the following priority Warrior > Magic > Healer > Trainer. 
    
    Someone has already gone through most of the trouble of figuring this out and even coding a calculator. But I think it might be done differently and for my own practice.