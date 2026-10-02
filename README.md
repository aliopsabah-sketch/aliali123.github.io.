<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>RJ للأكلات السريعة | الكوت</title>

<style>

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    background: #f7f7f7;
    color: #222;
}

header {
    background: #111;
    color: white;
    padding: 18px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

nav a {
    color: white;
    text-decoration: none;
    margin-right: 15px;
}

.hero {
    min-height: 430px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;

    background:
    linear-gradient(#0009,#0009),
    url("https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=1400&q=80")
    center/cover;

    color: white;
    padding: 30px;
}

.hero h1 {
    font-size: 45px;
    margin-bottom: 15px;
}

.hero p {
    font-size: 20px;
    margin-bottom: 25px;
}

.btn {
    display: inline-block;
    background: #e63946;
    color: white;
    padding: 13px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    border: none;
    cursor: pointer;
}

section {
    padding: 50px 7%;
}

.title {
    text-align: center;
    margin-bottom: 30px;
}

.title h2 {
    font-size: 30px;
}

.menu {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.food {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 5px 20px #0002;
}

.food img {
    width: 100%;
    height: 190px;
    object-fit: cover;
}

.food-content {
    padding: 18px;
}

.food-content h3 {
    margin-bottom: 7px;
}

.price {
    color: #e63946;
    font-size: 19px;
    font-weight: bold;
    margin: 8px 0 15px;
}

.add {
    background: #111;
    width: 100%;
}

.cart {
    max-width: 700px;
    margin: 50px auto 0;
    background: white;
    padding: 25px;
    border-radius: 15px;
    box-shadow: 0 5px 20px #0002;
}

.cart h2 {
    margin-bottom: 20px;
}

.cart-item {
    display: flex;
    justify-content: space-between;
    padding: 12px 0;
    border-bottom: 1px solid #ddd;
}

.total {
    font-size: 22px;
    font-weight: bold;
    margin: 20px 0;
}

input,
textarea {
    width: 100%;
    padding: 14px;
    margin: 8px 0;
    border: 1px solid #ddd;
    border-radius: 8px;
    font-size: 16px;
}

.whatsapp {
    background: #168c45;
    width: 100%;
    margin-top: 10px;
}

.about {
    background: #111;
    color: white;
    text-align: center;
}

footer {
    background: #111;
    color: #aaa;
    text-align: center;
    padding: 20px;
}

@media(max-width:700px) {

    header {
        flex-direction: column;
        gap: 12px;
    }

    .menu {
        grid-template-columns: 1fr;
    }

    .hero h1 {
        font-size: 34px;
    }

    section {
        padding: 40px 20px;
    }
}

</style>
</head>


<body>


<header>

<div class="logo">
🍔 RJ للأكلات السريعة
</div>

<nav>
<a href="#menu">القائمة</a>
<a href="#order">الطلب</a>
<a href="#contact">اتصل بنا</a>
</nav>

</header>



<section class="hero">

<div>

<h1>RJ للأكلات السريعة 🍔</h1>

<p>طعم تحبه... وسرعة تستحقها</p>

<a class="btn" href="#menu">
اطلب الآن
</a>

</div>

</section>



<section id="menu">

<div class="title">

<h2>🍔 قائمة الطعام</h2>

<p>اختار وجبتك واضغط إضافة للطلب</p>

</div>


<div class="menu">


<div class="food">

<img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🍔 برغر</h3>

<p>برغر طازج ولذيذ</p>

<div class="price">2,000 د.ع</div>

<button class="btn add"
onclick="addItem('برغر',2000)">
إضافة للطلب
</button>

</div>

</div>



<div class="food">

<img src="https://images.unsplash.com/photo-1572802419224-296b0aeee0d9?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🧀 برغر بالجبن</h3>

<p>برغر مع الجبن</p>

<div class="price">2,500 د.ع</div><button class="btn add"
onclick="addItem('برغر بالجبن',2500)">
إضافة للطلب
</button>

</div>

</div>



<div class="food">

<img src="https://images.unsplash.com/photo-1601050690597-df0568f70950?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🍗 ريزو</h3>

<p>وجبة ريزو شهية</p>

<div class="price">4,000 د.ع</div>

<button class="btn add"
onclick="addItem('ريزو',4000)">
إضافة للطلب
</button>

</div>

</div>



<div class="food">

<img src="https://images.unsplash.com/photo-1562967916-eb82221dfb92?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🍗 كنتاكي</h3>

<p>دجاج مقرمش ولذيذ</p>

<div class="price">5,000 د.ع</div>

<button class="btn add"
onclick="addItem('كنتاكي',5000)">
إضافة للطلب
</button>

</div>

</div>



<div class="food">

<img src="https://images.unsplash.com/photo-1521305916504-4a1121188589?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🌯 صاج</h3>

<p>صاج طازج</p>

<div class="price">3,000 د.ع</div>

<button class="btn add"
onclick="addItem('صاج',3000)">
إضافة للطلب
</button>

</div>

</div>



<div class="food">

<img src="https://images.unsplash.com/photo-1576116101997-4b5717c7e5e6?auto=format&fit=crop&w=700&q=80">

<div class="food-content">

<h3>🍟 قدح فنكر</h3>

<p>بطاطا مقرمشة</p>

<div class="price">1,000 د.ع</div>

<button class="btn add"
onclick="addItem('قدح فنكر',1000)">
إضافة للطلب
</button>

</div>

</div>


</div>



<div class="cart" id="order">

<h2>🛒 طلبك</h2>

<div id="cartItems">
لا توجد وجبات مضافة.
</div>

<div class="total">
المجموع: <span id="total">0</span> د.ع
</div>


<input
type="text"
id="name"
placeholder="اسمك">


<input
type="text"
id="address"
placeholder="العنوان / المنطقة">


<textarea
id="notes"
placeholder="ملاحظات إضافية"></textarea>


<button
class="btn whatsapp"
onclick="sendOrder()">

🟢 إرسال الطلب عبر WhatsApp

</button>

</div>

</section>



<section class="about">

<div class="title">

<h2>عن RJ</h2>

</div>

<p>
RJ للأكلات السريعة - الكوت الخاجية
<br>
قرب مدرسة النهرين
</p>

</section>



<section id="contact">

<div class="title">

<h2>📞 تواصل معنا</h2>

<p>07727071206</p>

</div>

</section>



<footer>

© 2026 RJ للأكلات السريعة

</footer>


<script>

let cart = [];

const deliveryFee = 2000;


function addItem(name, price) {

    const existing = cart.find(item => item.name === name);

    if (existing) {
        existing.quantity++;
    } else {
        cart.push({
            name: name,
            price: price,
            quantity: 1
        });
    }

    updateCart();

    document.getElementById("order")
        .scrollIntoView({ behavior: "smooth" });
}


function increaseItem(index) {

    cart[index].quantity++;

    updateCart();
}


function decreaseItem(index) {

    cart[index].quantity--;

    if (cart[index].quantity <= 0) {
        cart.splice(index, 1);
    }

    updateCart();
}


function removeItem(index) {

    cart.splice(index, 1);

    updateCart();
}


function updateCart() {

    const container =
        document.getElementById("cartItems");

    const totalElement =
        document.getElementById("total");


    if (cart.length === 0) {

        container.innerHTML =
            "<p>🛒 لا توجد وجبات في الطلب.</p>";

        totalElement.innerText = "0";

        return;
    }


    let subtotal = 0;

    container.innerHTML = "";


    cart.forEach((item, index) => {

        const itemTotal =
            item.price * item.quantity;

        subtotal += itemTotal;


        container.innerHTML += `

        <div class="cart-item">

            <div>

                <strong>
                    ${item.name}
                </strong>

                <br>

                <small>
                    ${item.price.toLocaleString()} د.ع ×
                    ${item.quantity}
                </small>

            </div>


            <div>

                <button
                    onclick="decreaseItem(${index})">
                    −
                </button>


                <strong style="margin:0 8px;">
                    ${item.quantity}
                </strong>


                <button
                    onclick="increaseItem(${index})">
                    +
                </button>


                <button
                    onclick="removeItem(${index})"
                    style="margin-right:8px;">
                    🗑️
                </button>

            </div>

        </div>

        `;

    });


    const delivery =
        subtotal > 0 ? deliveryFee : 0;


    const finalTotal =
        subtotal + delivery;


    totalElement.innerHTML = `

        <div>
            قيمة الطلب:
            ${subtotal.toLocaleString()} د.ع
        </div>

        <div>
            🚚 التوصيل:
            ${delivery.toLocaleString()} د.ع
        </div>

        <div style="margin-top:10px;">
            💰 الإجمالي:
            ${finalTotal.toLocaleString()} د.ع
        </div>

    `;

}


function sendOrder() {

    if (cart.length === 0) {

        alert("🛒 أضف وجبة واحدة على الأقل.");

        return;
    }


    const name =
        document.getElementById("name").value.trim();


    const address =
        document.getElementById("address").value.trim();


    const notes =
        document.getElementById("notes").value.trim();


    if (name === "") {

        alert("اكتب اسمك أولاً.");

        return;
    }


    if (address === "") {

        alert("اكتب عنوان التوصيل.");

        return;
    }


    let subtotal = 0;


    let message =
        "🍔 *طلب جديد - RJ للأكلات السريعة*%0A";

    message +=
        "━━━━━━━━━━━━━━%0A";


    message +=
        "👤 الاسم: " +
        encodeURIComponent(name) +
        "%0A";


    message +=
        "📍 العنوان: " +
        encodeURIComponent(address) +
        "%0A%0A";


    message +=
        "🛒 *الطلب:*%0A";


    cart.forEach(item => {

        const itemTotal =
            item.price * item.quantity;


        subtotal += itemTotal;


        message +=
            "• " +
            encodeURIComponent(item.name) +
            " × " +
            item.quantity +
            " = " +
            itemTotal.toLocaleString() +
            " د.ع%0A";

    });


    const delivery =
        deliveryFee;


    const finalTotal =
        subtotal + delivery;message +=
        "%0A💵 قيمة الطلب: " +
        subtotal.toLocaleString() +
        " د.ع";


    message +=
        "%0A🚚 التوصيل: " +
        delivery.toLocaleString() +
        " د.ع";


    message +=
        "%0A💰 *الإجمالي: " +
        finalTotal.toLocaleString() +
        " د.ع*";


    if (notes !== "") {

        message +=
            "%0A%0A📝 ملاحظات: " +
            encodeURIComponent(notes);

    }


    const phone =
        "9647727071206";


    const whatsappURL =
        "https://wa.me/" +
        phone +
        "?text=" +
        message;


    window.open(
        whatsappURL,
        "_blank"
    );

}

</script>


</body>
</html>