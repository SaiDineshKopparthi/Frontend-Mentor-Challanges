## 1️⃣ Default State (.links li & .links a)

- `li` elements:
  - `transition: background-color 0.3s ease-in-out 0.1s;`
    - **0.3s duration:** The transition from one color to another will take 0.3 seconds.
    - **ease-in-out:** The speed of the transition slows down at the beginning and end.
    - **0.1s delay:** The effect waits for 0.1 seconds before applying the change.

- `a` (links inside `li` elements):
  - `display: block;` ensures the anchor fills the entire list item.
  - `transition: color 0.3s ease-in-out 0.1s;`
    - The text color transition takes 0.3s, starts slow, speeds up, and then slows again.
    - 0.1s delay before the color change happens.

## 2️⃣ Hover, Active & Focus States (.links li:hover, .links li:active, .links li:focus-visible)

- When the user hovers, clicks (:active), or navigates using the keyboard (:focus-visible):
  - The transition is now faster (0.2s) and does not have a delay.

## 3️⃣ Link Color Change Inside Hovered li (.links li:hover a, .links li:active a, .links li:focus-visible a)

- The color transition happens in 0.2s with no delay.

## 🔥 Final Effect
2. The hover transition happens quickly, making the UI feel responsive.
3. When the user removes the cursor, the background slowly transitions back to var(--Gray-700), with a slight delay, making it feel smooth.