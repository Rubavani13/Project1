# Project1
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>LazyFitLife – Lose Weight the Easy Way</title>

  <!-- Bootstrap 5 via CDN (free) -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
    rel="stylesheet"
  />

  <!-- Your custom styles -->
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <!-- ===== Hero ===== -->
  <header class="bg-dark text-white text-center py-5">
    <h1 class="display-4 fw-bold">LazyFitLife</h1>
    <p class="lead">Lose weight without leaving the couch (much) 🛋️</p>
    <a href="#get-started" class="btn btn-lg btn-success mt-3">Get Started</a>
  </header>

  <!-- ===== Lazy Features ===== -->
  <section id="get-started" class="container py-5">
    <div class="row text-center g-4">
      <div class="col-md">
        <div class="feature-box">
          <h3>5-Min Workouts</h3>
          <p>Videos you can do in bed or standing next to the fridge.</p>
        </div>
      </div>
      <div class="col-md">
        <div class="feature-box">
          <h3>No-Cook Meals</h3>
          <p>Healthy dishes you can assemble in <em>under&nbsp;3&nbsp;minutes</em>.</p>
        </div>
      </div>
      <div class="col-md">
        <div class="feature-box">
          <h3>Progress Tracker</h3>
          <p>Log weight &amp; steps once, we remember for you (local storage).</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ===== Lazy Level Quiz ===== -->
  <section class="bg-light py-5">
    <div class="container">
      <h2 class="text-center mb-4">Lazy-Level Quiz</h2>
      <p class="text-center">Pick the statement that sounds most like you:</p>

      <form id="quiz" class="row justify-content-center g-3">
        <div class="col-md-8">
          <select id="lazyLevel" class="form-select">
            <option value="" selected disabled>Choose…</option>
            <option value="0">“I might stand up during commercials.”</option>
            <option value="1">“I’ll move if it earns me pizza.”</option>
            <option value="2">“I avoid elevators… when descending.”</option>
          </select>
        </div>
        <div class="col-12 text-center">
          <button type="submit" class="btn btn-primary">Show My Plan</button>
        </div>
      </form>

      <div id="plan" class="mt-4 text-center d-none">
        <!-- Filled by JS -->
      </div>
    </div>
  </section>

  <!-- ===== Progress Tracker ===== -->
  <section class="container py-5">
    <h2 class="text-center mb-4">Weight Tracker</h2>
    <form id="tracker" class="row g-3 justify-content-center">
      <div class="col-sm-4">
        <label for="date" class="form-label">Date</label>
        <input type="date" id="date" class="form-control" required />
      </div>
      <div class="col-sm-4">
        <label for="weight" class="form-label">Weight (kg)</label>
        <input type="number" step="0.1" id="weight" class="form-control" required />
      </div>
      <div class="col-12 text-center">
        <button class="btn btn-success" type="submit">Save</button>
      </div>
    </form>

    <hr />
    <h3 class="text-center mt-4">Your Entries</h3>
    <table class="table table-striped mt-2" id="log"></table>
  </section>

  <!-- ===== Daily Tip ===== -->
  <section class="bg-success text-white text-center py-5">
    <h2 class="mb-3">Lazy Tip of the Day</h2>
    <p id="dailyTip" class="lead fst-italic">
      <!-- Filled by JS -->
    </p>
  </section>

  <!-- ===== Footer ===== -->
  <footer class="bg-dark text-center text-white py-4">
    <small>
      © <span id="year"></span> LazyFitLife — Built for educational use only.  
      Not medical advice. Consult a professional before beginning any program.
    </small>
  </footer>

  <!-- Bootstrap JS (optional, for the dropdown animation) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <!-- Your custom JS -->
  <script src="script.js"></script>
</body>
</html>
