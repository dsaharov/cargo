2D

The cursor starts at position (0,0), with 2 fuel and 0 cargo.

If it runs out of fuel, the program terminates.

Every frame we subtract 1 fuel, run the operation at our current position, and move the cursor "forwards."

Positive x is right, positive y is down.

If the cursor leaves the grid, it wraps around along its current direction.


The operators

| Operator | Action |
|---|---|
| ^ | set forwards to up |
| \> | set forwards to right |
| v | set forwards to down |
| < | set forwards to left |
| + | add 1 cargo  |
| \- | subtract 1 cargo (if above 0)  |
| L,J,F,7 | Curve sections. If we have cargo, follow the curve. (e.g. going into L from the right sends you up)  |
| / | Ramp. If we don't have cargo, jump over the next position.  |
| 1-9 (except 7) |  Add this much fuel  |
| f |  print the amount of fuel  |
| l | print the character at the code point of the amount of fuel remaining  |
| c | print the amount of cargo  |
| o | print the character with the code point of the amount of cargo remaining  |
| i | Set the amount of fuel to an inputted value  |
| I | Set the amount of cargo to an inputted value  |
| . | No-op |
