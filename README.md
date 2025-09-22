<!doctype html>
<html lang="uz">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mevalar ro'yxati</title>
  <style>
    :root {
      --bg: linear-gradient(to right, #b7d0d7, #6184ac);
      --card: linear-gradient(to right, #b7d0d7, #6184ac, #505c81);
      --accent: #2b8aef;
      --text: #25303b;
      --muted: #6b7280;
    }
    * { box-sizing: border-box; }
    body {
      font-family: system-ui, -apple-system, "Segoe UI", Roboto, Arial;
      margin: 0; background: var(--bg); color: var(--text);
      padding: 25px;
    }
    .container {
      max-width: 1200px;margin: 36px auto;
      padding: 20px;
    }
    header {
      display: flex;
      align-items: center;
      gap: 16px;
      margin-bottom: 18px;
    }
    .logo {
      width: 56px;
      height: 56px;border-radius: 12px;
      background: linear-gradient(135deg, var(--accent), #505c81);
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-weight: 700;
      font-size: 20px;
    }
    h1 {
      font-size: 26px;
      margin: 0;
    }
    p.desc {
      color: var(--muted);
      margin: 4px 0 18px;
      font-size: 15px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
      gap: 24px;
    }
    figure.card {
      background: var(--card);
      border-radius: 16px;
      padding: 16px;
      text-align: center;
      box-shadow: 0 8px 22px rgba(20, 30, 50, 0.07);
      transition: transform .18s ease, box-shadow .18s ease;
      cursor: pointer;
    }
    figure.card:hover {
      transform: translateY(-6px);
      box-shadow: 0 14px 34px rgba(20, 30, 50, 0.1);
    }
    .img-wrap {
      width: 100%;
      aspect-ratio: 1/1;
      border-radius: 12px;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(180deg, #fff, #cbd8ec);
    }
    .img-wrap img {
      max-width: 90%;
      max-height: 90%;
      object-fit: contain;
      display: block;
    }
    figcaption {
      margin-top: 12px;
    }
    .fruit-price {
      display: inline-block;
      background-color: #ffe66d;
      padding: 2px 8px;
      border-radius: 6px;
      font-size: 14px;
      font-weight: bold;
      margin-bottom: 6px;
      color: #333;
    }
    .fruit-name {
      font-weight: 700;
      font-size: 18px;
    }
    .fruit-sub {
      font-size: 14px;
      color: var(--muted);
      margin-top: 6px;
    }
    @media (max-width: 420px) {
      .container { padding: 12px; }
      h1 { font-size: 20px; }
    }

    /* Modal uslubi */
    #modal {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0, 0, 0, 0.5);
      z-index: 1000;
      align-items: center;
      justify-content: center;
    }
    #modal-content {
      background: white;
      border-radius: 12px;
      padding: 24px;
      max-width: 400px;
      width: 90%;
      position: relative;
      box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
    }
    #modal-content h2 {
      margin-top: 0;
    }
    #modal-content button {
      position: absolute;
      top: 12px;
      right: 12px;
      background: none;
      border: none;
      font-size: 20px;
      cursor: pointer;
    }
    .title {
      color: #5C6AC4;
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">M</div>
      <div>
        <h1>Mevalar ro'yxati</h1>
        <p class="desc">Mevalar: olma, banan, anor, behi, nok</p>
      </div>
    </header>

    <main>
      <section class="grid">
        

        <figure class="card">
          <div class="img-wrap">
            <img src="https://cdn.shopify.com/s/files/1/0062/8532/8445/products/Honeycrisp_Apple_1_BB.jpg?v=1589550267" alt="Olma">
            </div>
          <figcaption>
            <div class="fruit-price">Narxi: 12 000 so'm/kg</div>
            <div class="fruit-name">Olma</div>
            <div class="fruit-sub">Vitaminlarga boy</div>
          </figcaption>
        </figure>

        <figure class="card">
          <div class="img-wrap">
            <img src="https://5.imimg.com/data5/SELLER/Default/2022/12/EK/NP/CN/49293026/fresh-banana-fruit.webp" alt="Banan">
          </div>
          <figcaption>
            <div class="fruit-price">Narxi: 18 000 so'm/kg</div>
            <div class="fruit-name">Banan</div>
            <div class="fruit-sub">Energiya beruvchi</div>
          </figcaption>
        </figure>

        <figure class="card">
          <div class="img-wrap">
            <img src="https://m.media-amazon.com/images/I/61ff6bI+F4L._SL1000_.jpg" alt="Anor">
          </div>
          <figcaption>
            <div class="fruit-price">Narxi: 25 000 so'm/kg</div>
            <div class="fruit-name">Anor</div>
            <div class="fruit-sub">Sog'lom va shirin</div>
          </figcaption>
        </figure>

        <figure class="card">
          <div class="img-wrap">
            <img src="https://www.suttons.co.uk/product_images/QUIN_VRANJA_L231481.jpg" alt="Behi">
          </div>
          <figcaption>
            <div class="fruit-price">Narxi: 15 000 so'm/kg</div>
            <div class="fruit-name">Behi</div>
            <div class="fruit-sub">Xushbo'y va foydali</div>
          </figcaption>
        </figure>

        <figure class="card">
          <div class="img-wrap">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR2Fxpjv-r34wjeNAKWijfkCSsY3GsRLucBdQ&s" alt="Nok">
          </div>
          <figcaption>
            <div class="fruit-price">Narxi: 14 000 so'm/kg</div>
            <div class="fruit-name">Nok</div>
            <div class="fruit-sub">Sharbatli va mayin</div>
          </figcaption>
        </figure>

      </section>
    </main>

    <footer style="margin-top:22px; text-align:center; color:var(--muted); font-size:13px">
      <div>Dastur Dilrozbegim tomonidan qilingan .</div>
      <div id="currentTime" style="margin-top:8px;"></div>
    </footer>
  </div>

  <!-- Modal Oynasi -->
  <div id="modal">
    <div id="modal-content">
      <button onclick="closeModal()">&times;</button>
      <h2 id="modal-title"></h2>
      <p id="modal-price" class="fruit-price"></p>
      <p id="modal-vitamin"></p>
      <p id="modal-benefit"></p>
    </div>
  </div>

  <script>
    const fruits = {
      "Olma": {
        vitamin: "Vitamin C, K, B6",
        benefit: "Immunitetni mustahkamlaydi, yurak faoliyatini yaxshilaydi",
        price: "12 000 so'm/kg"
      },
      "Banan": {
        vitamin: "Vitamin B6, C, magniy, kaliy",
        benefit: "Energiya beradi, ichak faoliyatini yaxshilaydi",
        price: "18 000 so'm/kg"
      },
      "Anor": {
        vitamin: "Vitamin C, K, B9",
        benefit: "Qon bosimini tushiradi, yurak uchun foydali",
        price: "25 000 so'm/kg"
      },
      "Behi": {
        vitamin: "Vitamin C, E, K",
        benefit: "Nafas yo‘llarini tozalaydi, hazmni yaxshilaydi",
        price: "15 000 so'm/kg"
      },
      "Nok": {
        vitamin: "Vitamin C, K, mis",
        benefit: "Teri salomatligini saqlaydi, suyaklarni mustahkamlaydi",
        price: "14 000 so'm/kg"
      }
    };

    document.querySelectorAll(".card").forEach(card => {
      const name = card.querySelector(".fruit-name").textContent;
      card.addEventListener("click", () => openModal(name));
    });
    

    function openModal(name) {
      const data = fruits[name];
      if (!data) return;
      document.getElementById("modal-title").textContent = name;
      document.getElementById("modal-price").textContent = `Narxi: ${data.price}`;
      document.getElementById("modal-vitamin").textContent = `Vitaminlar: ${data.vitamin}`;
      document.getElementById("modal-benefit").textContent = `Foydasi: ${data.benefit}`;
      document.getElementById("modal").style.display = "flex";
    }
    function closeModal() {
      document.getElementById("modal").style.display = "none";
    }

    function showTime() {
      document.getElementById('currentTime').innerHTML = new Date().toUTCString();
    }
    showTime();
    setInterval(showTime, 1000);
  </script>
</body>
</html>
