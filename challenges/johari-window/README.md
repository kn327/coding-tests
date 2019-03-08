# Navigate Circle

Challenge:
Given a fixed list of adjectives, write a function (using OOP principles) that will model a Johari Window for a given individual. At minimum there should be a class representing an individual's Johari Window, including all of the submissions from other individuals, and a class representing a collection of Johari Windows (the controller) that the application works through. The Window should know how many people voted for each adjective, and should be able to break down what each friend's input was.

<details>
    <summary>What is a Johari Window?</summary>
    <p>
The Johari Window was invented by Joseph Luft and Harrington Ingham in the 1950s as a model for mapping personality awareness. By describing yourself from a fixed list of 56 adjectives, then asking your friends and colleagues to describe you from the same list, a grid of overlap and difference can be built up.
    </p>
    <p>
The grid is made up of four quadrants:
    </p>
    <p>
<b>Open, or Arena</b>
    </p>
    <p>
Adjectives that both the subject and peers select go in this cell (or quadrant) of the grid. These are traits that subject and peers perceive.
    </p>
    <p>
<b>Hidden, or Façade</b>
    </p>
    <p>
Adjectives selected by the subject, but not by any of their peers, go in this quadrant. These are things the peers are either unaware of, or that are untrue but for the subject's claim.
    </p>
    <p>
<b>Blind Spot</b>
    </p>
    <p>
Adjectives not selected by subjects, but only by their peers go here. These represent what others perceive but the subject does not.
    </p>
    <p>
<b>Unknown</b>
    </p>
    <p>
Adjectives that neither subject nor peers selected go here. They represent subject's behaviors or motives that no one participating recognizes—either because they do not apply or because of collective ignorance of these traits.
    </p>
    <img src="https://upload.wikimedia.org/wikipedia/commons/2/2c/Johari_Window.PNG" />
</details>

```
var ADJECTIVES = [
    'able', 'accepting', 'adaptable', 'bold', 'brave',
    'calm', 'caring', 'cheerful', 'clever', 'complex',
    'confident', 'dependable', 'dignified', 'energetic', 'extroverted',
    'friendly', 'giving', 'happy', 'helpful', 'idealistic'
    'independent', 'ingenious', 'intelligent', 'introverted', 'kind'
    'knowledgeable', 'logical', 'loving', 'mature', 'modest'
    'nervous', 'observant', 'organized', 'patient', 'powerful'
    'proud', 'quiet', 'reflective', 'relaxed', 'religious'
    'responsive', 'searching', 'self-assertive', 'self-conscious', 'sensible'
    'sentimental', 'shy', 'silly', 'spontaneous', 'sympathetic',
    'tense', 'trustworthy', 'warm', 'wise', 'witty'
];
```

Input (Joe):<br>
Joe is asking his friends to help contribute to his Johari Window.
```
var windowName = "Joe";
var joesAdjectives = ['accepting', 'calm', 'dependable', 'kind', 'loving', 'intelligent'];

var friend1 = ['bold', 'dependable', 'knowledgeable', 'organized', 'helpful', 'observant'];
var friend2 = ['bold', 'friendly', 'proud', 'silly', 'warm'];
var friend3 = ['able', 'idealistic', 'helpful', 'intelligent', 'knowledgeable', 'happy'];
var friend4 = ['caring', 'accepting', 'intelligent', 'witty', 'modest', 'idealistic'];
```

Expected Output:
```
var johariWindow = {
    name: 'Joe',
    arena: ['accepting', 'dependable', 'intelligent'],

    blindSpot: ['able', 'bold', 'caring', 'friendly', 'happy', 'helpful', 'idealistic','knowledgeable', 'modest', 'observant', 'organized', 'proud', 'silly', 'warm', 'witty'],

    facade: ['calm', 'kind', 'loving'],

    unknown: ['adaptable', 'brave', 'cheerful', 'clever', 'complex', 'confident', 'dignified', 'energetic', 'extroverted', 'giving', 'independent', 'ingenious', 'introverted', 'logical', 'mature', 'nervous', 'patient', 'powerful', 'quiet', 'reflective', 'relaxed', 'religious', 'responsive', 'searching', 'self-assertive', 'self-conscious', 'sensible', 'sentimental', 'shy', 'spontaneous', 'sympathetic', 'tense', 'trustworthy', 'wise'],

    percentages: 'able (25%) accepting (25%) adaptable (0%) bold (50%) brave (0%) calm (0%) caring (25%) cheerful (0%) clever (0%) complex (0%) confident (0%) dependable (25%) dignified (0%) energetic (0%) extroverted (0%) friendly (25%) giving (0%) happy (25%) helpful (50%) idealistic (50%) independent (0%) ingenious (0%) intelligent (50%) introverted (0%) kind (0%) knowledgeable (50%) logical (0%) loving (0%) mature (0%) modest (25%) nervous (0%) observant (25%) organized (25%) patient (0%) powerful (0%) proud (25%) quiet (0%) reflective (0%) relaxed (0%) religious (0%) responsive (0%) searching (0%) self-assertive (0%) self-conscious (0%) sensible (0%) sentimental (0%) shy (0%) silly (25%) spontaneous (0%) sympathetic (0%) tense (0%) trustworthy (0%) warm (25%) wise (0%) witty (25%)',

    breakdown: {
        count: 4,
        people: [
            ['bold', 'dependable', 'knowledgeable', 'organised', 'helpful', 'observant'],
            ['bold', 'friendly', 'proud', 'silly', 'warm'],
            ['able', 'idealistic', 'helpful', 'intelligent', 'knowledgeable', 'happy'],
            ['caring', 'accepting', 'intelligent', 'witty', 'modest', 'idealistic'],
        ]
    }
};
```
