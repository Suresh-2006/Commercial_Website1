# Ex02 Commercial Website
## Date:28-07-2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

### index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechStore</title>

    <!-- CSS -->
    <link rel="stylesheet" href="styles.css">
</head>

<body>

    <!-- Header -->
    <header>

        <h1>TechStore</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
            <a href="#account">Account</a>
        </nav>

    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">

        <div class="hero-text">

            <h2>Premium Electronics For Everyone</h2>

            <p>
                Discover the latest laptops, smartphones and accessories
                at unbeatable prices.
            </p>

            <button>Explore Products</button>

        </div>

        <div class="hero-image">

            <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=700"
                alt="Electronics">

        </div>

    </section>

    <!-- Products -->

    <section id="products">

        <h2>Featured Products</h2>

        <div class="product-container">

            <div class="card">

                <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=600"
                    alt="Laptop">

                <h3>Gaming Laptop</h3>

                <p>
                    High performance laptop for professionals,
                    gamers and students.
                </p>

                <h4>$899</h4>

                <button>Buy Now</button>

            </div>

            <div class="card">

                <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=600"
                    alt="Phone">

                <h3>Smartphone</h3>

                <p>
                    Experience flagship performance with
                    an amazing camera.
                </p>

                <h4>$699</h4>

                <button>Buy Now</button>

            </div>

            <div class="card">

                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=600"
                    alt="Headphones">

                <h3>Headphones</h3>

                <p>
                    Crystal clear sound with premium
                    noise cancellation.
                </p>

                <h4>$199</h4>

                <button>Buy Now</button>

            </div>

        </div>

    </section>

    <!-- About -->

    <section id="about">

        <h2>About TechStore</h2>

        <div class="about">

            <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?w=700"
                alt="About Us">

            <div>

                <p>

                    TechStore is your trusted destination for premium
                    electronic gadgets. We provide genuine products,
                    affordable pricing, fast delivery and dedicated
                    customer support. Our goal is to make technology
                    accessible for everyone with a hassle-free shopping
                    experience.

                </p>

            </div>

        </div>

    </section>

    <!-- Contact -->

    <section id="contact">

        <h2>Contact Us</h2>

        <div class="contact-box">

            <p>📧 support@techstore.com</p>

            <p>📞 +91 98765 43210</p>

            <p>📍 Chennai, Tamil Nadu</p>

            <p>🕒 Mon - Sat : 9.00 AM - 8.00 PM</p>

        </div>

    </section>

    <!-- Login -->

    <section id="account">

        <h2>User Login</h2>

        <div class="account-box">

            <input type="text" placeholder="Username">

            <input type="password" placeholder="Password">

            <button>Login</button>

        </div>

    </section>

    <!-- Footer -->

    <footer>

        <div class="social">

            <a href="#">Facebook</a>

            <a href="#">Instagram</a>

            <a href="#">Twitter</a>

            <a href="#">LinkedIn</a>

        </div>

        <p>© 2026 TechStore | All Rights Reserved</p>

    </footer>

</body>

</html>
```

### styles.css

```
/* Google Font */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#f4f7fc;
    color:#333;
}

/* HEADER */

header{
    background:#0f172a;
    color:white;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:18px 70px;
    position:sticky;
    top:0;
    z-index:100;
    box-shadow:0 3px 10px rgba(0,0,0,.2);
}

header h1{
    color:#38bdf8;
}

nav{
    display:flex;
    gap:25px;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:500;
    transition:.3s;
}

nav a:hover{
    color:#38bdf8;
}

/* HERO */

.hero{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:70px;
    background:linear-gradient(135deg,#2563eb,#38bdf8);
    color:white;
    flex-wrap:wrap;
}

.hero-text{
    flex:1;
}

.hero-text h2{
    font-size:48px;
    margin-bottom:15px;
}

.hero-text p{
    font-size:20px;
    margin-bottom:25px;
}

.hero button{
    padding:12px 28px;
    border:none;
    background:white;
    color:#2563eb;
    border-radius:30px;
    font-size:16px;
    font-weight:600;
    cursor:pointer;
    transition:.3s;
}

.hero button:hover{
    transform:translateY(-4px);
    box-shadow:0 8px 20px rgba(0,0,0,.25);
}

.hero-image{
    flex:1;
    text-align:center;
}

.hero-image img{
    width:430px;
    border-radius:20px;
    box-shadow:0 15px 35px rgba(0,0,0,.25);
}

/* SECTION */

section{
    padding:70px;
}

section h2{
    text-align:center;
    font-size:34px;
    margin-bottom:40px;
    color:#0f172a;
}

/* PRODUCTS */

.product-container{
    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;
}

.card{
    width:290px;
    background:white;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 10px 25px rgba(0,0,0,.12);
    transition:.35s;
    text-align:center;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:200px;
    object-fit:cover;
}

.card h3{
    margin:18px 0 10px;
}

.card p{
    padding:0 18px;
    color:#666;
}

.card h4{
    color:#2563eb;
    margin:15px 0;
}

.card button{
    background:#2563eb;
    color:white;
    border:none;
    width:100%;
    padding:14px;
    cursor:pointer;
    transition:.3s;
}

.card button:hover{
    background:#1d4ed8;
}

/* ABOUT */

.about{
    display:flex;
    gap:40px;
    align-items:center;
    flex-wrap:wrap;
}

.about img{
    width:420px;
    border-radius:15px;
}

.about p{
    flex:1;
    line-height:1.8;
    color:#555;
}

/* CONTACT */

.contact-box{
    width:450px;
    margin:auto;
    background:white;
    padding:35px;
    border-radius:15px;
    box-shadow:0 10px 25px rgba(0,0,0,.1);
}

.contact-box p{
    margin:15px 0;
    font-size:17px;
}

/* LOGIN */

.account-box{
    width:400px;
    margin:auto;
    background:white;
    padding:35px;
    border-radius:15px;
    box-shadow:0 10px 25px rgba(0,0,0,.1);

    display:flex;
    flex-direction:column;
    gap:18px;
}

.account-box input{
    padding:14px;
    border:1px solid #ccc;
    border-radius:8px;
    outline:none;
}

.account-box input:focus{
    border-color:#2563eb;
}

.account-box button{
    padding:14px;
    border:none;
    background:#2563eb;
    color:white;
    border-radius:8px;
    cursor:pointer;
    transition:.3s;
}

.account-box button:hover{
    background:#1d4ed8;
}

/* FOOTER */

footer{
    background:#0f172a;
    color:white;
    text-align:center;
    padding:30px;
}

.social{
    display:flex;
    justify-content:center;
    gap:25px;
    margin-bottom:15px;
}

.social a{
    color:white;
    text-decoration:none;
    transition:.3s;
}

.social a:hover{
    color:#38bdf8;
}

/* MOBILE */

@media(max-width:768px){

header{
    flex-direction:column;
    gap:20px;
    padding:20px;
}

.hero{
    flex-direction:column;
    text-align:center;
}

.hero-text h2{
    font-size:35px;
}

.hero-image img{
    width:100%;
    margin-top:30px;
}

.about{
    flex-direction:column;
}

.about img{
    width:100%;
}

.contact-box,
.account-box{
    width:100%;
}

}
```


## OUTPUT
![alt text](<EXP_2/Screenshot 2026-07-28 134944.png>)
![alt text](<EXP_2/Screenshot 2026-07-28 135000.png>)
![alt text](<EXP_2/Screenshot 2026-07-28 135017.png>)
![alt text](<EXP_2/Screenshot 2026-07-28 135031.png>)
![alt text](<EXP_2/Screenshot 2026-07-28 135043.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
