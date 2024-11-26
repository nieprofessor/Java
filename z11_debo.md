<html>
<body bgcolor="yellow">
<div style="color:red;font-size:50px;">
<script language="JavaScript">

var liczba1=prompt("Dzien1=","");
var liczba2=prompt("Dzien2=","");
var ile_sekund_deb;

var D1_deb=parseFloat(liczba1);
var D2_deb=parseFloat(liczba2);

ile_sekund_deb=(D1_deb-D2_deb)*24*3600;

document.write("Dzien1=" +D1_deb+"<br>");
document.write("Dzien2=" +D2_deb+"<br>");
document.write("Sekund=" +ile_sekund_deb+" sek"+"<br>");

</script>
</div>
</body>
</html>
