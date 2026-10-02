<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RJ للأكلات السريعة</title>

<style>
*{box-sizing:border-box;margin:0;padding:0}

body{
font-family:Arial,Tahoma,sans-serif;
background:#f7f7f7;
color:#222;
line-height:1.7
}

header{
background:#111;
color:white;
padding:18px 5%;
display:flex;
justify-content:space-between;
align-items:center;
position:sticky;
top:0;
z-index:1000
}

.logo{
font-size:24px;
font-weight:bold;
color:#ffb000
}

nav a{
color:white;
text-decoration:none;
margin:0 8px
}

.hero{
min-height:420px;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
padding:40px 20px;
background:
linear-gradient(#0008,#0008),
url("https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=1400&q=80")
center/cover
}

.hero h1{
font-size:45px;
color:white;
margin-bottom:15px
}

.hero p{
color:white;
font-size:20px
}

.btn{
display:inline-block;
margin-top:20px;
padding:13px 25px;
background:#ffb000;
color:#111;
text-decoration:none;
border-radius:10px;
font-weight:bold
}

section{
padding:50px 6%
}

.title{
text-align:center;
font-size:32px;
margin-bottom:30px
}

.menu{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
gap:20px
}

.card{
background:white;
border-radius:15px;
overflow:hidden;
box-shadow:0 4px 15px #0001;
transition:.2s
}

.card:hover{
transform:translateY(-4px)
}

.card img{
width:100%;
height:180px;
object-fit:cover
}

.card-content{
padding:18px
}

.card h3{
font-size:21px
}

.price{
color:#e58b00;
font-size:19px;
font-weight:bold;
margin:8px 0
}

.add{
width:100%;
border:0;
padding:12px;
border-radius:8px;
background:#111;
color:white;
cursor:pointer;
font-size:16px
}

.cart{
max-width:700px;
margin:auto;
background:white;
padding:25px;
border-radius:15px;
box-shadow:0 4px 15px #0001
}

.cart-item{
display:flex;
justify-content:space-between;
align-items:center;
border-bottom:1px solid #ddd;
padding:12px 0;
gap:10px
}

.qty button{
border:0;
background:#eee;
padding:5px 10px;
border-radius:5px;
cursor:pointer
}

.total{
font-size:20px;
font-weight:bold;
margin-top:20px
}

input,textarea{
width:100%;
padding:13px;
margin-top:10px;
border:1px solid #ddd;
border-radius:8px;
font-size:16px
}

textarea{
height:90px;
resize:none
}

.order{
width:100%;
margin-top:15px;
padding:14px;
border:0;
border-radius:9px;
background:#25D366;
color:white;
font-size:18px;
font-weight:bold;
cursor:pointer
}

.contact{
text-align:center;
background:#111;
color:white
}

.contact a{
color:#ffb000;
text-decoration:none
}

footer{
text-align:center;
padding:20px;
background:#000;
color:#aaa
}

@media(max-width:600px){
.hero h1{font-size:32px}
.hero p{font-size:17px}

header{
flex-direction:column;
gap:10px
}

nav a{
font-size:14px
}

section{
padding:35px 5%
}
}
</style>
</head>

<body>

<header>
<div class="logo">RJ للأكلات السريعة 🍔</div>

<nav>
<a href="#home">الرئيسية</a>
<a href="#menu">المنيو</a>
<a href="#cart">السلة</a>
<a href="#contact">اتصل بنا</a>
</nav>
</header>

<section class="hero" id="home">
<div>
<h1>RJ للأكلات السريعة</h1>
<p>طعم تحبه... وسرعة تستحقها 🍔🔥</p>
<p>الكوت - الخاجية - قرب مدرسة النهرين</p>
<a href="#menu" class="btn">شوف المنيو</a>
</div>
</section>

<section id="menu">

<h2 class="title">🍔 المنيو</h2>

<div class="menu">

<div class="card">
<img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>برغر</h3>
<div class="price">2,000 د.ع</div>
<button class="add" onclick="addToCart('برغر',2000)">أضف للسلة</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1550317138-10000687a72b?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>بركر بالجبن</h3>
<div class="price">2,500 د.ع</div>
<button class="add" onclick="addToCart('بركر بالجبن',2500)">أضف للسلة</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1601050690597-df0568f70950?auto=format&fit=crop&w=800&q=80"><div class="card-content">
<h3>ريزو</h3>
<div class="price">4,000 د.ع</div>
<button class="add" onclick="addToCart('ريزو',4000)">أضف للسلة</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1529059997568-3d847b1154f0?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>كنتاكي</h3>
<div class="price">5,000 د.ع</div>
<button class="add" onclick="addToCart('كنتاكي',5000)">أضف للسلة</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1601050690117-94f5f6fa8bd7?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>صاج</h3>
<div class="price">3,000 د.ع</div>
<button class="add" onclick="addToCart('صاج',3000)">أضف للسلة</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1541592106381-b31e9677c0e5?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>قدح فنكر</h3>
<div class="price">1,000 د.ع</div>
<button class="add" onclick="addToCart('قدح فنكر',1000)">أضف للسلة</button>
</div>
</div>

</div>
</section>

<section id="cart">

<h2 class="title">🛒 سلة الطلب</h2>

<div class="cart">

<div id="cartItems">
السلة فارغة
</div>

<div class="total">
المجموع: <span id="total">0</span> د.ع
</div>

<input id="name" placeholder="اسم الزبون">

<input id="address" placeholder="العنوان">

<textarea id="notes" placeholder="ملاحظات إضافية"></textarea>

<button class="order" onclick="sendOrder()">
📲 إرسال الطلب عبر واتساب
</button>

</div>
</section>

<section class="contact" id="contact">

<h2 class="title">📞 اتصل بنا</h2>

<p>📍 الكوت - الخاجية - قرب مدرسة النهرين</p>

<p>📱 <a href="tel:07727071206">07727071206</a></p>

<a class="btn" href="https://wa.me/9647727071206">
تواصل معنا واتساب
</a>

</section>

<footer>
© 2026 RJ للأكلات السريعة - جميع الحقوق محفوظة
</footer>

<script>

let cart=[];

const deliveryFee=2000;

function addToCart(name,price){

let item=cart.find(x=>x.name===name);

if(item){
item.qty++;
}else{
cart.push({
name:name,
price:price,
qty:1
});
}

renderCart();

}

function renderCart(){

let box=document.getElementById("cartItems");

if(cart.length===0){

box.innerHTML="السلة فارغة";
document.getElementById("total").innerText="0";

return;
}

let html="";
let total=0;

cart.forEach((item,index)=>{

let subtotal=item.price*item.qty;

total+=subtotal;

html+=`

<div class="cart-item">

<div>
<strong>${item.name}</strong><br>
${item.price.toLocaleString()} د.ع
</div>

<div class="qty">

<button onclick="changeQty(${index},-1)">−</button>

<span>${item.qty}</span>

<button onclick="changeQty(${index},1)">+</button>

<button onclick="removeItem(${index})">🗑️</button>

</div>

</div>

`;

});

html+=`
<hr>
<div style="margin-top:15px">
أجرة التوصيل: ${deliveryFee.toLocaleString()} د.ع
</div>
`;

box.innerHTML=html;

document.getElementById("total").innerText=
(total+deliveryFee).toLocaleString();

}

function changeQty(index,value){

cart[index].qty+=value;

if(cart[index].qty<=0){
cart.splice(index,1);
}

renderCart();

}

function removeItem(index){

cart.splice(index,1);

renderCart();

}

function sendOrder(){

if(cart.length===0){

alert("السلة فارغة");

return;
}

let name=document.getElementById("name").value.trim();

let address=document.getElementById("address").value.trim();

let notes=document.getElementById("notes").value.trim();

if(!name || !address){

alert("يرجى كتابة الاسم والعنوان");

return;
}

let message="🍔 *طلب جديد من RJ للأكلات السريعة*%0A%0A";

message+="👤 الاسم: "+name+"%0A";

message+="📍 العنوان: "+address+"%0A%0A";

message+="🛒 *الطلبات:*%0A";

let total=0;

cart.forEach(item=>{

let subtotal=item.price*item.qty;

total+=subtotal;

message+="• "+item.name+
" × "+item.qty+
" = "+subtotal.toLocaleString()+" د.ع%0A";

});

message+="%0A🚚 التوصيل: "+
deliveryFee.toLocaleString()+" د.ع";

message+="%0A💰 *المجموع الكلي: "+
(total+deliveryFee).toLocaleString()+" د.ع*";

if(notes){

message+="%0A📝 ملاحظات: "+notes;
}

let phone="9647727071206";

window.open(
"https://wa.me/"+phone+"?text="+message,
"_blank"
);

}

renderCart();

</script>

</body>
</html>