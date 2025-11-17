<!DOCTYPE html><html lang="fr">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>MoDDinG_CSR</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: #000;
            font-family: Arial, sans-serif;
            color: white;
            overflow-x: hidden;
        }.container {
        display: flex;
        width: 100vw;
        height: 100vh;
    }

    /* LEFT SIDE IMAGE */
    .left {
        width: 50%;
        height: 100%;
        background: url('IMAGE_LINK_HERE') center/cover no-repeat;
        filter: brightness(0.9);
    }

    /* RIGHT MENU */
    .right {
        width: 50%;
        background: #0d0d0d;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 35px;
        padding: 20px;
    }

    h1 {
        font-size: 38px;
        text-transform: uppercase;
        letter-spacing: 3px;
        text-shadow: 0 0 12px white;
    }

    .btn {
        width: 75%;
        padding: 18px;
        text-align: center;
        border-radius: 10px;
        font-size: 24px;
        font-weight: bold;
        cursor: pointer;
        transition: 0.25s;
    }

    .ps4 {
        background: #ffc800;
        color: #000;
    }
    .ps4:hover { box-shadow: 0 0 20px #ffc800; }

    .hfw {
        background: #00e5ff;
        color: #000;
    }
    .hfw:hover { box-shadow: 0 0 20px #00e5ff; }

    .cfw {
        background: #ff0000;
        color: #000;
    }
    .cfw:hover { box-shadow: 0 0 20px #ff0000; }

    @media(max-width: 800px) {
        .container {
            flex-direction: column;
        }
        .left, .right {
            width: 100%;
            height: 50vh;
        }
    }

</style>

</head>
<body><div class
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Modding PS3/PS4</title>

<style>
body {
  margin: 0;
  font-family: Arial;
  background: #000;
  color: #fff;
}

/* TOP BAR */
.topbar {
  background: #6a00ff;
  padding: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 20px;
}

.menu-btn {
  font-size: 30px;
  cursor: pointer;
}

/* MENU */
.menu {
  position: fixed;
  top: 0;
  left: -100%;
  width: 70%;
  height: 100vh;
  background: #fff;
  padding: 30px 20px;
  transition: 0.3s;
  color: black;
  z-index: 1000;
}

.menu.open {
  left: 0;
}

.menu a {
  display: block;
  padding: 15px 0;
  text-decoration: none;
  font-size: 22px;
  color: black;
}

/* TITRES CATÉGORIES */
.category {
  margin: 50px 20px 20px 20px;
  font-size: 28px;
  font-weight: bold;
}

.card {
  background: #111;
  margin: 10px 20px;
  padding: 20px;
  border-radius: 10px;
  border: 1px solid #444;
}
.card h3 {
  margin: 0;
  font-size: 22px;
}
</style>

</head>
<body>

<div class="topbar">
  <div>Modding PS3 / PS4</div>
  <div class="menu-btn" onclick="openMenu()">☰</div>
</div>

<!-- MENU LATERAL -->
<div id="sideMenu" class="menu">
  <a href="#">CFW</a>
  <a href="#">HEN</a>
  <a href="#">HFW</a>
  <a href="#">MOD MENUS</a>
  <a href="#">RTM TOOLS</a>
  <a href="#">JEUX / PKG</a>
  <a href="#">UNBAN</a>
  <a href="#">TUTORIELS</a>
  <a href="#" onclick="closeMenu()">Fermer</a>
</div>

<!-- CONTENU PRINCIPAL -->
<div class="category">📦 CFW</div>
<div class="card"><h3>CFW 4.90 Evilnat</h3></div>
<div class="card"><h3>CFW Rebug</h3></div>

<div class="category">🟡 HEN</div>
<div class="card"><h3>HEN 4.90</h3></div>

<div class="category">🔵 HFW</div>
<div class="card"><h3>HFW 4.90</h3></div>

<script>
function openMenu() {
  document.getElementById("sideMenu").classList.add("open");
}
function closeMenu() {
  document.getElementById("sideMenu").classList.remove("open");
}
</script>

</body>
</html>
<body> 
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Site de modding PS3/PS4</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Style général */
    html, body { margin: 0; padding: 0; background: #000; color: #0F0; font-family: Arial, sans-serif; }
    h2, h3 { cursor: pointer; }
    a { color: #0F0; text-decoration: none; }
    a:hover { text-decoration: underline; }
    /* Canvas Matrix */
    #matrixCanvas { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; }
    /* Sections */
    .section { padding: 20px; }
    .mods { display: none; margin-top: 10px; }
    .mod { background: rgba(0, 0, 0, 0.7); border: 1px solid #0F0; border-radius: 5px; padding: 10px; margin-bottom: 10px; }
    /* Boutons */
    button.cat-btn { background: transparent; border: 1px solid #0F0; color: #0F0; padding: 10px 15px; border-radius: 4px; cursor: pointer; }
    button.cat-btn:hover { background: #0F0; color: #000; }
  </style>
</head>
<body>

  <!-- Canvas pour l'effet Matrix -->
  <canvas id="matrixCanvas"></canvas>

  <!-- Liste des catégories -->
  <div class="section">
    <h2>Catégories de jeux</h2>
    <button class="cat-btn" data-cat="bo2">Black Ops 2</button>
    <button class="cat-btn" data-cat="mw3">Modern Warfare 3</button>
  </div>

  <!-- Section des mods pour Black Ops 2 -->
  <div class="section mods" id="mods-bo2">
    <h3>Mods Black Ops 2</h3>
    <div class="mod">
      <h4>Mod Extra Armes</h4>
      <p>Ajoute de nouvelles armes au jeu.</p>
      <a href="https://raw.githubusercontent.com/monutilisateur/monrepo/main/bo2/extra-armes.zip" download>Télécharger</a>
    </div>
    <div class="mod">
      <h4>Script XP Infini</h4>
      <p>Augmente votre XP jusqu\'à l\'infini.</p>
      <a href="https://raw.githubusercontent.com/monutilisateur/monrepo/main/bo2/xp-infini.zip" download>Télécharger</a>
    </div>
  </div>

  <!-- Section des mods pour MW3 -->
  <div class="section mods" id="mods-mw3">
    <h3>Mods Modern Warfare 3</h3>
    <div class="mod">
      <h4>Outils CoDPoint</h4>
      <p>Permet de modifier vos points CoD.</p>
      <a href="https://raw.githubusercontent.com/monutilisateur/monrepo/main/mw3/codpoint-tool.zip" download>Télécharger</a>
    </div>
  
