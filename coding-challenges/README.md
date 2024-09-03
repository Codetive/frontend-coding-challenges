*Work in progress*

*Those are example questions which will be available both here written and as interactive challenges on Codetive website.*

> *It's free feature btw :-)*

## Example question 1:

### Interview Question
**Objective**: Implement a React component that fetches and displays data from the Pokémon API.

**Instructions**:

1. Create a functional React component named PokemonFetcher.

2. The component should fetch data from the Pokémon API (https://pokeapi.co/api/v2/pokemon/ditto) and display the Pokémon's name and an image of the Pokémon.

3. Display the Pokémon’s name in an `<h1>` tag.

4. Show an image of the Pokémon using the `<img>` tag. Use the sprites.front_default field from the API response for the image URL.

**Hints...**

1. Use the useEffect hook to fetch data from the Pokémon API when the component mounts.
2. Use the useState hook to manage the loading state, fetched data, and any potential error.

**Bonus:**
Handle loading and error states with appropriate messages or indicators.
Bonus:

Add basic styling to make the component visually appealing.



## Example Question 2:
### Interview Question
**Objective**: Implement a debounce function in JavaScript.

**Instructions**:

1. Implement a function named debounce that takes two arguments:
    - A function func to be debounced.
    - A delay time in milliseconds wait.

2. Function Behavior:

The debounce function should return a new function that, when invoked, will delay the execution of func until after wait milliseconds have elapsed since the last time the returned function was invoked.

3. Function Execution:

If the returned function is invoked again within the wait milliseconds, the previous call should be canceled and a new timer should start.
Ensure that func is executed only after the wait time has passed since the last invocation.

**Hints...**

Use setTimeout to create a delay before executing func.
Use clearTimeout to cancel the previous timeout if the function is invoked again before the delay has passed.