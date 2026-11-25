<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Métodos de búsqueda</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #f1f5f9;
    color: #263445;
    line-height: 1.7;
}

header {
    background: linear-gradient(135deg, #14213d, #2563eb);
    color: white;
    text-align: center;
    padding: 55px 20px;
}

header h1 {
    font-size: 38px;
    margin-bottom: 10px;
}

nav {
    background: #14213d;
    padding: 15px;
    text-align: center;
    position: sticky;
    top: 0;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 12px;
    font-weight: bold;
}

nav a:hover {
    color: #60a5fa;
}

main {
    max-width: 1000px;
    margin: auto;
    padding: 25px;
}

section {
    background: white;
    padding: 25px;
    margin: 25px 0;
    border-radius: 12px;
    box-shadow: 0 3px 12px #00000012;
}

h2 {
    color: #2563eb;
    margin-bottom: 15px;
}

h3 {
    color: #14213d;
    margin-top: 15px;
}

.example {
    background: #eaf2ff;
    padding: 15px;
    border-left: 5px solid #2563eb;
    margin: 15px 0;
    border-radius: 6px;
}

footer {
    background: #14213d;
    color: white;
    text-align: center;
    padding: 25px;
    margin-top: 30px;
}

ul {
    padding-left: 25px;
}
</style>
</head>

<body>

<header>
    <h1>MÉTODOS DE BÚSQUEDA</h1>
    <p>Algoritmos para localizar información de manera eficiente</p>
    <p>Programación y estructuras de datos</p>
</header>

<nav>
    <a href="#secuencial">Secuencial</a>
    <a href="#binaria">Binaria</a>
    <a href="#hash">HASH</a>
    <a href="#conclusion">Conclusión</a>
</nav>

<main>

<section>
    <h2>Introducción</h2>
    <p>
    Los métodos de búsqueda son procedimientos utilizados
    en programación para encontrar datos dentro de una
    colección de elementos. Estos métodos permiten localizar
    información de manera rápida y organizada.
    </p>
</section>

<section id="secuencial">
    <h2>6.1 Búsqueda secuencial</h2>

    <p>
    La búsqueda secuencial consiste en revisar los elementos
    de una lista uno por uno hasta encontrar el dato que
    estamos buscando o llegar al final de la lista.
    </p>

    <h3>Características</h3>
    <ul>
        <li>No necesita que los datos estén ordenados.</li>
        <li>Compara los elementos uno por uno.</li>
        <li>Es sencilla de implementar.</li>
        <li>Puede ser lenta cuando existen muchos elementos.</li>
    </ul>

    <div class="example">
        <h3>Ejemplo:</h3>
        <p>Lista: 10, 20, 30, 40, 50</p>
        <p>Dato buscado: 30</p>
        <p>El algoritmo revisa 10, después 20 y finalmente
        encuentra el 30.</p>
    </div>

    <h3>Ventajas</h3>
    <p>Es fácil de utilizar y funciona con listas ordenadas
    y desordenadas.</p>
</section>

<section id="binaria">
    <h2>6.2 Búsqueda binaria</h2>

    <p>
    La búsqueda binaria es un método que permite encontrar
    un elemento dividiendo una lista ordenada en dos partes.
    En cada paso descarta la mitad de los elementos.
    </p>

    <h3>Características</h3>
    <ul>
        <li>Necesita que los datos estén ordenados.</li>
        <li>Divide la lista en mitades.</li>
        <li>Es más rápida que la búsqueda secuencial en listas grandes.</li>
        <li>Compara el valor buscado con el elemento central.</li>
    </ul>

    <div class="example">
        <h3>Ejemplo:</h3>
        <p>Lista: 10, 20, 30, 40, 50, 60, 70</p>
        <p>Dato buscado: 60</p>
        <p>Primero revisa el número central (40).
        Como 60 es mayor, busca en la mitad derecha.
        Después encuentra el 60.</p>
    </div>

    <h3>Ventajas</h3>
    <p>Reduce considerablemente el número de comparaciones
    y es eficiente para grandes cantidades de datos ordenados.</p>
</section>

<section id="hash">
    <h2>6.3 Búsqueda por funciones de HASH</h2>

    <p>
    La búsqueda mediante funciones HASH utiliza una función
    matemática para transformar una clave en una posición
    dentro de una tabla, facilitando el acceso a los datos.
    </p>

    <h3>Características</h3>
    <ul>
        <li>Utiliza una función HASH.</li>
        <li>Permite acceder directamente a una posición.</li>
        <li>Es muy eficiente en condiciones adecuadas.</li>
        <li>Puede presentar colisiones cuando dos claves
        generan la misma posición.</li>
    </ul>

    <div class="example">
        <h3>Ejemplo:</h3>
        <p>Supongamos que tenemos una tabla HASH de 10 posiciones.</p>
        <p>Clave: 25</p>
        <p>Función: h(clave) = clave % 10</p>
        <p>Resultado: 25 % 10 = 5</p>
        <p>El dato se busca en la posición 5 de la tabla.</p>
    </div>

    <h3>Ventajas</h3>
    <p>Permite buscar información rápidamente sin tener que
    revisar todos los elementos de una lista.</p>
</section>

<section id="conclusion">
    <h2>Conclusión</h2>
    <p>
    Los métodos de búsqueda son fundamentales en la programación
    porque permiten encontrar información de diferentes maneras.
    La búsqueda secuencial revisa los datos uno por uno,
    la binaria divide una lista ordenada en mitades y la búsqueda
    HASH utiliza funciones para acceder a posiciones específicas.
    Cada método tiene características y ventajas que lo hacen
    útil dependiendo del problema que se necesite resolver.
    </p>
</section>

</main>

<footer>
    <p><strong>Alumna:</strong> Debany Camila Rosas Perea</p>
    <p>Actividad: Métodos de búsqueda</p>
    <p>Programación | 2026</p>
</footer>

</body>
</html>
