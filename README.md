<!DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GMZ - Multisserviços</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Garamond, serif;
}

body{
    background:#f5f7fa;
    color:#222;
}

/* MENU */
header{
    width:100%;
    background:#0f172a;
    color:white;
    padding:15px 40px;
    position:fixed;
    top:0;
    z-index:1000;
    display:flex;
    justify-content:space-between;
    align-items:center;
    box-shadow:0 2px 10px rgba(0,0,0,0.2);
}

.logo{
    font-size:30px;
    font-weight:bold;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:25px;
    font-size:18px;
    transition:0.3s;
}

nav a:hover{
    color:#38bdf8;
}

/* HERO */
.hero{
    width:100%;
    height:100vh;
    background:
    linear-gradient(rgba(0,0,0,0.65), rgba(0,0,0,0.65)),
    url('https://images.unsplash.com/photo-1504307651254-35680f356dfd?auto=format&fit=crop&w=1400&q=80');
    background-size:cover;
    background-position:center;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    padding:20px;
}

.hero-content h1{
    font-size:70px;
    margin-bottom:20px;
}

.hero-content p{
    font-size:24px;
    margin-bottom:35px;
}

.btn{
    display:inline-block;
    padding:15px 35px;
    background:#38bdf8;
    color:white;
    text-decoration:none;
    border-radius:10px;
    font-size:20px;
    transition:0.3s;
}

.btn:hover{
    background:#0284c7;
}

/* SERVIÇOS */
.services{
    padding:100px 40px;
    text-align:center;
}

.section-title{
    font-size:50px;
    margin-bottom:50px;
    color:#0f172a;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.card{
    background:white;
    padding:35px;
    border-radius:18px;
    box-shadow:0 5px 20px rgba(0,0,0,0.1);
    transition:0.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card h3{
    margin:20px 0;
    font-size:30px;
    color:#0f172a;
}

.card p{
    font-size:18px;
    color:#555;
}

.icon{
    font-size:60px;
}

/* GALERIA */
.gallery{
    padding:100px 40px;
    background:#e2e8f0;
    text-align:center;
}

.gallery-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:20px;
}

.gallery img{
    width:100%;
    height:250px;
    object-fit:cover;
    border-radius:15px;
    transition:0.4s;
}

.gallery img:hover{
    transform:scale(1.03);
}

/* TABELA */
.pricing{
    padding:100px 40px;
    text-align:center;
}

table{
    width:100%;
    border-collapse:collapse;
    margin-top:40px;
    background:white;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

table th{
    background:#0f172a;
    color:white;
    padding:18px;
    font-size:22px;
}

table td{
    padding:18px;
    border-bottom:1px solid #ddd;
    font-size:18px;
}

/* SOBRE */
.about{
    background:#0f172a;
    color:white;
    padding:100px 40px;
    text-align:center;
}

.about p{
    max-width:900px;
    margin:auto;
    font-size:22px;
    line-height:1.8;
}

/* CONTACTO */
.contact{
    padding:100px 40px;
    text-align:center;
}

form{
    max-width:700px;
    margin:auto;
}

input,
textarea{
    width:100%;
    padding:18px;
    margin-top:20px;
    border:none;
    border-radius:10px;
    background:#e2e8f0;
    font-size:18px;
}

textarea{
    height:180px;
}

button{
    margin-top:20px;
    padding:15px 40px;
    border:none;
    background:#0f172a;
    color:white;
    font-size:20px;
    border-radius:10px;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    background:#1e293b;
}

/* RODAPÉ */
footer{
    background:#020617;
    color:white;
    text-align:center;
    padding:30px;
    font-size:18px;
}

/* WHATSAPP */
.whatsapp{
    position:fixed;
    bottom:20px;
    right:20px;
    background:#25D366;
    color:white;
    width:70px;
    height:70px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:35px;
    text-decoration:none;
    box-shadow:0 4px 15px rgba(0,0,0,0.3);
}

/* RESPONSIVO */
@media(max-width:768px){

header{
    flex-direction:column;
}

nav{
    margin-top:10px;
}

.hero-content h1{
    font-size:45px;
}

.hero-content p{
    font-size:20px;
}

.section-title{
    font-size:38px;
}

}

</style>
</head>
<body>

<!-- MENU -->
<header>

<div class="logo">GMZ - Multisserviços</div>

<nav>
<a href="#inicio">Início</a>
<a href="#servicos">Serviços</a>
<a href="#galeria">Galeria</a>
<a href="#precos">Preços</a>
<a href="#sobre">Sobre</a>
<a href="#contacto">Contacto</a>
</nav>

</header>

<!-- HERO -->
<section class="hero" id="inicio">

<div class="hero-content">
<h1>GMZ - Multisserviços</h1>

<p>
Soluções modernas em instalação residencial,
electrobombas, antenas parabólicas e venda de roupas.
</p>

<a href="#contacto" class="btn">Solicitar Serviço</a>
</div>

</section>

<!-- SERVIÇOS -->
<section class="services" id="servicos">

<h2 class="section-title">Nossos Serviços</h2>

<div class="cards">

<div class="card">
<div class="icon">👕</div>
<h3>Venda de Roupa</h3>
<p>
Roupas modernas e elegantes para homens,
mulheres e crianças.
</p>
</div>

<div class="card">
<div class="icon">🏠</div>
<h3>Instalação Residencial</h3>
<p>
Instalações eléctricas profissionais para
residências e escritórios.
</p>
</div>

<div class="card">
<div class="icon">📡</div>
<h3>Antenas Parabólicas</h3>
<p>
Montagem e alinhamento de antenas
com alta qualidade.
</p>
</div>

<div class="card">
<div class="icon">💧</div>
<h3>Electrobombas</h3>
<p>
Instalação e manutenção de electrobombas.
</p>
</div>

</div>

</section>

<!-- GALERIA -->
<section class="gallery" id="galeria">

<h2 class="section-title">Galeria</h2>

<div class="gallery-container">

<img src="https://images.unsplash.com/photo-1520607162513-77705c0f0d4a?auto=format&fit=crop&w=900&q=80">

<img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=900&q=80">

<img src="https://images.unsplash.com/photo-1516321497487-e288fb19713f?auto=format&fit=crop&w=900&q=80">

</div>

</section>

<!-- PREÇOS -->
<section class="pricing" id="precos">

<h2 class="section-title">Tabela de Preços</h2>

<table>

<tr>
<th>Serviço</th>
<th>Preço</th>
</tr>

<tr>
<td>Instalação Residencial</td>
<td>1500 MT</td>
</tr>

<tr>
<td>Montagem de Antena</td>
<td>2500 MT</td>
</tr>

<tr>
<td>Instalação de Electrobomba</td>
<td>3500 MT</td>
</tr>

<tr>
<td>Venda de Roupa</td>
<td>Consultar</td>
</tr>

</table>

</section>

<!-- SOBRE -->
<section class="about" id="sobre">

<h2 class="section-title">Sobre a Empresa</h2>

<p>
A GMZ - Multisserviços é uma Mini-mpresa especializada em
serviços técnicos e comerciais, oferecendo soluções modernas,
seguras e profissionais para residências e empresas.
Nosso objectivo é garantir qualidade, confiança e satisfação
a todos os clientes.
</p>

</section>

<!-- CONTACTO -->
<section class="contact" id="contacto">

<h2 class="section-title">Entre em Contacto</h2>

<form>

<input type="text" placeholder="Seu Nome" required>

<input type="email" placeholder="Seu Email" required>

<input type="text" placeholder="Seu Número">

<textarea placeholder="Escreva sua mensagem"></textarea>

<button type="submit">Enviar Mensagem</button>

</form>

</section>

<!-- WHATSAPP -->
<a class="whatsapp" href="https://wa.me/258877527323" target="_blank">
☎
</a>

<!-- RODAPÉ -->
<footer>

© 2026 GMZ - Multisserviços | Todos os direitos reservados.

</footer>

</body>
</html>
