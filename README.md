<!doctype html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Syria 💌</title>
<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:#ffe4ec;
  font-family:system-ui,-apple-system;
}
.card{
  background:white;
  padding:30px;
  border-radius:20px;
  box-shadow:0 15px 40px rgba(0,0,0,.15);
  text-align:center;
  max-width:320px;
}
.envelope{
  font-size:70px;
  cursor:pointer;
}
.hidden{display:none;}
button{
  margin:10px;
  padding:10px 18px;
  border:none;
  border-radius:12px;
  font-size:16px;
}
.yes{background:#ff4d8d;color:white;}
.no{background:#f3f3f3;}
</style>
</head>
<body>

<div class="card">
  <div class="envelope" onclick="openLetter()">💌</div>
  <div id="letter" class="hidden">
    <div style="font-size:60px;">🧸</div>
    <h2>Syria, will you be my Valentine? 💕</h2>
    <button class="yes" onclick="yes()">Yes 💖</button>
    <button class="no" onclick="no()">No 😭</button>
  </div>
</div>

<script>
function openLetter(){
  document.querySelector('.envelope').style.display='none';
  document.getElementById('letter').classList.remove('hidden');
}
function yes(){
  document.querySelector('.card').innerHTML =
    "<h1>💘 You made me the happiest 💘</h1><div style='font-size:70px'>🧸💐</div>";
}
function no(){
  alert("Try again 😤❤️");
}
</script>

</body>
</html>
