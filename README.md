# reservation.

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>Reservation | Nail et moi</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- ===== CSSはこの中にまとめる ===== -->
  <style>
    /* 全体のリセット（余白を整える） */
    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background-color: #e6ded4; /* ベージュ系背景 */
      color: #5a4a42;
    }

    /* ページ全体の中央寄せ */
    .container {
      max-width: 500px;
      margin: 40px auto;
      background-color: #fff;
      padding: 24px;
      border-radius: 12px;
    }

    /* タイトル */
    h1 {
      text-align: center;
      font-size: 24px;
      margin-bottom: 8px;
    }

    /* 説明文 */
    .description {
      text-align: center;
      font-size: 14px;
      margin-bottom: 24px;
    }

    /* フォーム全体 */
    form {
      display: flex;
      flex-direction: column;
      gap: 16px; /* 入力欄の間隔 */
    }

    /* ラベル */
    label {
      font-size: 14px;
      margin-bottom: 4px;
    }

    /* 入力欄共通 */
    input,
    textarea {
      padding: 10px;
      font-size: 14px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    /* テキストエリアの高さ */
    textarea {
      resize: vertical;
      min-height: 80px;
    }

    /* 送信ボタン */
    button {
      margin-top: 16px;
      padding: 12px;
      font-size: 14px;
      background-color: #b9a89a;
      color: #fff;
      border: none;
      border-radius: 20px;
      cursor: pointer;
    }

    /* ボタンにマウスを乗せたとき */
    button:hover {
      opacity: 0.8;
    }

    /* スマホ用（画面が小さい時） */
    @media screen and (max-width: 480px) {
      .container {
        margin: 20px;
        padding: 20px;
      }

      h1 {
        font-size: 20px;
      }
    }
  </style>
</head>

<body>

  <div class="container">
    <h1>Reservation</h1>
    <p class="description">
      ご希望の日時を入力してください
    </p>

    <!-- ===== 予約フォーム ===== -->
    <form>
      <!-- 名前 -->
      <div>
        <label for="name">お名前</label><br>
        <input type="text" id="name" name="name" placeholder="例）山田 花子" required>
      </div>

      <!-- メール -->
      <div>
        <label for="email">メールアドレス</label><br>
        <input type="email" id="email" name="email" placeholder="example@mail.com" required>
      </div>

      <!-- 電話番号 -->
      <div>
        <label for="tel">電話番号</label><br>
        <input type="tel" id="tel" name="tel" placeholder="090-0000-0000">
      </div>

      <!-- 希望日 -->
      <div>
        <label for="date">希望日</label><br>
        <input type="date" id="date" name="date" required>
      </div>

      <!-- 希望時間 -->
      <div>
        <label for="time">希望時間</label><br>
        <input type="time" id="time" name="time" required>
      </div>

      <!-- メッセージ -->
      <div>
        <label for="message">ご要望・メッセージ（任意）</label><br>
        <textarea id="message" name="message" placeholder="デザインの希望など"></textarea>
      </div>

      <!-- 送信ボタン -->
      <button type="submit">予約する</button>
    </form>
  </div>

</body>
</html>

<!-- BOOK NOW をクリックすると reservation.html に移動 -->
<a href="reservation.html" class="btn-link">
  <button class="btn">BOOK NOW</button>
</a>

<!-- FOOT NAIL -->
<a href="reservation.html" class="btn-link">
  <button class="menu-btn">FOOT NAIL</button>
</a>

<!-- GEL NAIL -->
<a href="reservation.html" class="btn-link">
  <button class="menu-btn">GEL NAIL</button>
</a>

<!-- CHRISTMAS NAIL -->
<a href="reservation.html" class="btn-link">
  <button class="menu-btn">CHRISTMAS NAIL</button>
</a>

