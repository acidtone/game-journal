# [White, Brown, and Pink: The Flavors of Tabletop Game Randomness](https://www.youtube.com/watch?v=qXn3tGBztVc)
by Geoff Engelstein
> "In designing games, a certain degree of uncertainty is essential." - Greg Costikyan, Uncertainty in games (2013)

## Four major areas of uncertainty in games
1. Hidden information
2. Skill/Performance
3. Opponent uncertainty
4. Randomizers

## Randomizers
- Examples:
  - Die roll
  - Card draw
  - Tile flip
  - Spinner
  - Cube tower

Axes of Randomness
- Input/Output
- Correlation

### Input/Output
How are randomizers applied? 
1. Game State
2. Decision
3. Result

There are two main places where randomness can be placed in this paradigm.
1. Input randomness
    - Game State is randomized.
    - Result is fixed (the players know the outcome after the decision is made).
2. Output randomness
    - Result is randomized (the players don't know the outcome of their decision).
    - The Game State is fixed.

#### Output Randomness
- General characteristics:
  - Tactical
  - Feels random
  - Lower skill caps
- Examples:
  - Risk
  - Roulette
  - Dungeons and Dragons
  - Wargames (combat tables)

#### Input Randomness
- It's a more modern phenomenon.
- General characteristics:
  - Strategic
  - High level of control
  - Skillful
- Examples:
  - Dominion
  - Backgammon
  - Contract Bridge
  - Into the Breach

### Correlation
How much does an event tell you about what will happen at the next event?

1. White noise
    - You know nothing.
    - There is zero correlation between the last result and the next result.
    - This is the most common type of randomness in games.
2. Brown noise
    - You know a bit.
    - There is a very high correlation between the last result and the next result.
    - Example: Flip a coin. Heads, add 1. Tails, subtract 1.
    - Also called the random walk.
    - Short for Brownian motion.
3. Pink noise
    - You have a pretty good idea but could be wrong.
    - There is a big chance of a small change, and decreasing chances of larger changes.
    - Humans like Pink Noise.
4. Violet noise
    - Not used in games
    - There is a small chance of a small change and increasing chances of larger changes.

## Game Examples
- Schoko and Co (1987)
    - Supply of cocao and demand for chocolate determined by a card draw.
    - White Noise
    - Feels chaotic and makes it difficult to plan for the future.
- Crude/McMulti (1974)
    - Roll two dice - On doubles, the economy changes to a new state.
    - White/Brown Noise
        - Mechanic similar to Settlers
        - You kind of have an idea of what's happening but the trigger is random.
        - "It makes the economy feel a lot more alive." 
- Crude (2012)
    - Re-release refined this mechanic
    - Roll two dice - Add difference to an accumulator. When >= 8, change economy to a new state.
    - Pink Noise
      - You can have big (1 and 6) and small (2 and 2) changes but you can see it coming.
- Evo (2001)
    - Roll die to move around an environment track.
        - 3, 4, 5, 6: move forward
        - 2: Don't move
        - 1: Move backward
    - Brown Noise
        - This is a classical example
- Tyranno Ex (1990)
    - Face up tokens define environment. When face down exceeds face up, environment change. Possible cascades.
    - Pink Noise.
    - Cascades also apply in Pandemic but not as much of a pink noise as this example.

## Generating Pink Noise
- Not simple to generate exactly
- Constraint from where you are to where you're going
- Example implementations
    - Dice delta: the difference between two dice
    - Exploding dice:
        - 1-3: Miss
        - 4-5: Hit
        - 6: 2 Hits and Re-roll the die!
    - Card distribution
    - Multiple dice
        - More dice means less randomness
    - Extend the extremes
        - Crazy stuff happens if you roll and 2 or a 12 on a 2d6.

## Design Tips
- Consider input vs output randomness. How does it affect planning, strategy, analysis paralysis, etc.
- People like Pink Noise. Try to be between totally random and totally certain.
