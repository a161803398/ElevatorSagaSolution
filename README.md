# ElevatorSagaSolution
I became fascinated with the Elevator Saga programming game, and decided to share the best solution I developed. It was able to beat all of the levels (though some of the tougher ones required multiple tries). I created wrapper objects for the floors and elevators to add functionality. I also noticed that lodash was provided in the existing project, so I used it as well.

Copy and paste the code in elevator.js into the editor box for the game.

* Main game link: http://play.elevatorsaga.com/
* Last level link (perpetual sim, no goals, fun for experiments): http://play.elevatorsaga.com/#challenge=18

# Algorithm
The basic idea of the algorithm is, once going in a direction, set an elevator's destination to the furthest requested floor in that direction. Then as the elevator passes each floor, check to see if it should stop at that floor. When we go as far in a direction as we have requested stops, reverse direction and repeat. Includes a bit of an optimization to ignore a destination if another closer elevator going in the same direction is already headed to that destination.
