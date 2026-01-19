# reservation.

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>Nail et moi</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      font-family: serif;
      background-color: #e6ded4;
      color: #5a4a42;
      text-align: center;
    }

    header {
      padding: 80px 20px;
      background: #efe8df;
    }

    h1 {
      font-size: 40px;
      margin-bottom: 10px;
    }

    .btn {
      padding: 12px 30px;
      border-radius: 30px;
      border: none;
      background-color: #b9a89a;
      color: #fff;
      cursor: pointer;
    }

    .menu {
      padding: 60px 20px;
    }

    .menu-items {
      display: flex;
      gap: 20px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .menu-btn {
      padding: 10px 20px;
      border-radius: 20px;
      border: none;
      background-color: #fff;
      cursor: pointer;
    }

    a {
      text-decoration: none;
    }
  </style>
</head>

<body>

<header>
  <h1>Nail et moi</h1>
  <p>Your own kind of special.</p>

  <!-- BOOK NOW -->
  <a href="reservation.html">
    <button class="btn">BOOK NOW</button>
  </a>
</header>

<section class="menu">
  <h2>Ask Menu List</h2>

  <div class="menu-items">
    <a href="reservation.html?menu=foot">
      <button class="menu-btn">FOOT NAIL</button>
    </a>

    <a href="reservation.html?menu=gel">
      <button class="menu-btn">GEL NAIL</button>
    </a>

    <a href="reservation.html?menu=christmas">
      <button class="menu-btn">CHRISTMAS NAIL</button>
    </a>
  </div>
</section>

</body>
</html>

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>Reservation</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background-color: #e6ded4;
      color: #5a4a42;
    }

    .container {
      max-width: 500px;
      background-color: #fff;
      margin: 40px auto;
      padding: 24px;
      border-radius: 12px;
    }

    h1 {
      text-align: center;
      margin-bottom: 20px;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    label {
      font-size: 14px;
    }

    input, select, textarea {
      padding: 10px;
      font-size: 14px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }

    button {
      margin-top: 20px;
      padding: 12px;
      border-radius: 30px;
      border: none;
      background-color: #b9a89a;
      color: #fff;
      cursor: pointer;
    }
  </style>
</head>

<body>

<div class="container">
  <h1>Reservation</h1>

  <form>
    <!-- メニュー -->
    <div>
      <label>メニュー</label><br>
      <select id="menu" required>
        <option value="">選択してください</option>
        <option value="foot">FOOT NAIL</option>
        <option value="gel">GEL NAIL</option>
        <option value="christmas">CHRISTMAS NAIL</option>
      </select>
    </div>

    <!-- 名前 -->
    <div>
      <label>お名前</label><br>
      <input type="text" required>
    </div>

    <!-- メール -->
    <div>
      <label>メールアドレス</label><br>
      <input type="email" required>
    </div>

    <!-- 希望日 -->
    <div>
      <label>希望日</label><br>
      <input type="date" required>
    </div>

    <!-- 希望時間 -->
    <div>
      <label>希望時間</label><br>
      <input type="time" required>
    </div>

    <button type="submit">予約する</button>
  </form>
</div>

<!-- メニュー自動選択 -->
<script>
  const params = new URLSearchParams(location.search);
  const menu = params.get("menu");
  if (menu) {
    document.getElementById("menu").value = menu;
  }
</script>

</body>
</html>

