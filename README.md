# Hymd-obud-shop.mn
<!mash hymd obud html>
<html lang="mn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rims Mongolian Shop</title>

<style>
*{
  box-sizing:border-box;
}

body{
  margin:0;
  padding:15px;
  background:#0f0f0f;
  color:white;
  font-family:-apple-system,BlinkMacSystemFont,Arial,sans-serif;
}

/* ===== TITLE ===== */
h1{
  text-align:center;
  margin-bottom:15px;
  font-size:22px;
}

/* ===== GRID ===== */
.grid{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:12px;
}

/* ===== CARD ===== */
.card{
  background:#1c1c1c;
  border-radius:14px;
  padding:10px;
  text-align:center;
  box-shadow:0 5px 15px rgba(0,0,0,0.4);
}

/* ===== IMAGE ===== */
.card img{
  width:100%;
  height:140px;
  object-fit:cover;
  border-radius:10px;
}

/* ===== TEXT ===== */
.name{
  margin-top:8px;
  font-weight:bold;
  font-size:14px;
}

.price{
  color:#00ff99;
  margin:6px 0;
  font-size:15px;
}

/* ===== BUTTON ===== */
button{
  background:#ff2e2e;
  border:none;
  padding:8px 16px;
  border-radius:20px;
  color:white;
  cursor:pointer;
  font-size:14px;
  transition:0.2s;
}

button:hover{
  background:#ff4a4a;
}

button:active{
  transform:scale(0.95);
}
</style>
</head>

<body>

<h1>🔥 Sport Машины Обуд</h1>

<div class="grid" id="grid"></div>

<script>
const products = [
"BBS RS Sport","BBS LM Racing","RAYS Volk TE37","Gram Lights 57DR",
"OZ Ultraleggera","OZ Superturismo","Enkei RPF1","Enkei NT03",
"Work Emotion CR Kai","Work Meister S1","SSR GTX01","SSR Professor",
"HRE FF10","HRE P101","Rotiform BLQ","Rotiform RSE",
"ADVAN Racing GT","ADVAN RG-D2","Konig Hypergram","Konig Dekagram"
];

// GitHub Pages safe images
const images = [
"https://source.unsplash.com/400x300/?car,wheel",
"https://source.unsplash.com/400x300/?rims",
"https://source.unsplash.com/400x300/?sportcar,wheel",
"https://source.unsplash.com/400x300/?alloy,wheels",
"https://source.unsplash.com/400x300/?racing,wheel",
"https://source.unsplash.com/400x300/?tuning,car",
"https://source.unsplash.com/400x300/?drift,car",
"https://source.unsplash.com/400x300/?jdm,wheels",
"https://source.unsplash.com/400x300/?supercar,wheels",
"https://source.unsplash.com/400x300/?stance,car",
"https://source.unsplash.com/400x300/?wheel,closeup",
"https://source.unsplash.com/400x300/?automotive,wheel",
"https://source.unsplash.com/400x300/?rims,detail",
"https://source.unsplash.com/400x300/?car,mod",
"https://source.unsplash.com/400x300/?performance,wheel",
"https://source.unsplash.com/400x300/?luxury,wheels",
"https://source.unsplash.com/400x300/?trackcar,wheel",
"https://source.unsplash.com/400x300/?wheel,design",
"https://source.unsplash.com/400x300/?tire,wheel",
"https://source.unsplash.com/400x300/?motorsport,wheel"
];

const grid = document.getElementById("grid");

products.forEach((item,index)=>{

  const card = document.createElement("div");
  card.className = "card";

  card.innerHTML = `
    <img loading="lazy" src="${images[index]}" alt="${item}">
    <div class="name">${item}</div>
    <div class="price">1,000₮</div>
    <button onclick="buy('${item}')">Авах</button>
  `;

  grid.appendChild(card);
});

function buy(name){
  alert("🚗💨 " + name + "\n\nОдоогоор demo shop байна 😎");
}
</script>

</body>
</html>
