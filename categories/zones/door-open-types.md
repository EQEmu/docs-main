# Door Open Types

* 115-152: All need invert\_state to 1 to work correctly. If invert\_state is 0, they don't move but you take damage still if you touch them (Thanks Qadar, for this information):

| **Open Type ID** | **Description**                                                                                       |
| ---------------- | ----------------------------------------------------------------------------------------------------- |
| 0                | normal 90 degree door swing backward                                                                  |
| 1                | normal 90 degree door swing backward                                                                  |
| 2                | normal 90 degree door swing backward                                                                  |
| 3                | normal 90 degree door swing backward                                                                  |
| 4                | normal 90 degree door swing backward                                                                  |
| 5                | normal 90 degree door swing forward                                                                   |
| 6                | normal 90 degree door swing forward                                                                   |
| 7                | normal 90 degree door swing forward                                                                   |
| 8                | normal 90 degree door swing backward                                                                  |
| 9                | nothing                                                                                               |
| 10               | slides forward                                                                                        |
| 11               | slides forward                                                                                        |
| 12               | slides forward                                                                                        |
| 13               | nothing                                                                                               |
| 14               | nothing                                                                                               |
| 15               | slides further forward                                                                                |
| 16               | slides further forward                                                                                |
| 17               | slides further forward                                                                                |
| 18               | nothing                                                                                               |
| 19               | nothing                                                                                               |
| 20               | slides even further forward                                                                           |
| 21               | slides even further forward                                                                           |
| 22               | slides even further forward                                                                           |
| 23               | nothing                                                                                               |
| 24               | nothing                                                                                               |
| 25               | slides furthest forward                                                                               |
| 26               | slides furthest forward                                                                               |
| 27               | slides furthest forward                                                                               |
| 28               | nothing                                                                                               |
| 29               | nothing                                                                                               |
| 30               | rotates 90 degrees clockwise and returns                                                              |
| 31               | nothing                                                                                               |
| 32               | nothing                                                                                               |
| 33               | nothing                                                                                               |
| 34               | nothing                                                                                               |
| 35               | rotates 90 degrees clockwise and returns faster                                                       |
| 36               | rotates 90 degrees and jumps back                                                                     |
| 37               | nothing                                                                                               |
| 38               | nothing                                                                                               |
| 39               | nothing                                                                                               |
| 40               | rotates 90 degrees clockwise and returns slower                                                       |
| 41               | nothing                                                                                               |
| 42               | nothing                                                                                               |
| 43               | nothing                                                                                               |
| 44               | nothing                                                                                               |
| 45               | slide sideways open and closes slowly                                                                 |
| 46               | nothing                                                                                               |
| 47               | nothing                                                                                               |
| 48               | nothing                                                                                               |
| 49               | nothing                                                                                               |
| 50               | no door showing (invisible)                                                                           |
| 51               | nothing                                                                                               |
| 52               | nothing                                                                                               |
| 53               | no door showing (invisible)                                                                           |
| 54               | no door showing (invisible)                                                                           |
| 55               | nothing                                                                                               |
| 56               | nothing                                                                                               |
| 57               | nothing                                                                                               |
| 59               | rocks in a dryer noise -- no movement. \[game notes: spin lift (paineel key)]                         |
| 60               | chain noise/metallic slam -- vertical lift                                                            |
| 61               | chain noise/metallic slam -- vertical lift                                                            |
| 62               | stone noise -- vertical lift                                                                          |
| 63               | no noise -- vertical lift (very high)                                                                 |
| <p></p><p>64</p> | no noise -- vertical lift (very high)                                                                 |
| 65               | chain noise/metallic slam -- vertical lift                                                            |
| 66               | chain noise/metallic slam -- vertical lift                                                            |
| 67               | stone noise/metallic slam -- vertical lift                                                            |
| 68               | no noise -- vertical lift (very high)                                                                 |
| 69               | no noise -- vertical lift (very high)                                                                 |
| 70               | chain noise/metallic slam -- vertical lift                                                            |
| 71               | chain noise/metallic slam -- vertical lift                                                            |
| 72               | stone noise/metallic slam -- vertical lift                                                            |
| 73               | no noise -- vertical lift (very high)                                                                 |
| 74               | no noise -- vertical lift (very high)                                                                 |
| 75               | chain noise/metallic slam -- vertical lift                                                            |
| 76               | chain noise/metallic slam -- vertical lift                                                            |
| 77               | stone noise/metallic slam -- vertical lift                                                            |
| 78               | stone noise -- slide to right (very small amount)                                                     |
| 79               | stone noise -- slide to left (very small amount)                                                      |
| 80               | stone noise -- slide to right (very small amount)                                                     |
| 81               | stone noise -- slide to right (very small amount)                                                     |
| 115              | spins nonstop, 4 points saw damage                                                                    |
| 116              | spins with pause, 4 points saw damage                                                                 |
| 120              | moves down then up, 30 points spear damage                                                            |
| 125              | moves left then right, 30 points spear damage                                                         |
| 130              | swings back and forth, 4 points pendulum damage                                                       |
| 135              | no movement, 4 points blade damage if touched                                                         |
| 140              | moves up then down, 4 points crush damage                                                             |
| 142              | moves up then down nonstop automatically (moves up and down 1 time only if invert\_state is set to 0) |
| 143              | moves up then down nonstop automatically (moves up and down 1 time only if invert\_state is set to 0) |
| 144              | moves up then down nonstop automatically (moves up and down 1 time only if invert\_state is set to 0) |
| 145              | down then up, slow movement, 10 points crushed damage                                                 |
| 146              | down then up, fast movement, 50 points crushed damage                                                 |
| 150              | slide fast left, back slowly, 10 points crushed damage                                                |
| 151              | slide slow left, back slowly, 10 points crushed damage                                                |
| 152              | slide fast left, back quickly, 50 points crushed damage                                               |
