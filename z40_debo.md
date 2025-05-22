<!DOCTYPE html> 
<html lang="pl"> 
<head> 
 <title>Zadanie JavaScript</title> 
 <meta charset="utf-8"> 
 <style> 
  h1 { text-transform: uppercase; } 
  
 </style> 
</head> 
<body> 
 
 <h1>Proste działania</h1> 
 <br><br>
 <h1>Szymon Dębowski 3G</h1>
 <label for="a">Podaj pierwszą liczbę:</label> <input type="number" id="a"> 
 <br><br> 
 <label for="b">Podaj drugą liczbę:</label> <input type="number" id="b"> 
 <br><br> 
 <input type="button" value="DODAWANIE" onclick="suma()"> 
 <input type="button" value="ODEJMOWANIE" onclick="roznica()"> 
 <input type="button" value="MNOŻENIE" onclick="iloczyn()"> 
 <input type="button" value="DZIELENIE" onclick="iloraz()"> 
 <input type="button" value="TEORIA-Dębowski" onclick="teoria_deb()"> 
 <div id="wynik" style="margin-top:20px;"></div> 
 <script> 
  function suma() 
  { 
   var a = document.getElementById("a").value; 
   var b = document.getElementById("b").value; 
   if (a == "" || b == "") 
   { 
   document.getElementById("wynik").innerHTML = "Proszę uzupełnić obie liczby."; 
   } else 
   { 
    a = parseFloat(a); 
    b = parseFloat(b); 
    var suma = a + b; 
  document.getElementById("wynik").innerHTML = "Wynik działania wynosi: " + suma; 
   } 
  } 
  function roznica() 
  { 
   var a = document.getElementById("a").value; 
   var b = document.getElementById("b").value; 
   if (a == "" || b == "") 
   { 
  document.getElementById("wynik").innerHTML = "Proszę uzupełnić obie liczby."; 
   } else 
   { 
    a = parseFloat(a); 
    b = parseFloat(b); 
    var roznica = a - b; 
  document.getElementById("wynik").innerHTML = "Wynik działania wynosi: " + roznica; 
   } 
  } 
  function iloczyn() 
  { 
   var a = document.getElementById("a").value; 
   var b = document.getElementById("b").value; 
   if (a == "" || b == "") 
   { 
  document.getElementById("wynik").innerHTML = "Proszę uzupełnić obie liczby."; 
   } else 
   { 
    a = parseFloat(a); 
    b = parseFloat(b); 
    var iloczyn = a * b; 
  document.getElementById("wynik").innerHTML = "Wynik działania wynosi: " + iloczyn; 
   } 
  }   
 
  function iloraz() 
  { 
   var a = document.getElementById("a").value; 
   var b = document.getElementById("b").value; 
   if (a == "" || b == "") 
   { 
  document.getElementById("wynik").innerHTML = "Proszę uzupełnić obie liczby."; 
   } else 
   { 
    a = parseFloat(a); 
    b = parseFloat(b); 
    if (b == 0) 
    { 
  document.getElementById("wynik").innerHTML = "Nie wolno dzielić przez zero."; 
    } 
    else 
    {         
     var iloraz = a / b; 
  document.getElementById("wynik").innerHTML = "Wynik działania wynosi: " + iloraz; 
    } 
   } 
    }
   function teoria_kol()
    { 
    document.write("<font color=red size=4>&lt;"+"label for=&quot"+"a"+"&quot;"+"&gt;&quot;" + "Podaj pierwszą liczbę:" + "&lt;"+"/label"+"&gt;" + "&lt;"+"input type="+"&quot;" + "number"+"&quot;" + "id="+"&quot;" + "a"+"&quot;"+"&gt;" + "</font><br>");  
    document.write("<font color='red' size='4'>" + "&lt;" + "input type='button' value='DODAWANIE' onclick='suma()'&gt;" + "</font><br>");
    document.write("<font color='red' size='4'>" + "var a = document.getElementById('a').value;" + "</font><br>");
    document.write("<font color='red' size='4'>" + "if (a == '' || b == '')" + "" + "</font><br>");
    document.write("<font color='red' size='4'>" + "document.getElementById('wynik').innerHTML = 'Wynik działania wynosi: ' + suma;" + "</font><br>");
    } 
 </script> 
</body> 
</html> 
