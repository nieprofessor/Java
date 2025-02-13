<!DOCTYPE html>
<html>
<head>
    <title>zadanie 32 Szymon Dębowski</title>
    <script type="text/javascript">
        function Wazon(kolor, wysokosc, material) {
            this.kolor = kolor;
            this.wysokosc = wysokosc;
            this.material = material;
        }
        
        Wazon.prototype.wazon_wyswietl_debowski = function () {
            document.write("Obiekt: Wazon<br>");
            document.write("Pola:<br>");
            document.write("- Kolor: " + this.kolor + "<br>");
            document.write("- Wysokość: " + this.wysokosc + "<br>");
            document.write("- Materiał: " + this.material + "<br>");
            document.write("Metoda: wazon_wyswietl_debowski<br>");
        };
        
        var wazon1 = new Wazon('Niebieski', '30 cm', 'Ceramika');
        var wazon2 = new Wazon('Czerwony', '25 cm', 'Szkło');
        var wazon3 = new Wazon('Zielony', '40 cm', 'Porcelana');
        
        wazon1.wazon_wyswietl_debowski();
        wazon2.wazon_wyswietl_debowski();
        wazon3.wazon_wyswietl_debowski();
        
      
        Wazon.prototype.styl = 'Klasyczny';
        
   
        Wazon.prototype.wazon_pokaz_debowski = function () {
            document.write("Nowe pole: Styl - " + this.styl + "<br>");
            document.write("Nowa metoda: wazon_pokaz_debowski<br>");
        };
        
        wazon1.wazon_pokaz_debowski();
        wazon2.wazon_pokaz_debowski();
        wazon3.wazon_pokaz_debowski();
    </script>
</head>
<body>
    <br>
    Programowanie obiektowe. <br>
    Obiekt to Wazon<br>
    Pola:<br>
    Kolor<br>
    Wysokość<br>
    Materiał<br>
    Metoda: wazon_wyswietl_debowski<br>
    Nowe pole: Styl<br>
    Nowa metoda: wazon_pokaz_debowski<br>
</body>
</html>
