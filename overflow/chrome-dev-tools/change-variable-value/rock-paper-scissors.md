- author: Lev
- language: JavaScript
- topics: Chrome DevTools
- difficulty: 2.5
- format: Project

### Question

Anaximander would like to play a game of rock-paper-scissors, but the computer always seems to win. Help Anaximander win a game, or at least get a tie! Use Chrome DevTools and do not change any JavaScript or HTML code. Hint: there is a .js file located under the `Sources` tab, inside the `assets` folder. Use breakpoints. 


### Answer

The function getRandomChoice() checks the user's choice (since userChoiceString is a global variable) and is not really random. In order to get the player to win, the value of either userChoiceString or computerChoiceString need to be modified at runtime. This can be done at different points after getting the value for computerChoiceString from the getRandomChoice function.
