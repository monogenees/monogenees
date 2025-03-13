
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>美容師 [小松 亮介]</title>
  <style>
    body {
      background-color: #F7F1E1; /* 柔らかいベージュ背景 */
      margin: 0;
      font-family: 'Helvetica Neue', Arial, sans-serif;
      color: #333;
      position: relative;
      overflow: hidden;
    }
    /* スプラッシュ画面：テント＋名前 */
    #splash {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background-color: #F7F1E1;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      z-index: 10;
      animation: fadeOut 1s ease forwards;
      animation-delay: 2s; /* 2秒後にフェードアウト開始 */
    }
    .splash-img {
      width: 120px; /* テント画像の大きさ */
      margin-bottom: 20px;
    }
    .splash-name {
      font-size: 48px;
      font-weight: bold;
    }

    /* メインコンテンツは初め非表示（opacity:0） */
    #main-content {
      /* スプラッシュが消えたあと表示開始 */
      position: relative;
      opacity: 0;
      animation: fadeIn 1s ease forwards;
      animation-delay: 3s; /* 3秒後に全体がフェードイン */
      padding: 20px;
      text-align: center;
    }

    .profile {
      margin-bottom: 40px;
    }
    .profile-img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #333;
      margin: 20px auto;
      display: block;
    }

    /* 名前・LINE・インスタを順番に表示 */
    .my-name,
    .line-link,
    .insta-link {
      opacity: 0;
      animation: fadeInItem 1s ease forwards;
    }
    .my-name {
      font-size: 36px;
      margin: 10px 0;
      animation-delay: 3.5s; /* 名前は3.5秒後 */
    }
    .line-link {
      font-size: 20px;
      margin-top: 20px;
      display: inline-block;
      text-decoration: none;
      color: #333;
      border-bottom: 1px solid transparent;
      transition: border-bottom 0.3s;
      animation-delay: 4.5s; /* LINEは4.5秒後 */
    }
    .line-link:hover {
      border-bottom: 1px solid #333;
    }
    .insta-link {
      font-size: 20px;
      margin-top: 20px;
      display: inline-block;
      text-decoration: none;
      color: #333;
      border-bottom: 1px solid transparent;
      transition: border-bottom 0.3s;
      animation-delay: 5.5s; /* Instagramは5.5秒後 */
    }
    .insta-link:hover {
      border-bottom: 1px solid #333;
    }

    /* お店情報はさらに遅れて表示 (下からふわっと) */
    .shop-info {
      margin-top: 40px;
      opacity: 0;
      animation: fadeInUp 1s ease forwards;
      animation-delay: 6.5s; /* 6.5秒後に表示 */
    }
    .shop-info h2 {
      font-size: 28px;
      margin: 10px 0;
    }
    .shop-info p {
      font-size: 20px;
      margin: 5px 0;
    }

    /* アニメーション定義 */
    @keyframes fadeOut {
      from { opacity: 1; }
      to { opacity: 0; }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes fadeInItem {
      from {
        opacity: 0;
        transform: translateY(10px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>
  <!-- スプラッシュ画面：最初にテントのイラスト＋名前 -->
  <div id="splash">
    <img class="splash-img" src="[HASAMI47](https://github.com/user-attachments/assets/ea2bc66d-9083-43f6-b47b-74101a5c910f)
E_URL" alt="テントのイラスト">
    <div class="splash-name">小松 亮介</div>
  </div>

  <!-- メインコンテンツ -->
  <div id="main-content">
    <!-- プロフィール部分 -->
    <div class="profile">
      <img class="profile-img" src="あなたの写真のURL" alt="プロフィール写真">
      <!-- 名前・SNSを順番に表示 -->
      <div class="my-name">小松 亮介</div><br/>
      <a class="line-link" href="https://line.me/ti/p/komaryou0205" target="_blank">LINE</a><br/>
      <a class="insta-link" href="https://www.instagram.com/monogenees/" target="_blank">Instagram</a>
    </div>
    <!-- 店舗情報 -->
    <div class="shop-info">
      <h2>レアヘアー (RareHair)</h2>
      <p>〒305-0074</p>
      <p>茨城県つくば市 高野台2丁目9-5 サザンクロス</p>
    </div>
  </div>
</body>
</html>
