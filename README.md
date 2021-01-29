# codec-project-4-day-race-day
//a program that will register runners for the race and give them instructions on race day. 
Start time:
/* -Adult registrants run at 9:30 am or 11:00 am.
-Early adults run at 9:30 am.
-Late adults run at 11:00 am.
-Youth registrants run at 12:30 pm (regardless of registration).
...But we didn’t plan for runners that are exactly 18!...  codecademy proj conditionals section*/


let raceNumber = Math.floor(Math.random() * 1000);

let early = true; 
let age = 19;

if(early && age > 18){
raceNumber += 1000;
}
if(early && age > 18){
    console.log(`The race will begin at 9:30. Your race is ${raceNumber}.`);
}
else if (!early && age > 18) { 
  console.log(`Race will begin at 11:00, your race number is: ${raceNumber}.`);
}
else if (age < 18) {
  console.log(`Race will begin at 12:30, your race number is: ${raceNumber}.`);
} else  {
console.log('Go to the registration desk, thanks!');
}
