# -bama-fashion
    BAMA Premium Clothing Store 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>BAMA | Premium Fashion</title>

<meta name="description"
content="BAMA Premium Fashion - Men's and Women's stylish clothing.">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#f5f3ef;
    color:#111;
}

/* HEADER */

header{
    height:72px;
    background:#0a0a0a;
    color:white;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 6%;
    position:sticky;
    top:0;
    z-index:1000;
}

.logo{
    font-size:28px;
    font-weight:800;
    letter-spacing:7px;
}

.cart{
    font-size:16px;
}

/* HERO */

.hero{
    min-height:600px;
    background:
    linear-gradient(rgba(0,0,0,.48),rgba(0,0,0,.58)),
    url("IMG_3304.jpeg") center/cover;

    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    color:white;
    padding:30px;
}

.hero-content{
    max-width:700px;
}

.hero-small{
    font-size:13px;
    letter-spacing:5px;
    margin-bottom:20px;
}

.hero h1{
    font-size:clamp(55px,12vw,110px);
    letter-spacing:14px;
}

.hero p{
    font-size:17px;
    letter-spacing:2px;
    margin:15px 0 30px;
}

.hero-btn{
    display:inline-block;
    padding:16px 34px;
    background:#c9a85f;
    color:#111;
    text-decoration:none;
    font-weight:bold;
    letter-spacing:2px;
}

/* SECTION */

.section{
    padding:65px 6%;
}

.heading{
    text-align:center;
    margin-bottom:35px;
}

.heading span{
    font-size:12px;
    letter-spacing:4px;
    color:#a88745;
}

.heading h2{
    font-size:36px;
    margin-top:10px;
}

/* CATEGORY */

.categories{
    display:flex;
    justify-content:center;
    gap:12px;
    flex-wrap:wrap;
    margin-bottom:35px;
}

.categories button{
    padding:12px 28px;
    border:1px solid #111;
    background:white;
    border-radius:30px;
    cursor:pointer;
}

.categories button.active{
    background:#111;
    color:white;
}

/* PRODUCTS */

.products{
    max-width:500px;
    margin:auto;
}

.product{
    background:white;
    box-shadow:0 10px 35px rgba(0,0,0,.10);
    overflow:hidden;
}

.product-image{
    position:relative;
}

.product img{
    width:100%;
    height:auto;
    max-height:650px;
    object-fit:cover;
    display:block;
}

.badge{
    position:absolute;
    top:15px;
    left:15px;
    background:#111;
    color:white;
    padding:8px 13px;
    font-size:11px;
    letter-spacing:1px;
}

.info{
    padding:22px;
}

.category{
    font-size:12px;
    color:#888;
    letter-spacing:2px;
    text-transform:uppercase;
    margin-bottom:8px;
}

.info h3{
    font-size:19px;
    line-height:1.4;
    margin-bottom:12px;
}

.price{
    font-size:25px;
    font-weight:bold;
    margin-bottom:18px;
}

/* SIZE */

.size-title{
    font-size:13px;
    font-weight:bold;
    margin-bottom:8px;
}

.sizes{
    display:flex;
    gap:8px;
    margin-bottom:20px;
}

.sizes button{
    flex:1;
    padding:11px 5px;
    background:white;
    border:1px solid #bbb;
    cursor:pointer;
}

.sizes button.selected{
    background:#111;
    color:white;
    border-color:#111;
}

/* ORDER */

.order{
    width:100%;
    padding:16px;
    border:0;
    background:#111;
    color:white;
    font-size:14px;
    font-weight:bold;
    letter-spacing:1px;
    cursor:pointer;
}

.order:hover{
    background:#c9a85f;
    color:#111;
}

/* BRAND */

.brand{
    background:#0a0a0a;
    color:white;
    text-align:center;
}

.brand-logo{
    font-size:42px;
    letter-spacing:9px;
    font-weight:bold;
    margin-bottom:18px;
}

.brand p{
    max-width:650px;
    margin:auto;
    color:#aaa;
    line-height:1.8;
}

/* CONTACT */

.contact{
    text-align:center;
}

.contact-item{
    margin:18px 0;
}

.contact a{
    color:#111;
    text-decoration:none;
    font-weight:bold;
}

.whatsapp{
    display:inline-block;
    margin-top:15px;
    padding:16px 30px;
    background:#111;
    color:white !important;
}

/* FOOTER */

footer{
    background:#050505;
    color:#777;
    text-align:center;
    padding:30px 15px;
}

.footer-logo{
    color:white;
    font-size:23px;
    letter-spacing:5px;
    margin-bottom:10px;
}

/* MOBILE */

@media(max-width:600px){

    header{
        padding:0 5%;
    }

    .logo{
        font-size:23px;
        letter-spacing:5px;
    }

    .hero{
        min-height:520px;
    }

    .hero h1{
        font-size:58px;
        letter-spacing:8px;
    }

    .section{
        padding:50px 5%;
    }

    .heading h2{
        font-size:29px;
    }

}

</style>
</head>

<body>

<!-- HEADER -->

<header>

    <div class="logo">
        BAMA
    </div>

    <div class="cart">
        🛒 Cart (<span id="cartCount">0</span>)
    </div>

</header>


<!-- HERO -->

<section class="hero">

    <div class="hero-content">

        <div class="hero-small">
            PREMIUM FASHION
        </div>

        <h1>
            BAMA
        </h1>

        <p>
            STYLE THAT SPEAKS FOR YOU
        </p>

        <a href="#shop" class="hero-btn">
            SHOP NOW
        </a>

    </div>

</section>


<!-- SHOP -->

<section class="section" id="shop">

    <div class="heading">

        <span>
            BAMA COLLECTION
        </span>

        <h2>
            MEN'S COLLECTION
        </h2>

    </div>


    <div class="categories">

        <button class="active">
            MEN
        </button>

        <button onclick="showWomenMessage()">
            WOMEN
        </button>

    </div>


    <div class="products">

        <!-- PRODUCT -->

        <div class="product">

            <div class="product-image">

                <img
                    src="IMG_3304.jpeg"
                    alt="Men Regular Fit Solid Spread Collar Casual Shirt">

                <div class="badge">
                    NEW
                </div>

            </div>


            <div class="info">

                <div class="category">
                    MEN
                </div>

                <h3>
                    Men Regular Fit Solid Spread Collar Casual Shirt
                </h3>

                <div class="price">
                    ₹699
                </div>


                <div class="size-title">
                    SELECT SIZE
                </div>


                <div class="sizes">

                    <button onclick="selectSize(this,'M')">
                        M
                    </button>

                    <button onclick="selectSize(this,'L')">
                        L
                    </button>

                    <button onclick="selectSize(this,'XL')">
                        XL
                    </button>

                    <button onclick="selectSize(this,'XXL')">
                        XXL
                    </button>

                </div>


                <button
                    class="order"
                    onclick="orderProduct()">

                    ORDER ON WHATSAPP

                </button>

            </div>

        </div>

    </div>

</section>


<!-- BRAND -->

<section class="section brand">

    <div class="brand-logo">
        BAMA
    </div>

    <p>
        Premium fashion for Men & Women.
        Discover stylish clothing designed
        for your everyday look.
    </p>

</section>


<!-- CONTACT -->

<section class="section contact">

    <div class="heading">

        <span>
            GET IN TOUCH
        </span>

        <h2>
            CONTACT BAMA
        </h2>

    </div>


    <div class="contact-item">

        📞

        <a href="tel:8822153715">
            8822153715
        </a>

    </div>


    <div class="contact-item">

        📧

        <a href="mailto:babuansari7099871017@gmail.com">

            babuansari7099871017@gmail.com

        </a>

    </div>


    <a
        class="whatsapp"
        href="https://wa.me/918822153715"
        target="_blank">

        💬 CHAT ON WHATSAPP

    </a>

</section>


<!-- FOOTER -->

<footer>

    <div class="footer-logo">
        BAMA
    </div>

    Premium Fashion for Men & Women

    <br><br>

    © 2026 BAMA. All Rights Reserved.

</footer>


<script>

let selectedSize = "";
let cart = 0;


/* SIZE SELECT */

function selectSize(button,size){

    document
    .querySelectorAll(".sizes button")
    .forEach(btn => {
        btn.classList.remove("selected");
    });

    button.classList.add("selected");

    selectedSize = size;
}


/* WHATSAPP ORDER */

function orderProduct(){

    if(selectedSize === ""){

        alert("Please select a size first.");

        return;
    }


    cart++;

    document
    .getElementById("cartCount")
    .innerText = cart;


    const product =
    "Men Regular Fit Solid Spread Collar Casual Shirt";


    const price = "₹699";


    const message =
`Hello BAMA 👋

I want to order:

🛍️ Product: ${product}

💰 Price: ${price}

📏 Size: ${selectedSize}

Please confirm availability and delivery details.`;


    const whatsapp =
    "https://wa.me/918822153715?text="
    + encodeURIComponent(message);


    window.open(whatsapp,"_blank");

}


/* WOMEN */

function showWomenMessage(){

    alert(
        "Women's Collection is coming soon! ❤️"
    );

}

</script>

</body>
</html>
