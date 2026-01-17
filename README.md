# Gravity-Flow-School
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gravity Flow School</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header class="nav">
  <div class="logo">Gravity Flow School</div>
  <nav>
    <a href="#kurse">Kurse</a>
    <a href="#orte">Orte</a>
    <a href="#buchung">Buchung</a>
    <a href="#kontakt">Kontakt</a>
  </nav>
</header>

<section class="hero">
  <h1>Fahrtechnik.<br>Kontrolle.<br>Flow.</h1>
  <p>Moderne Fahrtechnikschule für Gravity, Enduro & Urban Riding</p>
  <a href="#kurse" class="btn">Kurse entdecken</a>
</section>

<section id="kurse" class="section">
  <h2>Kurse</h2>
  <div class="grid">
    <div class="card">
      <img src="assets/winterberg.jpg">
      <h3>Gravity & Enduro</h3>
      <p>Linienwahl, Kontrolle, Sicherheit & Flow auf anspruchsvollen Trails.</p>
      <span class="tag">Fortgeschritten</span>
    </div>
    <div class="card">
      <img src="assets/city.jpg">
      <h3>Urban & City</h3>
      <p>Fahrtechnik, Balance und Sicherheit im urbanen Raum.</p>
      <span class="tag">Coming Soon</span>
    </div>
  </div>
</section>

<section id="orte" class="section dark">
  <h2>Kursorte</h2>
  <div class="grid">
    <div class="card">
      <img src="assets/winterberg.jpg">
      <h3>Winterberg Bikepark</h3>
      <p>Gravity & Enduro Training auf natürlichen und gebauten Strecken.</p>
    </div>
    <div class="card">
      <img src="assets/wuppertal.jpg">
      <h3>Wuppertal Kothen</h3>
      <p>Downhill-Strecke mit Fokus auf Technik & Linienwahl.</p>
    </div>
  </div>
</section>

<section id="buchung" class="section">
  <h2>Kurs buchen</h2>

  <form class="booking-form">
    <select required>
      <option value="">Kurs auswählen</option>
      <option>Gravity & Enduro</option>
      <option>Urban & City (geplant)</option>
    </select>

    <select required>
      <option value="">Ort auswählen</option>
      <option>Winterberg Bikepark</option>
      <option>Wuppertal Kothen</option>
    </select>

    <input type="date" required>
    <input type="text" placeholder="Name" required>
    <input type="email" placeholder="E-Mail" required>

    <button type="submit">Anfrage senden</button>
  </form>

  <p class="hint">Preise & Termine werden individuell bestätigt.</p>
</section>

<section id="kontakt" class="section dark">
  <h2>Kontakt</h2>
  <p>Fragen oder individuelle Kursanfragen?</p>
  <p><strong>E-Mail:</strong> info@gravityflow.school</p>
</section>

<footer>
  <p>© 2026 Gravity Flow School</p>
</footer>

<script src="script.js"></script>
</body>
</html>

 * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}

body {
  color: #111;
  background: #fff;
}

.nav {
  position: fixed;
  top: 0;
  width: 100%;
  background: rgba(255,255,255,0.9);
  display: flex;
  justify-content: space-between;
  padding: 20px 60px;
  z-index: 10;
}

.nav a {
  margin-left: 30px;
  text-decoration: none;
  color: #111;
}

.hero {
  height: 100vh;
  padding: 140px 60px;
  background: linear-gradient(180deg,#fff,#f2f2f2);
}

.hero h1 {
  font-size: 72px;
  line-height: 1.1;
}

.hero p {
  margin-top: 20px;
  font-size: 22px;
}

.btn {
  display: inline-block;
  margin-top: 40px;
  padding: 14px 32px;
  background: #000;
  color: #fff;
  text-decoration: none;
  border-radius: 30px;
}

.section {
  padding: 120px 60px;
}

.section.dark {
  background: #000;
  color: #fff;
}

.section h2 {
  font-size: 48px;
  margin-bottom: 60px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
  gap: 40px;
}

.card {
  background: #fff;
  color: #000;
  border-radius: 24px;
  overflow: hidden;
}

.dark .card {
  background: #111;
  color: #fff;
}

.card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
}

.card h3 {
  padding: 20px;
  font-size: 24px;
}

.card p {
  padding: 0 20px 20px;
}

.tag {
  margin: 0 20px 20px;
  display: inline-block;
  font-size: 14px;
  opacity: 0.7;
}

.booking-form {
  max-width: 500px;
  display: grid;
  gap: 20px;
}

.booking-form input,
.booking-form select,
.booking-form button {
  padding: 14px;
  border-radius: 12px;
  border: 1px solid #ccc;
}

.booking-form button {
  background: #000;
  color: #fff;
  border: none;
}

footer {
  padding: 40px;
  text-align: center;
  font-size: 14px;
}
