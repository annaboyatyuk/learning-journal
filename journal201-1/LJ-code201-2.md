Learning Journal 1/15 begining of week 2!

loops were really hard to understand. when I did the Code 102 course, we learned loops but only with functions so I just wasn't understanding how to connect loops and arrays and pull from the arrays and question 6 on the lab, how to make the user guess a number a certain amount of times so Im just gonna paste my code in here so that I dont forget it


var answer6 = 3;
var notDone = true;
var guess;

for (var guesses = 4; guesses > 0 && notDone; guesses--) {
  guess = prompt('How many siblings does anna have'); // get user input
  guess = parseInt(guess); // convert user input to number
  if (guess < 3) { //if the user guesses too low
    alert('Try again, theres more than that!');
    console.log('the user guessed too low ' , guess);
  }
  if (guess > 3) { //if the user guesses too high
    alert('Not quite that many, try again!');
    console.log('the user guessed too high ' , guess);
  }
  if (guess === answer6) { //if the user gets the right answer
    alert('you got it!');
    notDone = false;
    userPoints++;
    console.log('the user got the right answer to question 6 ' , guess);
  } else if (guesses === 1) { //this had to be the last statement so that this is the last alert
    alert ('you are out of guesses');
  }
}

questionNumber++;
console.log('the user answered question 6' , guess);


alert('I have 3 sisters!');


that was question 6 and this ones question 7




var answer7 = ['iceland' , 'london' , 'loch ness' , 'lake hillier' , 'equador'];
var guessAgain = true;
var tries = 0;

while (guessAgain && tries < 7) {
  var question7 = prompt('Can you guess one of the top five places that Anna wants to visit?').toLowerCase();
  console.log('question7' + question7);

  for (var x = 0; x < answer7.length; x++)
    if (answer7[x] === question7.toLowerCase()) {
      alert('You got it! I want to go to ' + question7);
      guessAgain = false;
      tries++;
      userPoints++;
      console.log('the user got one of the answers to question 7 correct' + question7);
      break;
    }
  if (answer7[x] !== question7.toLowerCase()) {
    alert('I would probably like to go there but its not my top 5!');
    tries++;
    console.log('the user got the wrong answer to question 7 ' , question7);
  }
}
alert('The top 5 places I want to visit are: ' + answer7);

questionNumber++;
console.log('the user answered question 7 ' , question7);






for(starting value; condition; increment) {
    DO SOMETHING FOR A     FINITE    NUMBER OF TIME
}

    example
    for(var i = 0; i < 100; i++) {
        console.log("i is now" , i);
    }
this is so that i dont have to write the same code over and over




while(true) {
    DO SOMETHING UNTIL THE CONDITION IS FALSE
}

    example
    var n = 0;
    
    while(n < 3) {
        n++;
    }

    console.log(n);
    //expeced output: 3
    while loops are really useful especially for arrays
