<!DOCTYPE html>
<html lang="PL-pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zadanie 20</title>
</head>
<body>
    <h1>Oblicz długości boków trójkąta</h1>
    <form onsubmit="event.preventDefault(); calculateDistances()">
        <label>A(x): <input type="numer" id="xa_deb"></label><br>
        <label>A(y): <input type="numer" id="ya_deb"></label><br>
        <label>B(x): <input type="numer" id="xb_deb"></label><br>
        <label>B(y): <input type="numer" id="yb_deb"></label><br>
        <label>C(x): <input type="numer" id="xc_deb"></label><br>
        <label>C(y): <input type="numer" id="yc_deb"></label><br>
        <button type="submit">Oblicz</button>
    </form>

    <h2>Wyniki:</h2>
    <p id="sumaAB"></p>
    <p id="sumaBC"></p>
    <p id="sumaAC"></p>

    <script>
        function calculateDistance(x1, y1, x2, y2) {
            return Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2));
        }

        function calculateDistances() {
            const xa = +document.getElementById('xa_deb').value;
            const ya = +document.getElementById('ya_deb').value;
            const xb = +document.getElementById('xb_deb').value;
            const yb = +document.getElementById('yb_deb').value;
            const xc = +document.getElementById('xc_deb').value;
            const yc = +document.getElementById('yc_deb').value;

            const AB = calculateDistance(xa, ya, xb, yb);
            const BC = calculateDistance(xb, yb, xc, yc);
            const AC = calculateDistance(xa, ya, xc, yc);

            document.getElementById('sumaAB').textContent = `AB: ${AB.toFixed(2)}`;
            document.getElementById('sumaBC').textContent = `BC: ${BC.toFixed(2)}`;
            document.getElementById('sumaAC').textContent = `AC: ${AC.toFixed(2)}`;
        }
    </script>
</body>
</html>
