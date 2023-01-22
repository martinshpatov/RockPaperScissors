# "Rock-Paper-Scissors" Game


function rockPaperScissors(playerTurn) {
const rock = "rock";
const paper = "paper";
const scissors = "scissors";

if (playerTurn == "r" || playerTurn == "rock") {
    playerTurn = rock;
} else if (playerTurn = "p" || playerTurn == "paper") {
    playerTurn = paper;
} else if (playerTurn == "s" || playerTurn == "scissors") {
    playerTurn = scissors;
} else {
    console.log("Invalid Input. Try Again...");
}

let computerRandomNumber = Math.floor(Math.random() * 3) + 1;

switch (computerRandomNumber) {
    case 1:
        computerMove = rock;
        break;
    case 2:
        computerMove = paper;
        break;
    case 3:
        computerMove = scissors;
        break;
}
console.log(`You choose ${playerTurn}`)
console.log(`The computer chooses ${computerMove}`);

if(playerTurn == rock && computerMove == scissors || playerTurn == paper && computerMove == rock || playerTurn == scissors && computerMove == paper) {
    console.log("You win!")
} else if(playerTurn == scissors && computerMove == rock || playerTurn == rock && computerMove == paper || playerTurn == paper && computerMove == scissors) {
console.log("You lose!")
} else {
    console.log("DraW")
}
}
