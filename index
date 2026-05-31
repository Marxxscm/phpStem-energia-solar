<!DOCTYPE html>
<html lang="es-mx">
<head>
<meta charset="UTF-8">
<title>Práctica 12-Gpo XB</title>
<link rel="stylesheet" href="css/estilos.css"/>
<link rel="stylesheet" href="css/menu.css"/>
<link rel="stylesheet" href="css/problemas.css"/>
<link href="https://fonts.googleapis.com/css?family=Rambla" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Comfortaa" rel="stylesheet">
</head>
<body>
<section class="wrapper">
<header>
  <h1 class="logo"><a href="index.php">phpStem</a></h1>
  <nav>
    <ul>
      <li><a href="index.php" class="current">Inicio</a></li>
      <li><a href="acercade.php">Acerca de</a></li>
    </ul>
  </nav>
</header>

<section id="contenedor">

  <section class="problema">
    <h2>Problema: Calcular la energía generada por un panel solar</h2>
    <p>Descripción:</p>
    <p>Un panel solar tiene un área de 2 m², una eficiencia del 18% y recibe una
    irradiancia solar de 1000 W/m².<br>
    a) ¿Cuánta potencia eléctrica genera el panel?<br>
    b) Si opera 6 horas al día, ¿cuánta energía produce diariamente (en Wh y kWh)?<br>
    c) Si la eficiencia se reduce a la mitad, ¿cuál sería la potencia generada?</p>
  </section>

  <section class="formulas">
    <h2>Fórmulas</h2>
    Potencia (W) = Irradiancia (W/m²) × Área (m²) × Eficiencia<br>
    Energía diaria (Wh) = Potencia (W) × Horas de operación<br>
    Energía diaria (kWh) = Energía (Wh) / 1000
  </section>

  <section class="datos">
    <h2>Datos:</h2>
    Irradiancia = 1000 W/m²<br>
    Área = 2 m²<br>
    Eficiencia = 18% (0.18)<br>
    Horas de operación = 6 h/día
  </section>

  <section class="calculos">
    <h2>Solución</h2>
    <p>a) Potencia = 1000 W/m² × 2 m² × 0.18</p>
    <p>b) Energía diaria = Potencia × 6 horas</p>
    <p>c) Potencia con eficiencia reducida = 1000 × 2 × 0.09</p>
  </section>

<?php
function calcula_energia_solar() {
    $irradiancia  = 1000;
    $area         = 2;
    $eficiencia   = 0.18;
    $horas        = 6;

    $potencia     = $irradiancia * $area * $eficiencia;
    $energia_wh   = $potencia * $horas;
    $energia_kwh  = $energia_wh / 1000;
    $potencia_mit = $irradiancia * $area * ($eficiencia / 2);

    return [
        'potencia'     => $potencia,
        'energia_wh'   => $energia_wh,
        'energia_kwh'  => $energia_kwh,
        'potencia_mit' => $potencia_mit
    ];
}

$resultado = calcula_energia_solar();
?>

  <section class="resultado">
    <h2>Resultado:</h2>
    <?php
    echo "<p>a) Potencia generada: <strong>" . $resultado['potencia'] . " W</strong></p>";
    echo "<p>b) Energía diaria: <strong>" . $resultado['energia_wh'] . " Wh</strong> ("
         . $resultado['energia_kwh'] . " kWh)</p>";
    echo "<p>c) Potencia con eficiencia al 9%: <strong>" . $resultado['potencia_mit'] . " W</strong></p>";
    ?>
  </section>

</section>

<footer class="pie">
  Creative Commons versión 3.0 SciSoft 2025
</footer>
</section>
</body>
</html>
