# Food Preferences

Challenge:
The goal of this is to find out what all possible options for someone to eat are on a menu based off of some preferences.

    * lunchMenuPairs represents the type of food along with the food
        > [ "Curry", "Indian" ]
    * teamCuisinePreference represents the name of the team member along with their preference
        > [ "John", "Indian" ]
        > If the preference is "*", then all types of food apply

Create an algorithm to return all possible combinations of person to food choice. It is possible that there are no valid possibilities, at which point, return an empty array.

```
var lunchMenuPairs = [
    ["Curry", "Indian"],
    ["Noodles", "Japanese"]
];

var teamCuisinePreference = [
    ["John", "Indian"],
    ["Tim", "*"]
];


var output = [
    ["John", ["Curry"]],
    ["Tim", ["Curry", "Noodles"]]
];
```