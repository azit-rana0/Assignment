#Project: Amazon Clone

This project is a simplified Amazon clone created using only HTML and CSS. Below are the screenshots of the UI, along with explanations of the HTML tags and CSS properties used to create each part of the interface.

#This part is a HTML.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
    <link rel="icon" href="https://cdn-icons-png.flaticon.com/128/11378/11378728.png">
    <link rel="stylesheet" href="./style.css">
    <title>Amazon Clone</title>
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="navlogo">
                <a href="#">
                    <img src="https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/amazon_logo.png" alt="">
                </a>
            </div>
            <div class="address">
                <p>Deliver</p>
                <div class="loction">
                    <i class="material-symbols-outlined">location_on</i>
                    <p>India</p>
                </div>
            </div>
            <div class="navSearch">
                <select>
                    <option>All</option>
                    <option>All Categories</option>
                    <option>Amazon Devices</option>
                </select>
                <input type="text" placeholder="Search Amazon">
                <button><i class="material-symbols-outlined">search</i></button>
            </div>
            <div class="signIn">
                <p class="sign">Hello, sign in</p>
                <p class="account">Account & Lists</p>
            </div>
            <div class="returns">
                <p class="return">Returns</p>
                <p class="order account">& Orders
                </p>
            </div>
            <div class="navcart">
                <i class="material-symbols-outlined">shopping_cart</i>
                <p>Cart</p>
            </div>
        </nav>
        <div class="banner">
            <div class="menu">
                <ul class="menuList">
                    <li><i class="material-symbols-outlined">menu</i></li>
                    <li>All</li>
                    <li>Today's Deals</li>
                    <li>Customer Service</li>
                    <li>Registry</li>
                    <li>Gift Cards</li>
                    <li>Sell</li>
                </ul>
            </div>
            <div class="shop">
                <p>Shop deals in Electronics</p>
            </div>
        </div>
    </header>

    <main>
        <section class="prime"></section>
        <section class="carts">
            <div class="cart">
                <h3 class="cartTitle">Shop Laptops & Tables</h3>
                <img src="https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/img-1.png" alt="Laptop">
                <a href="#">Shop now</a>
            </div>

            <div class="cart">
                <h3 class="cartTitle">Shop Smartwatches</h3>
                <img src="https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/img-2.png" alt="Smartwatches">
                <a href="#">Shop now</a>
            </div>

            <div class="cart">
                <h3 class="cartTitle">Create with Strip Lights</h3>
                <img src="https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/img-3.png" alt="Lights">
                <a href="#">Shop now</a>
            </div>

            <div class="cart">
                <h3 class="cartTitle">Home Refresh Ideas</h3>
                <img src="https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/img-4.png" alt="Refresh">
                <a href="#">Shop now</a>
            </div>
        </section>

        <section class="back">
            <div>
                <a href="#">Back to top</a>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="footer-content">
            <p>Get to Know Us</p>
            <ul>
                <li>About us</li>
                <li>Careers</li>
                <li>Press Release</li>
                <li>Amazon Science</li>
            </ul>
        </div>
        <div class="footer-content">
            <p>Connect with Us</p>
            <ul>
                <li>Facebook</li>
                <li>Twitter</li>
                <li>Instagram</li>
            </ul>
        </div>
        <div class="footer-content">
            <p>Make Money with Us</p>
            <ul>
                <li>Sell on Amazon</li>
                <li>Sell under Amazon Accelerator</li>
                <li>Protect and Build Your Brand</li>
                <li>Amazon Global Selling</li>
                <li>Become an Affiliate</li>
                <li>Fulfillment by Amazon</li>
                <li>Advertise Your Products</li>
                <li>Amazon Pay on Merchants</li>
            </ul>
        </div>
        <div class="footer-content">
            <p>Let Us Help You</p>
            <ul>
                <li>COVID-19 and Amazon</li>
                <li>Your Account</li>
                <li>Return Centre</li>
                <li>100% Purchase Protection</li>
                <li>Amazon App Download</li>
                <li>Help</li>
            </ul>
        </div>
    </footer>
</body>
</html>


#This part is CSS part.

@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Open Sans", sans-serif;
    scroll-behavior: smooth;
 }
/* header */
 .navbar {
    width: 100%;
    height: 60px;
    background-color: rgb(14,16,17);
    display: flex;
    align-items: center;
    justify-content: space-between;
    cursor: pointer;
    color: rgb(255, 255, 255);
    padding-inline: 7%;
 }
.navbar:hover {
    color: rgb(221, 221, 221);
}
 .navlogo > a > img {
    width: 130px;
    margin-top: 10px;
 }

 .address {
    display: flex;
    flex-direction: column;
 }

 .address > p {
    font-size: 12px;
    margin-left: 20px;
    color: rgb(204, 204, 204);
 }

 .loction {
    display: flex;
    flex-direction: row;
    align-items: center;
    font-weight: 500;
 }

 .navSearch {
    width: 48%;
    height: 40px;
    display: flex;
    flex-direction: row;
 }

 .navSearch > select {
    width: 50px;
    height: 100%;
    border: none;
    text-align: center;
    font-weight: 100;
    color: rgba(34, 33, 33, 0.816);
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
 }

 .navSearch > input {
    height: 100%;
    width: 100%;
    border: none;
    font-size: 16px;
    font-weight: 100;
    padding-left: 5px;
    letter-spacing: 0.8px;
 }

 .navSearch > input:focus {
    outline: none;
 }

 .navSearch > button {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    width: 50px;
    background-color: rgb(254,188,105);
    border: none;
    border-top-right-radius: 5px;
    border-bottom-right-radius: 5px;
    cursor: pointer;
 }

 .signIn, .returns {
    display: flex;
    flex-direction: column;
    gap: 5px;
    font-weight: 600;
 }

 .signIn > .sign {
    font-size: 12px;
 }

 .signIn > .account, .order{
    font-size: 14px;
 }

 .returns > .return {
    font-size: 12px;
    font-weight: 500;
 }

 .navcart {
    display: flex;
    align-items: end;
 }

 .navcart > i {
    font-size: 40px;
 }
 
/* banner */
 .banner {
    width: 100%;
    height: 45px;
    background-color: rgb(34,47,61);
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-inline: 7%;
    font-size: 14px;
    font-weight: 100;
 }

 .shop:hover{
    color: rgb(221, 221, 221);
    cursor: pointer;
 }
 .menuList > li:hover {
    color: rgb(221, 221, 221);
    cursor: pointer;
 }
.menu > ul > li > i {
    margin-top: 4px;
}
 .menu > ul{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
 }

 .menu > ul > li {
    list-style: none;
 }

/* main Section */
 .prime {
    height: 400px;
    width: 100%;
    background-image: url('https://priyanshu-240499.github.io/Assignments-CSS/Weekly%20Test%20for%20CSS%20(Week-3)/images/hero-img.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
 }

 .carts {
    width: 100%;
    height: fit-content;
    background-color: rgb(243,242,242);
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 40px;
    padding: 50px 0;
 }

 .cart {
    width: 300px;
    height: 400px;
    background-color: rgb(254,254,255);
    display: flex;
    gap: 15px;
    flex-direction: column;
    justify-content: center;
    align-items: start;
    padding: 30px;
    cursor: pointer;
    transition: 0.7s ease-in-out;
 }

 .cart:hover {
    transform: scale(1.06);  
 }

 .cart:hover > a {
    color: brown;
    text-decoration: underline;
 }

 .cart > img{
    width: 100%;
    height: 100%;
    object-fit: cover;
 }

 .cart > a {
    text-decoration: none;
 }

 .back {
    width: 100%;
    height: 60px;
    background-color: rgb(55,71,90);
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 14px;
 }

 .back > div > a {
    text-decoration: none;
    color: white;
 }

 .back > div > a:hover {
    color: rgb(221, 221, 221)
 }

 /* footer */

 .footer {
    background-color: rgb(35,46,63);
    color: white;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 20px 12%;
 }

 .footer-content > p {
    margin-bottom: 15px;
    font-size: 16px;
 }

 .footer-content > ul > li {
    list-style: none;
    margin-top: 5px;
    font-size: 14px;
    color: rgb(221, 221, 221);
    letter-spacing: 1px;
 }

 .footer-content > ul > li:hover {
    text-decoration: underline;
 }
