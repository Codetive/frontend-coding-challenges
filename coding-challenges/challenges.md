*Each of the challenge you can do interactively on the Codetive app (launching late September 2024). Order of the questions might differ*

---

Let's start with 2 short and quick warmup questions, so you can get familiar with the question template.

## 1. Sum of Two Numbers (warmup)

**Objective**: Write a function that takes two numbers as input and returns their sum.

**Instructions**:

1. Write a function named `sum` that accepts two arguments (both numbers).
2. The function should return the sum of the two input numbers.

**Expected Output**:

```js
sum(5, 3); // Output: 8
sum(10, -2); // Output: 8
```

**Requirements**:

- Function should return the sum of the two input numbers
- Function works correctly with both positive and negative numbers
- Function handles invalid inputs


## 2. Counter (warmup)

*Beginner | Javascript/Typescript/React*

**Objective**: Build a functional counter using HTML, CSS, and JS/TS/React.

**Instructions**:

1. Create a simple counter with the following elements:
   - A display showing the current count.
   - Two buttons: one for incrementing the count and another for decrementing it.

2. The counter should start at `0` by default.

3. Clicking the "Increment" button should add `1` to the current count.

4. Clicking the "Decrement" button should subtract `1` from the current count.

**Requirements**:

- The counter must always start at `0` when the page loads.
- The counter cannot go below `0` (disable the "Decrement" button or handle the logic to prevent negative counts).
- The count must persist correctly between increments and decrements without refreshing the page.

**Hints**:

1. Store the current count in a variable and update it when the buttons are clicked.
2. Update the displayed count by modifying the inner text of an HTML element (like a `<span>` or `<h1>`).
3. You can disable the "Decrement" button when the count is at `0` to prevent negative values.

**Bonus:**
- Add a reset button that sets the counter back to `0`.
- Style the buttons and counter display

## 3. Infinite Scroll

*Beginner | Javascript/Typescript/React*

**Objective**: Implement an infinite scroll feature using JS/TS/React.

**Instructions**:

1. Create a web page with a list of items that loads more items when the user scrolls to the bottom of the page.
2. The list should initially display `10` items.
3. When the user scrolls to the bottom, dynamically load the next `10` items and append them to the existing list.
4. Use an API or a mocked list of data to populate the items.

**Requirements**:

- Items must load dynamically without a full page reload.
- The infinite scroll should work smoothly regardless of the data size.

**Hints**:

1. Use JavaScript's `scroll` event to detect when the user reaches the bottom of the page.
2. Ensure that the new items are appended to the list smoothly without overwriting the current items.
3. Optionally, add a loading spinner to indicate that more data is being loaded.

**Bonus:**
- Add a "Load More" button as an alternative for users who don't want automatic loading.
- Handle errors, showing a message if items can't be loaded.

## 4. Pokémon Fetcher

*Beginner | React*

**Objective**: Fetch and display Pokémon data using React.

**Instructions**:

1. Create a React component named `PokemonFetcher`.

2. The component should fetch data from the **Pokémon API**: `https://pokeapi.co/api/v2/pokemon/ditto`.

3. Display the Pokémon’s name inside an `<h1>` tag.

4. Display an image of the Pokémon using the `<img>` tag. Use the `sprites.front_default` field from the API response for the image URL.

**Requirements**:

- Use the `useEffect` hook to fetch data from the API when the component mounts.
- Use the `useState` hook to manage the following states:
   - Fetched Pokémon data.
   - Loading status (optional)
   - Error handling for failed API calls (optional)

**Hints**:

1. Use `fetch` to retrieve the Pokémon data.
2. Handle different states:
   - Loading (while waiting for the data).
   - Success (once the data is fetched).
   - Error (if something goes wrong).

**Bonus**:

- Display a loading message or spinner while the data is being fetched.
- Style the component to make it look good.

## 5. Skeleton Loader for Content

*Beginner | Javascript/Typescript/React*

**Objective**: Implement a skeleton loader for content while waiting for an API response.

**Instructions**:

1. Create a functional React component named `ContentWithSkeleton`.

2. The component should fetch data from any public API of your choice (or use `https://jsonplaceholder.typicode.com/posts/1` as a default).

3. Display a skeleton loader while the data is being fetched. Once the data is fetched, replace the skeleton with the actual content (e.g., a title and body).

4. Ensure that the skeleton loader is styled to look like the content it will replace (e.g., rectangles for text blocks).

**Requirements**:

- Use the `useEffect` hook to fetch data when the component mounts.
- Use the `useState` hook to manage loading, error, and success states.
- Replace the skeleton with real data when the API call is successful.

**Hints**:

1. Style the skeleton loader using CSS to simulate the structure of the final content (e.g., gray boxes representing text).
2. Handle different states:
   - Loading (display skeleton).
   - Success (display actual content).
   - Error (display an error message if the API call fails).

**Bonus**:

- Add animations to the skeleton loader to simulate loading (e.g., shimmer effect).
- Ensure the skeleton loader is responsive and works on different screen sizes.

## 5. Skeleton Loader for Content

*Beginner | Javascript/Typescript/React*

**Objective**: Implement a skeleton loader for content while waiting for an API response.

Example how it looks: [Link ->](https://ui.shadcn.com/docs/components/skeleton)

**Instructions**:

1. Create a component named `ContentWithSkeleton` (or if you are not using React just create an HTML element).

2. The component should fetch data from any public API of your choice (or use `https://jsonplaceholder.typicode.com/posts/1` as a default).

3. Display a skeleton loader while the data is being fetched. Once the data is fetched, replace the skeleton with the actual content.

4. Ensure that the skeleton loader is styled to resemble the structure of the content it will replace (e.g., rectangles for text blocks).

**Requirements**:

- Fetch data when the component or page loads.
- Manage loading, error, and success states to ensure the skeleton is replaced by actual content once the data is retrieved.

**Hints**:

1. Use CSS to style the skeleton loader to simulate the final content structure (e.g., gray boxes representing text or images).
2. Handle different states:
   - Loading (display skeleton).
   - Success (display actual content).
   - Error (display an error message if the API call fails).

**Bonus**:

- Add animations to the skeleton loader, such as a `shimmer effect`, to simulate loading.
- Handle errors, showing an error message if the API call fails or changing skeleton style

## 6. Flatten Array

*Beginner | Javascript/Typescript*


**Objective**: Write a function that takes a nested array and returns a flat array with all elements at the same level.

**Instructions**:

1. Create a function called `flattenArray` that accepts an array containing nested arrays of various depths.
2. The function should return a new array where all the elements are "flattened" to the top level (i.e., no nested arrays).

**Example**:

```js
flattenArray([1, [2, 3], [4, [5, 6]]]); 
// Output: [1, 2, 3, 4, 5, 6]
```
**Requirements**:

- The function must handle arrays with multiple levels of nesting.
- You cannot use the built-in `Array.prototype.flat()` method.
- The function should work recursively to ensure that deeply nested arrays are also flattened.

**Hints**:

1. Use `recursion` to handle arrays nested at multiple levels.
2. `Concatenation` or `spreading` can help combine arrays when flattenin

**Bonus**:

- Add a second argument to the function that limits how deep it should flatten the array (like `Array.prototype.flat(depth)`).

## 7. Draggable and Droppable Elements

*Beginner | Javascript/Typescript/React*

**Objective**: Implement a UI where users can drag and drop boxes into a container.

**Instructions**:

1. Create a draggable UI with a set of boxes placed outside a container.
2. The container should have a 2x2 grid layout.
3. Users should be able to drag and drop the boxes into the container.

**Requirements**:

- The boxes should be draggable.
- The container should accept boxes dropped into it and maintain a grid layout (2x2).
- Make sure the drag-and-drop functionality is intuitive and works smoothly.

**Hints**:

1. Use `dragstart`, `dragover`, and `drop` events in JavaScript to handle the drag-and-drop functionality.
2. Ensure that the container keeps its 2x2 layout when the boxes are dropped into it.

**Bonus**:

- Implement a "snap to grid" feature, where the boxes automatically align to the nearest corner of the container when dropped.
- Make the boxes repositionable after being dropped into the container.
- Add info when a box is being dragged over the container (e.g., a highlight effect).

## 8. Mini CSS Library

*Intermediate | Javascript/Typescript/React*

**Objective**: Create a utility function that helps manage and generate CSS class names dynamically based on conditions.

**Instructions**:

1. Write a function called `customCSS` that accepts an object as its argument. The object will have CSS class names as keys and conditions (boolean values) as their corresponding values.

2. The function should return a string of class names where the condition is true.

3. You should be able to pass multiple class names into the function, and it should only include those that meet the conditions.

**Example**:

```js
miniCSS({
  'btn-primary': true,
  'btn-disabled': isDisabled,
  'hidden': !isVisible
});
// Output: 'btn-primary' (if `isDisabled` is false and `isVisible` is true)
```

**Requirements**:

- Accept an object with class names as keys and boolean conditions as values.
- Return a string of class names that satisfy the true condition.
- Ignore any classes where the value is false.

**Bonus:**

1. Add support for combining static class names with dynamic ones.
2. Allow function to accept more complex conditions, example:
   
```js
miniCSS({
  'btn-primary': true,
  'btn-disabled': isDisabled,
  'hidden': !isVisible,
  'md:text-lg': windowWidth > 768, // Responsive condition
});
```

## 9. Notification Bell

*Intermediate | Javascript/Typescript/React*

**Objective**: Implement a notification bell component that shows an unread notification count and displays a list of notifications on click.

**Instructions**:

1. Create a notification bell icon that displays the number of unread notifications.
2. Clicking the bell should open a list of notifications.
3. Include two buttons for different types of notifications (e.g., "Messages" and "Alerts"). Clicking these buttons should *simulate* adding new notifications of the respective type.
4. Add a button to clear all notifications under the list of notifications.

**Requirements**:

- The notification bell should display an unread count.
- Clicking the bell should show a list of notifications.
- The "Messages" and "Alerts" buttons should simulate adding a new notification of the corresponding type.
- Add a "Clear All" button to remove all notifications.

**Hints**:

1. You can style the notification list as a dropdown or a modal that opens when the bell is clicked.
2. Use conditional rendering to toggle between showing and hiding the notification list.

**Bonus**:

- Add animations or transitions when the notification list opens or closes.
- Allow users to remove individual notifications from the list.
- Add visual difference between notification types.

## 10. Custom Hook / Window Dimensions

*Beginner | React*

**Objective**: Implement a custom React hook that returns the current window dimensions (width and height).

**Instructions**:

1. Create a custom hook named `useWindowDimensions`.
2. The hook should return an object containing the current width and height of the browser window.
3. The hook should update the dimensions in real-time when the window is resized.

**Example Usage**:

```js
const { width, height } = useWindowDimensions();
console.log(`Width: ${width}, Height: ${height}`);
```

**Requirements**:

- The custom hook should listen for the resize event on the window and update the width and height values accordingly.
- The hook returns the correct dimensions when the component mounts.

**Hints**:

1. Use `useState` to store the width and height values.
2. Use `useEffect` to handle the window resize event and update the dimensions in real-time.
3. Remember to remove the event listener when the component unmounts to avoid memory leaks.

## 11. Progress Bar with Dynamic Updates

*Beginner | Javascript/Typescript/React*

**Objective**: Implement a progress bar that updates dynamically based on the input.

**Instructions**:

1. Create a progress bar component that visually represents progress as a percentage.
2. Allow the progress value to update dynamically based on input.
3. The progress bar smoothly transitions as the value changes.

**Example Usage**:

- A button to increment progress by 10%.
- Number input to update the progress value.

**Requirements**:

- The progress bar should display the current percentage of completion.
- The progress bar should visually fill from 0% to 100% based on the progress value.

**Bonus**:

- Add a label inside the progress bar to display the current percentage.
- Make the progress bar color change as it progresses (e.g., green for 0-50%, yellow for 51-80%, and red for 81-100%).

## 12. Debounce Input

*Beginner | Javascript/Typescript*

**Objective**: Implement an input field with a debounced event handler to optimize performance.

**Instructions**:

1. Create an input field where user input is handled after a specified delay (debounced) to prevent unnecessary function calls (e.g., when searching or filtering data).
2. The event handler should only trigger after the user has stopped typing for a certain period (e.g., 500 milliseconds).
3. The input value should be displayed or logged *after* the debounce delay.

**Requirements**:

- Implement a debounce mechanism to delay the input handling.
- The input value should only update **once** the debounce delay has passed without additional input.

**Hints**:

1. You can use `setTimeout` and `clearTimeout` to manage the debounce logic.

## 13. Tooltip

*Beginner | Javascript/Typescript/React*

**Objective**: Implement a tooltip component that appears when hovering over an element and allows positioning control.

**Instructions**:

1. Create a tooltip that appears when the user hovers over an element.

**Requirements**:

- The tooltip should appear on hover and disappear when the hover ends.
- Allow customization of the tooltip's position (top, bottom, left, or right).
- Implement a customizable delay before the tooltip shows and hides.

**Hints**:

1. Use CSS for the positioning of the tooltip and for handling the hover effect.
2. You can use JavaScript to manage the delay and control when the tooltip appears or disappears.
3. Ensure that the tooltip remains visible while the user hovers over it.
4. With React you can experiment with `portals`.

## 14. Promise.all Polyfill

*Advanced | Javascript/Typescript*

**Objective**: Implement a polyfill for `Promise.all`, which takes an array of promises and returns a single promise that resolves when all of the input promises have resolved.

**Instructions**:

1. Create a function named `promiseAll` that mimics the behavior of `Promise.all`.
2. The function should take an array of promises and return a single promise that:
   - Resolves with an array of resolved values when all promises are fulfilled.
   - Rejects immediately with the reason of the first promise that rejects.

**Example Usage**:

```js
promiseAll([promise1, promise2, promise3])
  .then(values => console.log(values))  // All promises fulfilled, output an array of results
  .catch(error => console.error(error));  // One of the promises rejected
```

**Requirements**:

- The `promiseAll` function should take an array of promises as input.
- It should resolve with an array of resolved values if all promises resolve.
- It should reject immediately with the reason of the first promise that rejects.
- **You cannot use the native `Promise.all.`**
  
**Hints:**

- Use Promise.resolve() and Promise.reject() to handle the result of each promise.
- Return a new promise that resolves or rejects based on the input promises.

**Bonus:**

1. Handle non-promise values in the array by treating them as resolved promises.

## 15. Floating Chat Widget

*Intermediate | Javascript/Typescript/React*

**Objective**: Implement a floating chat widget that mimics a customer support chatbox, which can be opened and minimized.

**Instructions**:

1. Create a floating button on the `bottom-right` of the screen that, when clicked, opens a chat window.
2. The chat window should allow users to type and send messages.
3. Include a button to close or minimize the chat window, returning to just the floating button.

**Requirements**:

- The floating button should be fixed to the `bottom-right` corner of the screen.
- The chat window should appear and disappear when the floating button is clicked.
- Users should be able to send messages in the chat window *(no actual backend needed for this task)*.
- The chat window stays open as long as the user is interacting with it.

**Bonus**:

- Add basic chat-like functionality where the chat window displays sent messages in real time.
- Implement a smooth transition effect when the chat window opens or closes.
- Make chat window resizable.
 
## 16. Throttle API Calls

**Objective**: Implement a function that throttles API calls, make sure that a function is only executed once within a specified time window, even if it's triggered multiple times.

**Instructions**:

1. Create a function named `throttle` that limits how often an API call is made. If the function is called again within the time window, it should ignore the subsequent calls until the window has passed.
2. The function should take two arguments: 
   - The API call function to throttle.
   - The throttle time in milliseconds (e.g., 2000 ms for a 2-second throttle).
3. Ensure the function can handle multiple calls but only executes the API call once per time window.

**Example Usage:**

*Advanced | Javascript/Typescript/React*

```js
const throttledApiCall = throttle(apiCall, 2000);

button.addEventListener('click', throttledApiCall); 
// Only allows the API call once every 2 seconds, even if the button is clicked multiple times.
```

**Requirements:**

- Create a `throttle` function that limits how frequently an API call can be made.
- The function should ignore subsequent calls during the window and only execute after the window has passed.
- Ensure the API call function is executed at least once after the throttle window resets.

**Hints:**

1. Use `setTimeout` or timestamps to track the time between calls.
2. Consider using `closures` to keep track of the throttle state between function calls.

**Bonus:**

1. Allow the `throttle` function to accept an option that triggers the first call immediately, but enforces the throttle after that.

## 17. Multistep Form

*Intermediate | Javascript/Typescript/React*

**Note**: This challenge focuses more on logic than UI. If you want to also focus on and practice UI, visit our **UI Components** challenges.

**Objective**: Implement a multistep form with 3 steps, where users can input data and navigate back and forth between steps.

**Instructions**:

1. Create a form with at least 3 steps. Each step should contain a set of input fields.
   - Step 1: Personal Information (e.g., Name, Email).
   - Step 2: Contact Details (e.g., Phone Number, Address).
   - Step 3: Review (Display entered information for review before submission).
   
2. Include "Next" and "Back" buttons to allow users to navigate between the steps.

3. On the final step, provide a "Submit" button that `console.logs` or processes the form data.

**Requirements**:

- Users should be able to move between steps using the "Next" and "Back" buttons.
- The form data should persist as users navigate between steps.

**Hints**:

1. Use an array or object to store the form data and update it as the user progresses through the steps.

**Bonus**:

1. Implement validation for the form fields (e.g., email format, required fields).
2. Allow users to directly jump to a specific step if they’ve already visited it. 
3. Show a summary of all entered information on the final review step before submission.

## 18. Memoize Function

*Expert | Javascript/Typescript/React*

**Objective**: Implement a memoization function that caches the results of function calls to improve performance.

**Instructions**:

1. Create a function named `memoize` that takes a function as an argument and returns a new function that caches the results of the function.
2. The memoized function should store the results of previous calls and return the cached result when the same arguments are provided.
3. The function should only recompute the result if the arguments have changed.

**Example Usage**:

```js
const slowFunction = (num) => {
  // Simulate a slow computation
  return new Promise((resolve) => {
    setTimeout(() => resolve(num * 2), 3000); // Simulates a 3-second delay
  });
};

const memoizedFunction = memoize(slowFunction);

memoizedFunction(5).then(result => console.log(result));  // Calls slowFunction, outputs: 10 after 3 seconds
memoizedFunction(5).then(result => console.log(result));  // Returns cached result, outputs: 10 immediately
```

**Requirements:**

- The `memoize` function should cache the result of previous function calls based on the arguments provided.
- When called with the same arguments, the function should return the cached result instead of recomputing it.
- The cache should clear or replace old values when new ones are computed.
  
**Hints:**

1. Use an `object` or `Map` to store the function arguments and their corresponding results.
2. Consider how you will handle multiple arguments and different types of data.

**Bonus:**

1. Implement a cache size limit, where the oldest cached result is removed when the cache reaches its limit.
2. Add support for handling multiple arguments and deep comparisons of objects.

## 19. Dark Mode Toggler

*Beginner | Javascript/Typescript/React*

**Note**: This challenge focuses more on logic than UI. If you want to also focus on and practice UI, visit our **UI Components** challenges.

**Objective**: Implement a dark mode toggle that switches between light and dark modes.

**Instructions**:

1. Create a button or switch that toggles between light and dark modes when clicked.
2. Create some basic CSS styles to indicate theme difference

**Requirements**:

- Implement a function that toggles between light and dark modes.
- Create basic CSS theme for light/dark mode.

**Bonus**:

1. Automatically detect the user's OS-level dark mode preference and apply it on first load.
2. Add a transition effect when switching between modes.

## 20. Rate limiter

*Expert | Javascript/Typescript*

**Objective**: Implement a rate limiter that restricts the number of function executions within a specified time window.

**Instructions**:

1. Create a function named `rateLimiter` that accepts two arguments:
   - A function to limit.
   - The maximum number of times the function can be executed within a specified time window (e.g., 5 times per 10 seconds).
2. Ensure that after reaching the limit, the function is blocked from executing until the time window resets.

**Example Usage**:

```js
const limitedFunction = rateLimiter(apiCall, 5, 10000); // 5 calls per 10 seconds

limitedFunction(); // Executes the first call
limitedFunction(); // Executes the second call
// After 5 calls in 10 seconds, the function will be blocked until the next window starts.
```

**Requirements:**

- The `rateLimiter` should limit how many times the function can be executed within a specific time window.
- Once the limit is reached, further function calls should be blocked until the time window resets.
- The time window should reset after a specified duration (e.g., every 10 seconds).
- 
**Hints:**

1. Use timestamps to track when the time window starts and the number of function calls.
2. Use a counter to track how many times the function has been executed within the time window.

**Bonus:**

1. Add the ability to reset the limiter manually.
2. Add key for each action, so different actions can be rate limited separately

## 21. Infinite Carousel

*Intermediate | Javascript/Typescript/React*

**Note**: This challenge focuses more on logic than UI. If you want to also focus on and practice UI, visit our **UI Components** challenges.

**Objective**: Implement an infinite carousel component that allows users to cycle through items.

**Instructions**:

1. Create a carousel that displays a series of items (e.g., images or cards) one at a time.
2. The carousel should loop infinitely, meaning that when the user reaches the last item, it cycles back to the first, and vice versa.
3. Include "Next" and "Previous" buttons to allow users to navigate through the items.

**Requirements**:

- The carousel should loop infinitely, so users can navigate through the items without reaching an end.
- Add at least 5 items.

**Hints**:

1. Use a state variable or index to track the current item in the carousel.
2. Reset the index to the start or end when it goes out of bounds to create the infinite loop.
3. Use a timer or interval to handle the automatic cycling of items (bonus).

**Bonus**:

1. Automatic cycling - The carousel automatically cycles through the items after a set interval.

## 22. Flatten nested Object

*Advanced | Javascript/Typescript*

**Objective:** Write a function that takes a deeply nested object and returns a flat object with all keys flattened.

**Instructions:**

1. Create a function called `flattenObject` that accepts an object with nested objects at various levels.
2. The function should return a new object where all nested keys are flattened into a single-level object, with the keys representing the nested structure using dot notation (e.g., `'key1.key2': value`).

**Example:**

```js
flattenObject({
  a: 1,
  b: { 
    c: 2, 
    d: { 
      e: 3 
    }
  }
});
// Output: { 'a': 1, 'b.c': 2, 'b.d.e': 3 }
```

**Requirements:**

- The function must handle objects with multiple levels of nesting.
- The function should work recursively to flatten deeply nested objects.
- You cannot use any built-in flattening utilities.

**Hints:**

1. Use `recursion` to flatten nested objects.
2. Use dot notation to `concatenate` keys as you go deeper into nested objects.

**Bonus:**

1. Add a second argument to the function that limits how deep the object should be flattened.

## 23. Toast Notifications

*Intermediate | Javascript/Typescript/React*

**Note**: This challenge focuses more on logic than UI. If you want to also focus on and practice UI, visit our **UI Components** challenges.

**Objective**: Implement a toast notification that allows displaying temporary messages that automatically disappear after a certain time.

**Instructions**:

1. Create a function or component to show toast notifications with a message.
2. Each notification should disappear automatically after a specified duration (e.g., 3 seconds).
3. Provide the ability to trigger multiple notifications and display them in a queue.

**Requirements**:

- The toast notifications should be temporary and automatically disappear after a set time.
- Support multiple notifications at once, displayed in a queue (stacked on top of each other).

**Hints**:

1. Use a timeout to control how long each notification stays visible.
2. Use an array to manage multiple notifications and their removal from the list.

**Bonus**:

1. Allow the user to dismiss a notification manually by clicking a close button.
2. Add different types of notifications (e.g., success, error, info) with corresponding styles.

## 24. Event queue

*Advanced | Javascript/Typescript/React*

**Objective:** Implement an event queue system that manages user actions (like liking posts) in sequence and handles cancelable events (e.g., like + unlike = no action).

**Instructions:**

1. Create a function called `createEventQueue` that manages an event queue.
2. The event queue should support adding and canceling actions (e.g., "like post" followed by "unlike post" results in no event).
3. Ensure that events are processed in the order they were added, but allow new events to be triggered while previous events are still being processed.

**Example:**

```js
const eventQueue = createEventQueue();

eventQueue.add('like', () => console.log('Liked post 1'));
eventQueue.add('unlike', () => console.log('Unliked post 1'));
eventQueue.add('like', () => console.log('Liked post 2'));

// Output:
// Liked post 2

// In this case, the "like" and "unlike" actions for post 1 cancel each other,
// so only the "Liked post 2" event is processed.
```

**Requirements:**

- Create a queue system that stores actions and processes them in sequence.
- Ensure that cancelable actions (like/unlike) cancel each other when triggered for the same post.
- Provide a way to trigger new events while the queue is still being processed.
   
**Hints:**

1. Use an array to store the events in the queue.
2. Keep track of actions (like/unlike) to determine if they cancel each other out before executing them.

## 25. Keyboard Navigation

**Beginner | Javascript/Typescript/React**

**Objective**: Implement a simple keyboard navigation system that allows users to navigate between pages, create new pages, and delete pages using keyboard input.

**Instructions**:

1. Create a system starting with 10 pages, each representing a simple page (can be a numbered div or section).
2. Use the **left** and **right** arrow keys to navigate between pages.
3. Pressing **Enter** should create a new page.
4. Pressing **Backspace** should delete the current page.

**Requirements**:

- The system should have 10 pages by default.
- Allow users to navigate between pages using the left and right arrow keys.
- Pressing **Enter** should add a new page, and pressing **Backspace** should delete the current page.
- Ensure the user cannot navigate beyond the first or last page.

**Example Usage**:

- **Left arrow**: Moves to the previous page.
- **Right arrow**: Moves to the next page.
- **Enter**: Creates a new page at the current position.
- **Backspace**: Deletes the current page.

**Hints**:

1. Use **keyboard event listeners** to detect key presses.
2. Store the pages in an array and update the navigation state accordingly.
3. Ensure that creating or deleting pages updates the total number of pages and maintains navigation logic.

**Bonus**:

1. Allow the user to skip to the first or last page using the **Home** and **End** keys.

## 26. Image Lazy Loading

**Intermediate | Javascript/Typescript/React**

**Objective**: Implement a lazy loading mechanism for images, so they load only when they are about to enter the user's viewport, improving performance and reducing unnecessary network requests.

**Instructions**:

1. Build simple scrollable page with any images.
2. Create a function or component that handles the lazy loading of images.
2. The images should only load when they are about to enter the viewport.
3. Ensure that the mechanism works across multiple images on the page.

**Requirements**:

- The images should not load until they are close to appearing in the viewport.
- Use a placeholder or a loading indicator until the image has fully loaded.
- The lazy loading should work for multiple images on a single page.

**Hints**:

1. Use the **Intersection Observer API** to detect when the images are about to enter the viewport.
2. Replace the placeholder with the actual image URL when the image is about to load.

## 27. Dialog with Actions (Cancel/Confirm)

**Intermediate | Javascript/Typescript/React**

**Note**: This challenge focuses more on logic than UI. If you want to also focus on and practice UI, visit our **UI Components** challenges.

**Objective**: Implement an alert dialog that displays a message and provides "Cancel" and "Confirm" buttons for user interaction.

**Instructions**:

1. Create a component that displays an alert dialog with a message.
2. Include two actions in the dialog: "Cancel" and "Confirm".
3. The "Cancel" action should close the dialog without any further action.
4. The "Confirm" action should trigger a specified function and then close the dialog.

**Requirements**:

- The dialog should be a modal, meaning it blocks interaction with the rest of the page until the user takes an action.
- The component should handle both "Cancel" and "Confirm" actions appropriately.

**Hints**:

1. Use a arguments/props to control the visibility of the dialog.
2. Ensure the dialog is positioned and styled to be centered on the screen.
3. Use event listeners to close the dialog when clicking outside of it or pressing the "Escape" key.

## 28. Deep Clone Function

**Advanced | Javascript/Typescript**

**Objective**: Implement a function that creates a deep clone of a given object or array, ensuring that all nested structures are also cloned.

**Instructions**:

1. Create a function named `deepClone` that takes an object or array as an argument and returns a deep copy of it.
2. The cloned object or array should not share references with the original (i.e., modifying the clone should not affect the original).
3. Handle nested objects and arrays, ensuring all levels are cloned.

**Example Usage**:

```js
const original = { a: 1, b: { c: 2 } };
const cloned = deepClone(original);

cloned.b.c = 3;

console.log(original.b.c); // Output: 2 (original remains unchanged)
console.log(cloned.b.c);   // Output: 3 (cloned object is independent)
```

**Requirements:**

- The `deepClone` function should work recursively to clone deeply nested `objects` and `arrays`.
- The function should handle primitive values, `arrays`, and `objects` (not `Dates` or `RegExp`)
  
**Hints:**

1. Use recursion to iterate through the structure of the object or array.
2. Ensure that each nested object or array is cloned and not simply referenced.

## 29. Password Strength Indicator

**Intermediate | Javascript/Typescript**

**Objective**: Implement a function that evaluates the strength of a password based on certain criteria and returns a strength score or label.

**Instructions**:

1. Create a function called `checkPasswordStrength` that takes a password as input.
2. The function should evaluate the password based on the following criteria:
   - Length of the password.
   - Inclusion of uppercase and lowercase letters.
   - Inclusion of numbers.
   - Inclusion of special characters (e.g., `!@#$%^&*`).
3. The function should return a score or label such as "Weak", "Medium", or "Strong".

**Example Usage**:

```js
console.log(checkPasswordStrength('Password123'));  // Output: "Medium"
console.log(checkPasswordStrength('Password@123'));  // Output: "Strong"
console.log(checkPasswordStrength('pass'));  // Output: "Weak"
```

**Requirements:**

- The function should check for a combination of length, character variety (uppercase, lowercase, numbers, special characters).
- Return a label or score to indicate the password strength.

**Hints:**

1. Use `regular expressions` to check for the presence of numbers, uppercase letters, and special characters.
2. Create a point system based on the criteria and return the label based on the score.

**Bonus:**

1. Provide suggestions to improve a weak password (e.g., "Add special characters").
2. Allow customization of strength rules (e.g., minimum length, required character types).

## 30. Mini Form Validation Library

**Intermediate | Javascript/Typescript**

**Objective**: Implement a simple form validation library that allows validating form fields based on custom rules.

**Instructions**:

1. Create a function named `validateForm` that takes an object representing form data and an object representing validation rules.
2. The function should validate each field based on the provided rules and return a result indicating whether the form is valid and what errors (if any) were found.
3. The validation rules should support checks for:
   - Required fields
   - Minimum/maximum length for text fields
   - Email format validation

**Example Usage**:

```js
const formData = {
  username: 'user123',
  password: 'pass',
  email: 'user@example.com',
};

const validationRules = {
  username: { required: true, minLength: 5 },
  password: { required: true, minLength: 8 },
  email: { required: true, email: true },
};

const result = validateForm(formData, validationRules);
console.log(result);
// Output: { valid: false, errors: { password: 'Password must be at least 8 characters.' } }
```

**Requirements:**

- The function should validate based on rules like required, minLength, and email format.
- Return an object with a valid boolean and an errors object indicating what validation failed.

**Bonus:**

1. Add support for validating multiple types of fields (e.g., numbers, dates).