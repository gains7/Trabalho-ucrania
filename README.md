html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  
 <header>
      <nav>
        <div>
          <img src="Brasil.png" alt="" width="53px">
          <img src="ucrane.png" alt="" width="50px">
        </div>
        
        <a class="logo" href="/">Por elas</a>
        <div class="mobile-menu">
          <div class="line1"></div>
          <div class="line2"></div>
          <div class="line3"></div>
        </div>
        
        <ul class="nav-list">
          
      <li><a href="pag1.html" target="_blank">Início</a></li>

      <li><a href="pag2.html" target="_blank">Sobre</a></li>

      <li><a href="pag3.html" target="_blank">Projetos</a></li>

      <li><a href="pag4.html" target="_blank">Anfitriã</a></li>

      <li><a href="pag5.html" target="_blank">Refugiada</a></li>
      
        </ul>
      </nav>
    </header>

<h1>Quem somos:</h1>

  <li>O por elas é uma ONG(organização não governamental) que possui como objetivo dar abrigo a mulheres e crianças refugiadas ucranianas.</li>

  
<h2>Como posso comtribuir para a ONG?</h2>

  <li>Você pode contribur se tornando uma anfitriã e sedendo algum comodo de sua moradia para abrigar uma refugiada.</li>

  <script src="script.js"></script>

</body>

</html>

class MobileNavbar {
    constructor(mobileMenu, navList, navLinks) {
      this.mobileMenu = document.querySelector(mobileMenu);
      this.navList = document.querySelector(navList);
      this.navLinks = document.querySelectorAll(navLinks);
      this.activeClass = "active";
  
      this.handleClick = this.handleClick.bind(this);
    }
  
    animateLinks() {
      this.navLinks.forEach((link, index) => {
        link.style.animation
          ? (link.style.animation = "")
          : (link.style.animation = `navLinkFade 0.5s ease forwards ${
              index / 7 + 0.3
            }s`);
      });
    }
    
    handleClick() {
      this.navList.classList.toggle(this.activeClass);
      this.mobileMenu.classList.toggle(this.activeClass);
      this.animateLinks();
    }
  
    addClickEvent() {
      this.mobileMenu.addEventListener("click", this.handleClick);
    }
  
    init() {
      if (this.mobileMenu) {
        this.addClickEvent();
      }
      return this;
    }
  }
  
  const mobileNavbar = new MobileNavbar(
    ".mobile-menu",
    ".nav-list",
    ".nav-list li",
  );
  mobileNavbar.init();
  
  html, body {
  height: 100%;
  width: 100%;
}


{
  margin: 0;
  padding: 0;
}

a {
  color: #fff;
  text-decoration: none;
  transition: 0.3s;
}

a:hover {
  opacity: 0.7;
}

.logo {
  font-size: 24px;
  text-transform: uppercase;
  letter-spacing: 4px;
}

nav {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-family: system-ui, -apple-system, Helvetica, Arial, sans-serif;
  background: #23232e;
  height: 8vh;
}

main {
  background: url("bg.jpg") no-repeat center center;
  background-size: cover;
  height: 92vh;
}

.nav-list {
  list-style: none;
  display: flex;
}

.nav-list li {
  letter-spacing: 3px;
  margin-left: 32px;
}

.mobile-menu {
  display: none;
  cursor: pointer;
}

.mobile-menu div {
  width: 32px;
  height: 2px;
  background: #fff;
  margin: 8px;
  transition: 0.3s;
}

@media (max-width: 999px) {
  body {
    overflow-x: hidden;
  }
  .nav-list {
    position: absolute;
    top: 8vh;
    right: 0;
    width: 50vw;
    height: 92vh;
    background: #23232e;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    transform: translateX(100%);
    transition: transform 0.3s ease-in;
  }
  .nav-list li {
    margin-left: 0;
    opacity: 0;
  }
  .mobile-menu {
    display: block;
  }
}

.nav-list.active {
  transform: translateX(0);
}

@keyframes navLinkFade {
  from {
    opacity: 0;
    transform: translateX(50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.mobile-menu.active .line1 {
  transform: rotate(-45deg) translate(-8px, 8px);
}

.mobile-menu.active .line2 {
  opacity: 0;
}

.mobile-menu.active .line3 {
  transform: rotate(45deg) translate(-5px, -7px);
}

li {
  font-size: 18px
}

li {
  font-family: Andale Mono;
}

h1 {
  font-size: 26px
}

h1 {
  font-family: Andale Mono;
}

h2 {
  font-size: 26px
}

h2 {
  font-family: Andale Mono;
}

<h1>Em construção</h1>

<h1>Em construção</h1>

<h1>Em construção</h1>

<h1>Em construção</h1>

<h1>Em costrução</h1>

![ucrane (1)](https://user-images.githubusercontent.com/102962254/172742803-a297c832-04fc-4291-9b91-ac679b231501.png)

![Brasil (1)](https://user-images.githubusercontent.com/102962254/172742812-4e943f96-d7e5-44cc-a922-a859cb8d88db.png)
