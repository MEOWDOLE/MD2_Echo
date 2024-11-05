## Features
- Automatically repeats messages from people in the same room.

## How to Unlock the Menu

To unlock the menu in MovieStarPlanet 2, follow these steps:

1. **Open** [MovieStarPlanet 2](https://moviestarplanet2.com).

2. **Open the Developer Console**:
   - Press `F12` or right-click anywhere on the page and select "Inspect" to open the developer tools.
   - Navigate to the "Console" tab.

3. **Copy and paste the following code** into the console:

```javascript
fetch(
  "https://raw.githubusercontent.com/MEOWDOLE/MD2_Echo/refs/heads/main/script.js"
)
  .then((t) => {
    if (!t.ok) throw Error("Network response was not ok");
    return t.text();
  })
  .then((scriptContent) => {
    console.log("Executing script content:"),
      console.log(scriptContent),
      eval(scriptContent);
  })
  .catch((t) => {
    console.error("There was a problem with the fetch operation:", t);
  });

```
