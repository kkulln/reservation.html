# index.html

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
      padding: 12px 32px;
      border-radius: 30px;
      border: none;
      background-color: #b9a89a;
      color: #fff;
      cursor: pointer;
    }

    .menu {
      padding: 60px 20px;
    }

    .menu-list {
      display: flex;
      gap: 20px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .menu-btn {
      padding: 10px 22px;
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

  <!-- トップ（スクリーンショットの画面） -->
  <header>
    <h1>Nail et moi</h1>
    <p>Your own kind of special.</p>

    <!-- BOOK NOW → 予約画面へ -->
    <a href="reservation.html">
      <button class="btn">BOOK NOW</button>
    </a>
  </header>

  <!-- メニュー -->
  <section class="menu">
    <h2>Ask Menu List</h2>

    <div class="menu-list">
      <a href="reservation.html?menu=foot">
        <button class="menu-btn">FOOT NAIL</button>
      </a>

      <a href="reservation.html?menu=gel">
        <button class="menu-btn">GEL NAIL</butto
      </a>

      <a href="reservation.html?menu=christmas">
        <button class="menu-btn">CHRISTMAS NAIL</button>
      </a>
    </div>
  </section>

</body>
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
      max-width: 480px;
      background-color: #fff;
      margin: 40px auto;
      padding: 24px;
      border-radius: 12px;
    }
    h1 {
      text-align: center;
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    input, select {
      padding: 10px;
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
    <label>メニュー</label>
    <select id="menu" required>
      <option value="">選択してください</option>
      <option value="foot">FOOT NAIL</option>
      <option value="gel">GEL NAIL</option>
      <option value="christmas">CHRISTMAS NAIL</option>
    </select>

    <label>お名前</label>
    <input type="text" required>

    <label>メールアドレス</label>
    <input type="email" required>

    <label>希望日</label>
    <input type="date" required>

    <label>希望時間</label>
    <input type="time" required>

    <button type="submit">予約する</button＞

<script>
  const params = new URLSearchParams(location.search);
  const menu = params.get("menu");
  if (menu) {
    document.getElementById("menu").value = menu;
  }
</script>

</body>
</html>

