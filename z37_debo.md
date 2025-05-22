<!DOCTYPE html>
<html lang="PL-pl">
    <meta charset="UTF-8">
    <html> 
        <body> 
        <div style="color:red;font-size:50px;"> 
            <script language="JavaScript"> 
        

        document.write("Czy wiesz od którego roku jest używany JavaScript?"+"<br>");

        var rok_deb=prompt("Czy wiesz od którego roku jest używany JavaScript?=",""); 
        var a_deb=parseFloat(rok_deb);

        document.write("Wczytany rok: "+a_deb+"<br>");

        if(rok_deb==1995)
        {
                document.write("<font color=blue size=4>Brawo znasz rok od kiedy działa JavaScript</font>"+"<br>")
                
        }
        else
        {
                document.write("<font color=red size=7>Źle musisz jeszcze poczytać</font>"+"<br>")
        }
                
            </script> 
        </div> 
        </body> 
       </html>
</html>
