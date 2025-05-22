<!DOCTYPE html>
<html lang="PL-pl">
    <meta charset="UTF-8">
    <html> 
        <body> 
        <div style="color:red;font-size:50px;"> 
            <script language="JavaScript"> 
        var x_deb=prompt("podaj liczbę x=",""); 
        var a_deb=parseFloat(x_deb); 
        document.write("czytana liczba x="+a_deb+"<br>");     
            if(a_deb%2==0) 
            {
                document.write("<font color=red size=3>liczba jest parzysta</font>"+"<br>");
            } 

            if(a_deb%2 !== 0) 
            {
                document.write("<font color=silver size=5>liczba jest nieparzysta</font>"+"<br>");
            }
            </script> 
        </div> 
        </body> 
       </html>
</html>
