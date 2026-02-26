<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tienda de Frutos Secos</title>
<style>
body{
    font-family: Arial, sans-serif;
    margin:0;
    background-color:#f5f5f5;
}
header{
    background-color:#8B4513;
    color:white;
    padding:20px;
    text-align:center;
}
.container{
    width:90%;
    max-width:1000px;
    margin:auto;
    padding:20px;
}
.productos{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(200px,1fr));
    gap:20px;
}
.card{
    background:white;
    padding:15px;
    border-radius:10px;
    box-shadow:0 4px 8px rgba(0,0,0,0.1);
    text-align:center;
}
button{
    background-color:#8B4513;
    color:white;
    border:none;
    padding:10px;
    border-radius:5px;
    cursor:pointer;
}
button:hover{
    background-color:#5c2e0e;
}
.formulario{
    background:white;
    padding:20px;
    border-radius:10px;
    margin-top:30px;
    box-shadow:0 4px 8px rgba(0,0,0,0.1);
}
input{
    width:100%;
    padding:8px;
    margin:8px 0;
}
footer{
    background:#333;
    color:white;
    text-align:center;
    padding:15px;
    margin-top:30px;
}
</style>
</head>

<body>

<header>
<h1>Tienda Natural - Frutos Secos</h1>
<p>Compra saludable y segura</p>
</header>

<div class="container">

<h2>Nuestros Productos</h2>

<div class="productos">

<div class="card">
<h3>Almendras</h3>
<p>$5.00</p>
<button onclick="alert('Producto agregado al carrito')">Agregar</button>
</div>

<div class="card">
<h3>Nueces</h3>
<p>$6.50</p>
<button onclick="alert('Producto agregado al carrito')">Agregar</button>
</div>

<div class="card">
<h3>Maní</h3>
<p>$3.00</p>
<button onclick="alert('Producto agregado al carrito')">Agregar</button>
</div>

<div class="card">
<h3>Pistachos</h3>
<p>$7.00</p>
<button onclick="alert('Producto agregado al carrito')">Agregar</button>
</div>

</div>

<div class="formulario">
<h2>Pago con Tarjeta</h2>

<form onsubmit="return pagar()">
<label>Nombre del titular</label>
<input type="text" required>

<label>Número de tarjeta</label>
<input type="text" maxlength="16" required>

<label>Fecha de vencimiento</label>
<input type="month" required>

<label>CVV</label>
<input type="password" maxlength="3" required>

<button type="submit">Pagar</button>
</form>
</div>

</div>

<footer>
<p>© 2026 Tienda Natural - Frutos Secos</p>
</footer>

<script>
function pagar(){
    alert("Pago procesado (simulación). Gracias por su compra.");
    return false;
}
</script>

</body>
</html>
