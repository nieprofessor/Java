<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <title>Wczytaj kolor</title>
</head>
<body>
    <div style="color:red; font-size:50px;">
    </div>
    
    <div id="wynik"></div> 

    <div style="color:green; font-size:45px;">MENU</div>
    <div style="color:red; font-size:45px;">1 - CZERWONY</div>
    <div style="color:blue; font-size:45px;">2- NIEBIESKI</div>
    <input type="button" value="Oblicz" onclick="fun_deb()" />

    


    <script>

        function fun_deb() {
            var x_deb = prompt("Podaj kolor", "");

            if (x_deb == "1" || x_deb.toLowerCase() == "czerwony") {
                document.getElementById("wynik").innerHTML = '<h1 style="color:red;">Wczytałeś kolor czerwony</h1>';
            } 
            else if (x_deb == "2" || x_deb.toLowerCase() == "niebieski") {
                document.getElementById("wynik").innerHTML = '<h1 style="color:blue;">Wczytałeś kolor niebieski</h1>';
            } 
            else {
                document.getElementById("wynik").innerHTML = '<h1 style="color:gray;">Nieznany kolor</h1>';
            }
        }
    </script>
</body>
</html>
