Create a responsive seat selector UI in HTML, CSS, and JS
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Movie Tickets Online Booking</title>
    <link
      rel="icon"
      type="image/x-icon"
      href="./assets/images/movie-favicon.png"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css"
      integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w=="
      crossorigin="anonymous"
      referrerpolicy="no-referrer"
    />
    <link rel="stylesheet" href="./styles/normalize.css" />
    <link rel="stylesheet" href="./styles/style.css" />
  </head>
  <body>
    <div class="main-container">
      <div class="container">
        <div class="movie-container">
          <label for="movie">Select a Movie</label>
          <select name="movie" id="movie">
            <option value="190"> Jailer</option>
            <option value="150"> PS - 2</option>
            <option value="150"> Pisasu - 2</option>
            <option value="190"> Vikram - 2</option>
          </select>
        </div>
        <ul class="showcase-container">
          <li>
            <div class="seat sold"></div>
            <small>Sold</small>
          </li>
          <li>
            <div class="seat available"></div>
            <small>Available</small>
          </li>
          <li>
            <div class="seat selected"></div>
            <small>Selected</small>
          </li>
        </ul>
        <div class="seating-container">
        <div class="screen"></div>
        <div class="row">
          <div class="seat"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
        </div>
        <div class="row">
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
        </div>
        <div class="row">
          <div class="seat"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
        </div>
        <div class="row">
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
        </div>
        <div class="row">
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat sold"></div>
          <div class="seat sold"></div>
          <div class="seat"></div>
          <div class="seat"></div>
          <div class="seat"></div>
        </div>
        <div class="summary">
          <p>You have selected <span class="bold" id="count">0</span> seats, total price is ₹<span class="bold" id="total">0</span> </p>
        </div>
      </div>
    </div>
    <script src="./scripts/script.js"></script>
  </body>
</html>




/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */

/* Document
   ========================================================================== */

/**
 * 1. Correct the line height in all browsers.
 * 2. Prevent adjustments of font size after orientation changes in iOS.
 */

html {
  line-height: 1.15; /* 1 */
  -webkit-text-size-adjust: 100%; /* 2 */
}

/* Sections
   ========================================================================== */

/**
 * Remove the margin in all browsers.
 */

body {
  margin: 0;
}

/**
 * Render the `main` element consistently in IE.
 */

main {
  display: block;
}

/**
 * Correct the font size and margin on `h1` elements within `section` and
 * `article` contexts in Chrome, Firefox, and Safari.
 */

h1 {
  font-size: 2em;
  margin: 0.67em 0;
}

/* Grouping content
   ========================================================================== */

/**
 * 1. Add the correct box sizing in Firefox.
 * 2. Show the overflow in Edge and IE.
 */

hr {
  box-sizing: content-box; /* 1 */
  height: 0; /* 1 */
  overflow: visible; /* 2 */
}

/**
 * 1. Correct the inheritance and scaling of font size in all browsers.
 * 2. Correct the odd `em` font sizing in all browsers.
 */

pre {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/* Text-level semantics
   ========================================================================== */

/**
 * Remove the gray background on active links in IE 10.
 */

a {
  background-color: transparent;
}

/**
 * 1. Remove the bottom border in Chrome 57-
 * 2. Add the correct text decoration in Chrome, Edge, IE, Opera, and Safari.
 */

abbr[title] {
  border-bottom: none; /* 1 */
  text-decoration: underline; /* 2 */
  -webkit-text-decoration: underline dotted;
  text-decoration: underline dotted; /* 2 */
}

/**
 * Add the correct font weight in Chrome, Edge, and Safari.
 */

b,
strong {
  font-weight: bolder;
}

/**
 * 1. Correct the inheritance and scaling of font size in all browsers.
 * 2. Correct the odd `em` font sizing in all browsers.
 */

code,
kbd,
samp {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/**
 * Add the correct font size in all browsers.
 */

small {
  font-size: 80%;
}

/**
 * Prevent `sub` and `sup` elements from affecting the line height in
 * all browsers.
 */

sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}

sub {
  bottom: -0.25em;
}

sup {
  top: -0.5em;
}

/* Embedded content
   ========================================================================== */

/**
 * Remove the border on images inside links in IE 10.
 */

img {
  border-style: none;
}

/* Forms
   ========================================================================== */

/**
 * 1. Change the font styles in all browsers.
 * 2. Remove the margin in Firefox and Safari.
 */

button,
input,
optgroup,
select,
textarea {
  font-family: inherit; /* 1 */
  font-size: 100%; /* 1 */
  line-height: 1.15; /* 1 */
  margin: 0; /* 2 */
}

/**
 * Show the overflow in IE.
 * 1. Show the overflow in Edge.
 */

button,
input {
  /* 1 */
  overflow: visible;
}

/**
 * Remove the inheritance of text transform in Edge, Firefox, and IE.
 * 1. Remove the inheritance of text transform in Firefox.
 */

button,
select {
  /* 1 */
  text-transform: none;
}

/**
 * Correct the inability to style clickable types in iOS and Safari.
 */

button,
[type="button"],
[type="reset"],
[type="submit"] {
  -webkit-appearance: button;
}

/**
 * Remove the inner border and padding in Firefox.
 */

button::-moz-focus-inner,
[type="button"]::-moz-focus-inner,
[type="reset"]::-moz-focus-inner,
[type="submit"]::-moz-focus-inner {
  border-style: none;
  padding: 0;
}

/**
 * Restore the focus styles unset by the previous rule.
 */

button:-moz-focusring,
[type="button"]:-moz-focusring,
[type="reset"]:-moz-focusring,
[type="submit"]:-moz-focusring {
  outline: 1px dotted ButtonText;
}

/**
 * Correct the padding in Firefox.
 */

fieldset {
  padding: 0.35em 0.75em 0.625em;
}

/**
 * 1. Correct the text wrapping in Edge and IE.
 * 2. Correct the color inheritance from `fieldset` elements in IE.
 * 3. Remove the padding so developers are not caught out when they zero out
 *    `fieldset` elements in all browsers.
 */

legend {
  box-sizing: border-box; /* 1 */
  color: inherit; /* 2 */
  display: table; /* 1 */
  max-width: 100%; /* 1 */
  padding: 0; /* 3 */
  white-space: normal; /* 1 */
}

/**
 * Add the correct vertical alignment in Chrome, Firefox, and Opera.
 */

progress {
  vertical-align: baseline;
}

/**
 * Remove the default vertical scrollbar in IE 10+.
 */

textarea {
  overflow: auto;
}

/**
 * 1. Add the correct box sizing in IE 10.
 * 2. Remove the padding in IE 10.
 */

[type="checkbox"],
[type="radio"] {
  box-sizing: border-box; /* 1 */
  padding: 0; /* 2 */
}

/**
 * Correct the cursor style of increment and decrement buttons in Chrome.
 */

[type="number"]::-webkit-inner-spin-button,
[type="number"]::-webkit-outer-spin-button {
  height: auto;
}

/**
 * 1. Correct the odd appearance in Chrome and Safari.
 * 2. Correct the outline style in Safari.
 */

[type="search"] {
  -webkit-appearance: textfield; /* 1 */
  outline-offset: -2px; /* 2 */
}

/**
 * Remove the inner padding in Chrome and Safari on macOS.
 */

[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}

/**
 * 1. Correct the inability to style clickable types in iOS and Safari.
 * 2. Change font properties to `inherit` in Safari.
 */

::-webkit-file-upload-button {
  -webkit-appearance: button; /* 1 */
  font: inherit; /* 2 */
}

/* Interactive
   ========================================================================== */

/*
 * Add the correct display in Edge, IE 10+, and Firefox.
 */

details {
  display: block;
}

/*
 * Add the correct display in all browsers.
 */

summary {
  display: list-item;
}

/* Misc
   ========================================================================== */

/**
 * Add the correct display in IE 10+.
 */

template {
  display: none;
}

/**
 * Add the correct display in IE 10.
 */

[hidden] {
  display: none;
}

`use strict`;
// select elements
const movieEl = document.getElementById(`movie`);
const seatContainerEl = document.querySelector(`.seating-container`);
const countEl = document.getElementById(`count`);
const totalEl = document.getElementById(`total`);

// global variables
let seatCount = 0;
let ticketPrice = Number(movieEl.value);

// function
const totalPrice = function () {
  ticketPrice = Number(movieEl.value);
  countEl.textContent = seatCount;
  totalEl.innerText = seatCount * ticketPrice;
};

// event listeners
movieEl.addEventListener(`change`, function () {
  ticketPrice = Number(movieEl.value);
  totalPrice();
});
seatContainerEl.addEventListener(`click`, function (e) {
  if (e.target.classList.contains(`seat`)) {
    if (!e.target.classList.contains(`sold`)) {
      e.target.classList.toggle(`selected`);
      const selectedSeatEl = document.querySelectorAll(`.row .seat.selected`);
      seatCount = selectedSeatEl.length;
      totalPrice();
    }
  }
});

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  outline: none;
}

:root {
  --grey-outer: #f8f8f8;
  --grey-inner: #e5e5e5;
  --selected-clr: #1ea83c;
  --sold-clr: #696767;
  --screen-clr: #d9e6fb;
  --white-clr: #ffffff;
  --max-width: 1140px;
}

html {
  font-size: 16px;
  scroll-behavior: smooth;
}

body {
  font-family: "Poppins", sans-serif;
  background-color: var(--grey-outer);
}

a {
  text-decoration: none;
}

li {
  list-style: none;
}

select {
  border: none;
}

img {
  width: 100%;
  height: auto;
}

.main-container {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  background-color: var(--grey-inner);
  text-align: center;
  border-radius: 48px;
  width: 40rem;
}

.movie-container {
  font-size: 1.2rem;
  font-weight: 600;
  margin-top: 2rem;
}

select {
  border-radius: 8px;
  width: 8rem;
  font-size: 1.1rem;
  font-weight: 500;
}

option {
  text-align: left;
}

.seat {
  background-color: var(--white-clr);
  background-image: url(../assets/images/seat-icon.png);
  background-size: cover;
  width: 1.5rem;
  height: 1.5rem;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}

.seat.sold {
  background-color: var(--sold-clr);
}

.seat.selected {
  background-color: var(--selected-clr);
}

.showcase-container li {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.4rem;
}

.seating-container .seat:hover {
  cursor: pointer;
  /* background-color: var(--selected-clr); */
}

.seating-container .seat.sold:hover {
  cursor: default;
  background-color: var(--sold-clr);
}

.showcase-container {
  margin-top: 2rem;
  font-size: 1.2rem;
  font-weight: 600;
  background-color: rgba(0, 0, 0, 0.05);
  height: 2.5rem;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.seating-container {
  height: 400px;
  display: flex;
  flex-direction: column;
  align-items: center;
  perspective: 1000px;
}

.screen {
  margin-bottom: 1rem;
  background-color: var(--white-clr);
  width: 12rem;
  height: 2rem;
  padding: 3rem;
  transform: rotateX(-45deg);
  box-shadow: 0 25px 25px rgba(255, 255, 255, 0.8);
}

.row {
  height: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 1.2rem;
}

.seat:nth-of-type(3) {
  margin-left: 1.5rem;
}

.seat:nth-last-of-type(3) {
  margin-left: 1.5rem;
}

.summary {
  margin-top: 1rem;
}

@media screen and (max-width: 375px) {
  .container {
    width: 25rem;
  }

  .showcase-container li {
    margin-right: 1rem;
  }

  .row {
    column-gap: 0.5rem;
  }

  .summary {
    text-align: justify;
  }
}
