# Let's make a sound board!

We going to build the ultimate musical instrument -- a web application that plays sound when you click buttons!

## Step 0 -- Prerequisites

To take full advangage of this repository, you'll need to install [node and npm](https://nodejs.org).

## Step 1 -- Install Dependencies

Within this repository, run

```sh
npm install
```

This installs a small 'live-server' program that will serve and automatically reload the page as you make changes.

## Step 2 -- Test Web App

```sh
npm start
```

This starts the 'live-server' module.

Navigate to [http://localhost:8080](http://localhost:8080) or [http://127.0.0.1:8080](http://127.0.0.1:8080).

You should see a page that displays "Sound Board".

## Step 3 -- Add sound object

Within [index.html](./index.html) find the comment

```javascript
// ADD CODE HERE
```

replace it with

```javascript
const beep = new Audio('./beep.wav');
```

and save the page.

This does nothing visually, but it crates an object named "beep" and loads the included `./beep.wav` file into the page for later use.

## Step 4 -- Add button

Within [index.html](./index.html) find the comment

```html
<!-- ADD BUTTONS HERE -->
```

replace it with 

```html
<button onclick="beep.play()">BEEP</button>
```

and save the page.

This adds a button to the page with the text "BEEP". 

Notice "onclick" attribute. This calls a method, on the "beep" object from the previous step. This method plays the loaded file "./beep.wav".

You soundboard is now functional!, but because we'll be adding more buttons, we'll want to set up 

## Step 5 -- Add Style

Within [index.html](./index.html) find the comment

```css
/* ADD STYLES HERE */
```

replace it with 

```css
.soundboard {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

and save the page.

This ensures that as buttons you add more buttons, they will be arranged into a grid with 3 columns.

## Step 6 -- The Challenge

Now that you know how to add one, add three or more original sounds to the board.

You can get files from anywhere, but here are some recommendations:

- [Leashy SF Maker](https://www.leshylabs.com/apps/sfMaker/) can be used to creat sound effect programatically.

- [Online Voice Recorder](https://online-voice-recorder.com/) can be used to record audio.
