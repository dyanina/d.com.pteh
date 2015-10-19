# d.com.pteh
<!DOCTYPE HTML>
<html>
<head>
<style>
.td {
width: 100px;
height: 70px;
font-size: 20px;
text-align: center;
position: absolute;
}
#area {
position: relative;
height: 260px;
background-color: yellow;
}
#answer {
font-size: 36px;
color: violet;
}
</style>
</head>
<body>
<div id="area">
<input placeholder="Введите массу" id="td11">
<input placeholder="Введите скорость" id="td12">
<input type="button" 
          value="Вычислить импульс" onclick="det()" style="position: absolute; top:50px; left: 0px; width: 150px; height: 50px;">
<span style="position: absolute; top:60px; left:170px;" id = "answer"> Ответ </span>	
</div>
<div>
</div>
</body>
</html>
<script>
function det() {
var m, v, imp;
m = parseInt( document.getElementById("td11").value );
v = parseInt( document.getElementById("td12").value );
imp = m*v;
document.getElementById("answer").innerHTML = 
String( imp );
}
</script>
