<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <link rel="stylesheet" href="menu.css" />
  <title>THE CHEF'S KITCHEN</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body class="background">

<!-- Splash Screen with Logo -->
<div class="splash">
  <img src="https://static.vecteezy.com/system/resources/previews/007/923/910/original/master-chef-logo-design-template-free-vector.jpg" alt="Chef Food Logo" />
  <h1>THE CHEF’S KITCHEN</h1>
</div>

<!-- Scrolling Menu -->
<div class="menu" id="menu">
  <h1 class="menu-title">Our Menu</h1>

  <!-- Starters -->
  <div class="section">
    <h2>Starters</h2>
    <div class="scroll-frame">
      <div class="food-row">
        <div class="food-card"><img src="https://www.cookforindia.com/wp-content/uploads/2016/08/Paneer-Tikka-_LR.jpg"><p>Paneer Tikka<br><span>₹180</span></p></div>
        <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.tF4CoVoYtb8Je1QNsF79qwHaFC"><p>Veg Spring Roll<br><span>₹150</span></p></div>
        <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.vi4fm7X8wyKLld1X4GLpZQHaFU"><p>Sandwich<br><span>₹200</span></p></div>
      </div>
    </div>
  </div>

  <!-- Main Course -->
  <div class="section">
    <h2>Main Course</h2>
    <div class="scroll-frame">
      <div class="food-row">
        <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.cMa0VSkJUlyY8gvV3xc-ywHaEK"><p>Butter Naan<br><span>₹25</span></p></div>
        <div class="food-card"><img src="https://www.cubesnjuliennes.com/wp-content/uploads/2019/03/Easy-Butter-Paneer-Masala-Recipe.jpg"><p>Paneer Butter Masala<br><span>₹220</span></p></div>
        <div class="food-card"><img src="https://tse2.mm.bing.net/th?id=OIP.om4sBr-Pvd15TzXGl4QyfAHaFj"><p>Dal Tadka<br><span>₹160</span></p></div>
      </div>
    </div>
  </div>

  <!-- Beverages -->
  <div class="section">
    <h2>Beverages</h2>
    <div class="scroll-frame">
      <div class="food-row">
        <div class="food-card"><img src="https://www.cookwithmanali.com/wp-content/uploads/2021/06/Lassi-Recipe-676x1024.jpg"><p>Lassi<br><span>₹60</span></p></div>
        <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.eJlL1bD_3COtRZisaPXgqwHaLO"><p>Cold Coffee<br><span>₹80</span></p></div>
        <div class="food-card"><img src="https://tse1.mm.bing.net/th?id=OIP.HZzHIkCuIUPt0VGeXJIJuAHaLH"><p>Mojito<br><span>₹90</span></p></div>
      </div>
    </div>
  </div>

  <!-- Desserts -->
  <div class="section">
    <h2>Desserts</h2>
    <div class="scroll-frame">
      <div class="food-row">
        <div class="food-card"><img src="https://bakewithzoha.com/wp-content/uploads/2023/04/gulab-jamun-3-scaled.jpg"><p>Gulab Jamun<br><span>₹70</span></p></div>
        <div class="food-card"><img src="https://tse1.mm.bing.net/th?id=OIP.zyQfOPY2223yuX3bx2kc6AHaE7"><p>Ice Cream<br><span>₹100</span></p></div>
        <div class="food-card"><img src="https://tse3.mm.bing.net/th?id=OIP.AJm0Zndzj24rzNJw32cKxQHaFN"><p>Rasgulla<br><span>₹60</span></p></div>
      </div>
    </div>
  </div>
</div>

<!-- Splash Screen Delay -->
<script>
  setTimeout(() => {
    document.querySelector('.menu').style.display = 'block';
  }, 3000);
</script>

</body>
</html>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: #000814;
  color: white;
}

.splash {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #001d3d;
  text-align: center;
}

.splash img {
  width: 180px;
  height: auto;
  border-radius: 50%;
  margin-bottom: 10px;
}

.splash h1 {
  font-size: 2em;
  color: #ffc300;
}

.menu {
  display: none;
  padding: 20px;
}

.menu-title {
  text-align: center;
  color: #ffc300;
  font-size: 2rem;
  margin-bottom: 20px;
}

.section {
  margin-bottom: 30px;
}

.section h2 {
  text-align: center;
  color: #ffd60a;
  margin-bottom: 10px;
}

.scroll-frame {
  overflow-x: auto;
}

.food-row {
  display: flex;
  gap: 15px;
  justify-content: center;
  flex-wrap: wrap;
}

.food-card {
  background-color: #003566;
  border-radius: 10px;
  padding: 10px;
  width: 180px;
  text-align: center;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
  transition: transform 0.3s;
}

.food-card:hover {
  transform: scale(1.05);
}

.food-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
  border-radius: 6px;
}

.food-card p {
  margin: 10px 0 0;
  font-size: 1rem;
}

.food-card span {
  color: #ffd60a;
  font-weight: bold;
}
