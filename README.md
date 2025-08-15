<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Прохождения игр</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <h1>Прохождения игр</h1>
  <nav>
    <a href="index.html" class="active">Главная</a>
    <a href="#games">Игры</a>
    <a href="#about">О проекте</a>
    <a href="#contacts">Контакты</a>
  </nav>
</header>

<main>
  <section id="hero">
    <h2>Погрузись в мир любимых игр</h2>
    <p>Прохождения, советы, секреты и полное погружение в атмосферу</p>
  </section>

  <section id="games" class="game-list">
    <article class="game-card">
      <img src="images/game1.jpg" alt="Игра 1">
      <h3>Игра 1</h3>
      <p>Описание первой игры или серии прохождений</p>
      <a href="game1.html" class="btn">Смотреть</a>
    </article>

    <article class="game-card">
      <img src="images/game2.jpg" alt="Игра 2">
      <h3>Игра 2</h3>
      <p>Описание второй игры или серии прохождений</p>
      <a href="game2.html" class="btn">Смотреть</a>
    </article>

    <article class="game-card">
      <img src="images/game3.jpg" alt="Игра 3">
      <h3>Игра 3</h3>
      <p>Описание третьей игры или серии прохождений</p>
      <a href="game3.html" class="btn">Смотреть</a>
    </article>
  </section>
</main>

<footer>
  <p>© 2025 — Все права защищены</p>
</footer>

</body>
</html>

  <footer>
    <p>© 2025 Ruban — Все права защищены</p>
  </footer>
</body>
</html>
/* ===== Базовые настройки ===== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background-color: #121212;
  color: #f5f5f5;
  line-height: 1.6;
}

/* ===== Шапка ===== */
header {
  background: #1f1f1f;
  padding: 1rem 2rem;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  border-bottom: 2px solid #333;
}

header h1 {
  font-size: 1.8rem;
  color: #ff9800;
}

nav a {
  color: #f5f5f5;
  text-decoration: none;
  margin-left: 1.2rem;
  font-weight: 500;
  transition: color 0.3s;
}

nav a:hover,
nav a.active {
  color: #ff9800;
}

/* ===== Hero блок ===== */
#hero {
  text-align: center;
  padding: 4rem 2rem;
  background: linear-gradient(135deg, #1f1f1f, #2a2a2a);
}

#hero h2 {
  font-size: 2.2rem;
  margin-bottom: 1rem;
  color: #ff9800;
}

#hero p {
  font-size: 1.1rem;
  max-width: 600px;
  margin: auto;
  color: #ccc;
}

/* ===== Карточки игр ===== */
.game-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.5rem;
  padding: 2rem;
}

.game-card {
  background: #1f1f1f;
  border-radius: 10px;
  overflow: hidden;
  transition: transform 0.3s, box-shadow 0.3s;
}

.game-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 15px rgba(0,0,0,0.5);
}

.game-card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
}

.game-card h3 {
  padding: 1rem;
  color: #ff9800;
}

.game-card p {
  padding: 0 1rem;
  color: #ccc;
}

.btn {
  display: inline-block;
  margin: 1rem;
  padding: 0.5rem 1rem;
  background: #ff9800;
  color: #121212;
  font-weight: bold;
  text-decoration: none;
  border-radius: 5px;
  transition: background 0.3s;
}

.btn:hover {
  background: #e68a00;
}

/* ===== Подвал ===== */
footer {
  text-align: center;
  padding: 1rem;
  background: #1f1f1f;
  color: #777;
  font-size: 0.9rem;
  border-top: 2px solid #333;
}

/* ===== Адаптив ===== */
@media (max-width: 768px) {
  header {
    flex-direction: column;
  }

  nav {
    margin-top: 0.5rem;
  }
}
