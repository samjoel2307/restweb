# Ex.07 Restaurant Website
## Date:08-10-2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
rest.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Website</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Open+Sans&family=Poppins&family=Playfair+Display&family=Roboto+Mono&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <nav class="controller">
            <ul id="navbar">
                <h2 id="head">HAPPY FEAST
                </h2>
                <li><a href="#home" onclick="why()">Home</a></li>
                <li><a href="admin.html">Administration</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>
          <img src="https://sulaindianrestaurant.com/wp-content/uploads/2024/07/Indian-food-near-me-by-sula-indian-restaurant-serving-vancouver-with-locations-on-commercial-drive-main-street-davie-street-1200x799.jpg" alt="Signature Dish" class = "menu-item">

    <div class="content-type">
        <h1>Best Quality <br> Food</h1><br>
        <p><strong>we serve up a delicious mix of South Indian classics, fast food favorites,
            <br> juicy burgers, and refreshing beverages — all crafted with love and premium ingredients.
</strong></p>
    </div>
    <footer id="footer">
        <h1>&copy;</h1><h4>SAM JOEL JOSHUA(25001200)</h4>
    </footer>
</body>


</html>
<script>
    function why(){
        alert("You are already on the home page")
    }
</script>

style.css

* {
    padding: 0px;
    margin: 0px;
    accent-color: #FFD700;
}

body {
    background-color:#FFD700;
    overflow-x: hidden;
}
.controller{
    width: 100%;
}
#navbar {
    background-color: #6A0DAD;
    max-width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    list-style-type: none;
    padding: 25px;
    margin-left: 0%;
}

#footer {
    position: absolute;
    bottom: 0;
    width: 100%;
    background-color: #2e2e2e;
    display: flex;
    justify-content: center;
    padding:10px;
    font-family: 'Roboto Mono', monospace;
    color:#FAF9F6;
}

#navbar a {
    text-decoration: none;
    font-weight:700;
    font-size: large;
    color: #FAF9F6;
    font-family:'poppins', sans-serif;
}

li {
    padding-top: 10px;
    padding:10px;
}

#head {
    font-family: playfair display;
    position: relative;
    top:-2px;
    font-size:xx-large;
    margin-left:60px;
    color:#FAF9F6;
}

p {
    text-align: left;
    color:#2A2D43;
}

.content-type {
    margin-top: 170px;
    animation: slideInLeft 1s ease-out forwards;
    display: inline-block;
    position: relative;
    bottom:100px;
    right:200px;
}
.content-type h1,p{
    color:#2A2D43;
}
@keyframes slideInLeft {
    from {
        transform: translateX(-100%);
        opacity: 0;
    }

    to {
        transform: translateX(0%);
        opacity: 1;
    }
}
*:hover{
    cursor:context-menu;
}
.menu-item {
    width: 300px;
    height: 400px;
    display: inline-block;
    object-fit: cover;
    border-radius: 10px;
    animation: scaleUp 1.2s ease-out forwards;
    position: relative;
    left: 1100px;
    top:60px;
    border-radius: 25%;
}
@keyframes scaleUp {
    from {
        opacity: 0;
        transform: scale(0.5);
    }
    to{
        opacity: 1;
        transform: scale(1);
    }
}
li:hover{
    background-color: #2A2D43;
    border-radius: 10px;
    
}
#navbar a:hover{
    color: #A2C7E5;
    cursor:pointer;
}
#footer h4{
    word-spacing: 20px;
}
#footer h1{
    font-family: 'Courier New', Courier, monospace;
    position: relative;
    right:10px;
    bottom:0px;
}
#footer h4{
    position: relative;
    top:6px;
}
#head {
  font-family: 'Great Vibes', cursive;
}

.content-type h1 {
  font-family: 'Satisfy', cursive;
}

.content-type p {
  font-family: 'Dancing Script', cursive;
}

admin.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration</title>
    <link rel="stylesheet" href="admin.css">
</head>

<body>
    <header>
        <h1>Our Administration Team</h1>
    </header>
    <div class="parent">
        <div class="child"><img src="400 PX.jpg"><h2>Founder</h2></div>
        <div class="child"><img src="download (2).jpg"><h2>Co-Founder</h2></div>
        <div class="child"><img src="download.jpg"><h2>Team Leader</h2></div>
        <div class="child"><img src="download (1).jpg"><h2>Senior Developer</h2></div>
    </div>
    <footer>
        <h4>&copy; SAM JOEL JOSHUA(25001200)</h4>
    </footer>
</body>
</html>


admin.css

*{
    padding:0px;
    margin:0px;
}
body{
    overflow: hidden;
    background-color:#FFD700;
}
footer{
    background-color: #2e2e2e;
    font-family: 'Roboto Mono', monospace;
    color:#FAF9F6;
    position:fixed;
    bottom: 0%;
    
    text-align:center;
    display: block;
    width:100%;
    padding:20px;
}
header{
    background-color:#6A0DAD;
    color:white;
    text-align: center;
    text-shadow : 2px 2px 4px rgba(0,0,0,0.4);
    padding:20px;
    width:100%;
}
.parent{
    display:flex;
    flex-direction:row;
    justify-content:center;
    margin-top:40px;
    text-align: center;
    color:#2e2e2e;
    margin-bottom:40px;

}
img{
    width:300px;
    height:450px;
    border-radius: 10%;
}
.child{
    padding:20px;
}

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <link rel="stylesheet" href="contact.css">
</head>
<body>
    <div class="box">
        <h1>Contact Us</h1><br><br>
        <p>Ready to enjoy a delicious meal at HappyFeast? We’d love to hear from you! Visit us at 123 Flavor Street, Chennai, or give us a call at (555) 123-4567 to make a reservation.</p>
        <br><p>For inquiries, catering, or special events, reach out via email at info@happyfeast.com. Follow us on social media for updates and specials. We can’t wait to welcome you to our table!</p>
        <br><br><img src="https://images.unsplash.com/photo-1552566626-52f8b828add9" alt="Restaurant Ambiance">
    </div>
    <footer>
        <h4>&copy;SAM JOEL JOSHUA (25001200)</h4>
    </footer>
</body>
</html>


contact.css

*{
    padding:0%;
    margin:0%;

}
body{
    background-color:#FFD700;
    overflow-y: hidden;
}
.box{
    position:relative;
    left:550px;
    top:60px;
    width:450px;
    color:whitesmoke;
    background-color:#6A0DAD;
    padding:10px;
    border-radius:5%;
    animation-name: anime;
    animation-duration:0.8s;
}
.box img{
    max-width:100%;
    max-height:300px;
    height:auto;
    border-radius: 10%;
    text-align: center;
}
.box h1{
    text-align: center;
    color:#FDEBD0;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.4);
}
footer{
    background-color: #2e2e2e;
    position:fixed;
    bottom: 0%; 

    width:100%;
    display : inline-block;
    padding:20px;
    color:#F5F5DC;
    text-align: center;
}
.box p{
    font-family: cursive;
}
@keyframes anime{
    from{
        transform: scale(0.5);
        opacity:0;
    }
    to{
        transform:scale(1);
        opacity: 1;
    }
}


menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HappyFeast - Menu</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Open+Sans&family=Playfair+Display&family=Roboto+Mono&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="menu.css">
</head>
<body>
    <section class="menu-section">
        <h1>Our Menu</h1>
        <div class="category">
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/725990/pexels-photo-725990.jpeg" alt="Calamari">
                <h3>Calamari</h3>
                <p>Fried squid served with marinara sauce. $9.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/533325/pexels-photo-533325.jpeg" alt="Prosciutto e Melone">
                <h3>Prosciutto e Melone</h3>
                <p>Thinly sliced prosciutto wrapped around sweet melon. $8.49</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/1437267/pexels-photo-1437267.jpeg" alt="Margherita Pizza">
                <h3>Margherita Pizza</h3>
                <p>Classic pizza with fresh tomatoes, mozzarella, and basil. $12.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/2619967/pexels-photo-2619967.jpeg" alt="Spaghetti Carbonara">
                <h3>Spaghetti Carbonara</h3>
                <p>Creamy pasta with pancetta, egg, and Parmesan. $14.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/1487511/pexels-photo-1487511.jpeg" alt="Lasagna">
                <h3>Lasagna</h3>
                <p>Layers of pasta, meat sauce, and melted cheese. $15.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/2133989/pexels-photo-2133989.jpeg" alt="Fettuccine Alfredo">
                <h3>Fettuccine Alfredo</h3>
                <p>Creamy Alfredo sauce over fettuccine pasta. $13.49</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/323682/pexels-photo-323682.jpeg" alt="Pesto Gnocchi">
                <h3>Pesto Gnocchi</h3>
                <p>Soft potato dumplings in a basil pesto sauce. $14.49</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/2144112/pexels-photo-2144112.jpeg" alt="Tiramisu">
                <h3>Tiramisu</h3>
                <p>Rich coffee-flavored dessert with mascarpone and cocoa. $6.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/338713/pexels-photo-338713.jpeg" alt="Espresso">
                <h3>Espresso</h3>
                <p>Rich, bold Italian coffee. $3.99</p>
            </div>
            <div class="menu-item">
                <img src="7udlx3rm.png" alt="Chicken Parmesan">
                <h3>Chicken Parmesan</h3>
                <p>Breaded chicken breast topped with marinara and mozzarella. $16.99</p>
            </div>
            <div class="menu-item">
                <img src="703mt8wr.png" alt="Caprese Salad">
                <h3>Caprese Salad</h3>
                <p>Fresh tomatoes, mozzarella, basil, and balsamic glaze. $7.99</p>
            </div>
            <div class="menu-item">
                <img src="https://images.pexels.com/photos/1351238/pexels-photo-1351238.jpeg" alt="Lemon Sorbet">
                <h3>Lemon Sorbet</h3>
                <p>Refreshing lemon dessert with a zesty finish. $5.99</p>
            </div>
        </div>
    </section>
    <footer>
        <h4>&copy; HappyFeast 2025 | SAM JOEL JOSHUA | 25001200</h4>
        <div class="social-links">
            <a href="#"><img src="https://img.icons8.com/ios-filled/24/ffffff/facebook-new.png" alt="Facebook"></a>
            <a href="#"><img src="https://img.icons8.com/ios-filled/24/ffffff/instagram-new.png" alt="Instagram"></a>
            <a href="#"><img src="https://img.icons8.com/ios-filled/24/ffffff/twitter.png" alt="Twitter"></a>
        </div>
    </footer>
</body>
</html>


menu.css

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Open Sans', sans-serif;
    color: #2A2D43;
}

.menu-section {
    padding: 50px;
    text-align: center;
}

.menu-section h1 {
    font-family: 'Playfair Display', serif;
    font-size: 2.5rem;
    color: #2A2D43;
    margin-bottom: 40px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

.category {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
    padding: 20px;
}

.menu-item {
    background: #FAF9F6;
    border-radius: 10px;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    animation: scaleUp 1s ease-out forwards;
}

.menu-item:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.menu-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 10px;
    margin-bottom: 15px;
}

.menu-item h3 {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.5rem;
    color: #2A2D43;
    margin-bottom: 10px;
}

.menu-item p {
    font-family: 'Open Sans', sans-serif;
    font-size: 1rem;
    color: #555;
}

footer {
    background-color: #2e2e2e;
    color: #FAF9F6;
    text-align: center;
    padding: 20px;
    font-family: 'Roboto Mono', monospace;
    margin-top: 40px;
}

footer .social-links {
    margin-top: 10px;
}

footer .social-links a {
    margin: 0 10px;
}



#navbar {
    display: none;
    flex-direction: column;
    position: absolute;
    top: 70px;
    right: 0;
    background-color: #A52A2A;
    width: 100%;
    padding: 20px;
}

#navbar {
    display: flex;
}

.menu-section {
    padding: 20px;
}

```

## OUTPUT:
![alt text](<Screenshot (41).png>)
![alt text](<Screenshot (42).png>)
![alt text](<Screenshot (43).png>)
![alt text](<Screenshot (44).png>)





## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
