# RESTAURANT-MENU
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <link rel="stylesheet" href="menu.css" />
  <title>NEWS WEBSITE</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body class="background">

 <!-- Splash Screen with Logo -->
<div class="logo">
  <img src="https://static.vecteezy.com/system/resources/previews/007/923/910/original/master-chef-logo-design-template-free-vector.jpg" alt="Chef Food Logo" /><P><span><h1>THE CHEF`S KITCHEN</h1></P></span>

</div>


  <!-- Scrolling Menu -->
  <div class="menu" id="menu">

    <h1 class="menu-title">Our Menu</h1>

    <div class="section">
      <h2>Starters</h2>
      <div class="scroll-frame">
        <div class="food-row">
          <div class="food-card"><img src="https://www.cookforindia.com/wp-content/uploads/2016/08/Paneer-Tikka-_LR.jpg" alt=""><p>Paneer Tikka<br><span>₹180</span></p></div>
          <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.tF4CoVoYtb8Je1QNsF79qwHaFC&pid=Api&P=0&h=180" alt=""><p>Veg Spring Roll<br><span>₹150</span></p></div>
          <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.vi4fm7X8wyKLld1X4GLpZQHaFU&pid=Api&P=0&h=180" alt=""><p>Sandwich<br><span>₹200</span></p></div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Main Course</h2>
      <div class="scroll-frame">
        <div class="food-row">
          <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.cMa0VSkJUlyY8gvV3xc-ywHaEK&pid=Api&P=0&h=180" alt=""><p>Butter Naan<br><span>₹25</span></p></div>
          <div class="food-card"><img src="https://www.cubesnjuliennes.com/wp-content/uploads/2019/03/Easy-Butter-Paneer-Masala-Recipe.jpg" alt=""><p>Paneer Butter Masala<br><span>₹220</span></p></div>
          <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.om4sBr-Pvd15TzXGl4QyfAHaFj&pid=Api&P=0&h=180" alt=""><p>Dal Tadka<br><span>₹160</span></p></div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Beverages</h2>
      <div class="scroll-frame">
        <div class="food-row">
          <div class="food-card"><img src="https://www.cookwithmanali.com/wp-content/uploads/2021/06/Lassi-Recipe-676x1024.jpg" alt=""><p>Lassi<br><span>₹60</span></p></div>
          <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.eJlL1bD_3COtRZisaPXgqwHaLO&pid=Api&P=0&h=180" alt=""><p>Cold Coffee<br><span>₹80</span></p></div>
          <div class="food-card"><img src="https://tse1.mm.bing.net/th?id=OIP.HZzHIkCuIUPt0VGeXJIJuAHaLH&pid=Api&P=0&h=180" alt=""><p>Mojito<br><span>₹90</span></p></div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Desserts</h2>
      <div class="scroll-frame">
        <div class="food-row">
          <div class="food-card"><img src="https://bakewithzoha.com/wp-content/uploads/2023/04/gulab-jamun-3-scaled.jpg" alt=""><p>Gulab Jamun<br><span>₹70</span></p></div>
          <div class="food-card"><img src="https://tse1.mm.bing.net/th?id=OIP.zyQfOPY2223yuX3bx2kc6AHaE7&pid=Api&P=0&h=180" alt=""><p>Ice Cream<br><span>₹100</span></p></div>
          <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.AJm0Zndzj24rzNJw32cKxQHaFN&pid=Api&P=0&h=180" alt=""><p>Rasgulla<br><span>₹60</span></p></div>
        </div>
      </div>
    </div>

  </div>

  <script>
    setTimeout(() => {
      document.querySelector('.menu').style.display = 'block';
    }, 3500);
  </script>






</body>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body.background {
  background: black;
  color: white;
  overflow-x: hidden;
}

/* Splash Logo */
.logo {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: black;
  animation: fadeOut 2s ease-in-out 3s forwards;
}

.logo img {
  width: 180px;
  height: auto;
  border-radius: 45%;
  animation: pop 1.5s ease-in-out;
  filter: drop-shadow(0 0 15px #ffcc00);
}

@keyframes pop {
  0% {
    transform: scale(0.2);
    opacity: 0;
  }
  100% {
    transform: scale(1);
    opacity: 1;
  }
}

@keyframes fadeOut {
  to {
    opacity: 0;
    visibility: hidden;
    position: absolute;
  }
}

/* Menu Container */
.menu {
  padding: 2rem 1rem;
  display: none;
}

.menu-title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 2rem;
  color: #ffcc00;
  text-shadow: 0 0 10px #fff700a6;
}

.section {
  margin-bottom: 2rem;
}

.section h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #ffbb00;
  text-shadow: 0 0 8px #ff8c00;
  border-bottom: 2px solid #ffcc00;
  padding-bottom: 0.5rem;
}

/* Horizontal Scroll Frame */
.scroll-frame {
  display: flex;
  justify-content: center;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  padding-bottom: 10px;
}

.food-row {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1rem;
  padding: 1rem 0;
  flex-wrap: nowrap;
  scroll-snap-type: x mandatory;
}

.food-card {
  background: #1c1c1c;
  border-radius: 15px;
  width: 180px;
  min-width: 180px;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 0 15px #ffcc00a2;
  transition: transform 0.3s;
  flex-shrink: 0;
  scroll-snap-align: center;
}

.food-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
  border-radius: 10px;
}

.food-card p {
  margin-top: 0.5rem;
  font-size: 1rem;
}

.food-card span {
  display: block;
  color: #ffcc00;
  font-weight: bold;
  font-size: 1.1rem;
}

.food-card:hover {
  transform: scale(1.05);
}

/* Scrollbar Styling */
.scroll-frame::-webkit-scrollbar {
  height: 6px;
}
.scroll-frame::-webkit-scrollbar-thumb {
  background-color: #ffcc00;
  border-radius: 5px;
}

/* ------------------- */
/* Responsive Changes  */
/* ------------------- */

@media (max-width: 600px) {
  .menu-title {
    font-size: 1.8rem;
  }

  .section h2 {
    font-size: 1.3rem;
  }

  .food-card {
    width: 150px;
    min-width: 150px;
  }

  .food-card img {
    height: 100px;
  }

  .food-card p {
    font-size: 0.9rem;
  }

  .food-card span {
    font-size: 1rem;
  }

  .splash img {
    width: 140px;
  }
  .logo {
  height:110vh;
  display: flex;
  margin-left: 50px;
  border-radius: 45px;
  align-items: center;
  justify-content: center;
  background-color: black;
  animation: fadeOut 2s ease-in-out 3s forwards;
}
}
