<!DOCTYPE html><html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Urban Twins</title>
  <style>
    :root{ --bg:#000; --fg:#fff; --muted:#aaa; }
    *{ box-sizing:border-box; }
    body{
      margin:0; background:var(--bg); color:var(--fg); font-family:Arial, Helvetica, sans-serif;
    }
    header{
      padding:20px; text-align:center; border-bottom:1px solid #111;
    }
    header h1{ margin:0; letter-spacing:2px; }
    header p{ margin:6px 0 0; color:var(--muted); }
    main{ padding:20px; }
    .grid{
      display:grid; grid-template-columns:repeat(auto-fill, minmax(180px,1fr)); gap:16px;
    }
    .card{
      background:#050505; border:1px solid #111; border-radius:10px; overflow:hidden;
      transition:transform .15s ease, box-shadow .15s ease;
    }
    .card:hover{ transform:translateY(-2px); box-shadow:0 10px 30px rgba(0,0,0,.5); }
    .card img{ width:100%; height:200px; object-fit:cover; display:block; }
    .card .info{ padding:10px; text-align:center; }
    .card .info h3{ margin:0; font-size:14px; font-weight:600; }
    .card .info span{ color:var(--muted); font-size:12px; }
    footer{ text-align:center; padding:16px; color:var(--muted); border-top:1px solid #111; }
    .hint{ color:#666; font-size:12px; text-align:center; margin-top:10px; }
  </style>
</head>
<body>
  <header>
    <h1>URBAN TWINS</h1>
    <p>Catálogo oficial</p>
  </header>  <main>
    <section id="catalog" class="grid"></section>
    <div class="hint">El catálogo se carga automáticamente desde Cloudinary.</div>
  </main>  <footer>
    © <span id="year"></span> Urban Twins
  </footer>  <script>
    // ================== CONFIGURA AQUÍ ==================
    const CLOUD_NAME = 'el-urban'; // <-- pon tu cloud name
    const FOLDER = 'urban-twins'; // carpeta en Cloudinary
    // ====================================================

    const catalog = document.getElementById('catalog');
    document.getElementById('year').textContent = new Date().getFullYear();

    // Carga automática del catálogo (solo imágenes)
    async function loadCatalog(){
      try{
        const url = `https://res.cloudinary.com/${CLOUD_NAME}/image/list/${FOLDER}.json`;
        const res = await fetch(url);
        if(!res.ok) throw new Error('No se pudo cargar el catálogo');
        const data = await res.json();
        catalog.innerHTML = '';
        (data.resources || []).forEach(img => {
          const card = document.createElement('div');
          card.className = 'card';
          const imageUrl = `https://res.cloudinary.com/${CLOUD_NAME}/image/upload/${img.public_id}.${img.format}`;
          card.innerHTML = `
            <img src="${imageUrl}" alt="Urban Twins cap" />
            <div class="info">
              <h3>${img.public_id.split('/').pop()}</h3>
              <span>Urban Twins</span>
            </div>`;
          catalog.appendChild(card);
        });
      }catch(err){
        catalog.innerHTML = '<p style="color:#888">Aún no hay productos.</p>';
        console.error(err);
      }
    }

    loadCatalog();
  </script></body>
</html>
