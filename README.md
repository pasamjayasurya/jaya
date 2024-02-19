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
