body {
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
margin: 0;
font-family: Arial, Helvetica, sans-serif;
8
10
.form
11
text-align: center;
12
13
.container(
14
display: flex;
15
margin-bottom: 10px;
16
align-items: center;
17
gap: 30px;
18
19
button{
width: 200px;
height: 30px;




// Функция получения данных из эмулятора
v function getData ()(
fetch("http://localhost:4444/TransferSimulator/fullName")
.then(responce => responce.]son())
.then (data => document. querySelector"-FIO"). textContent = data.value)
document. querySelector("-result"). textContent - "...";
8
Функция
проверки данных по регулярному выражению
function
validateData() (
10
let
name
= document-querySelector(" FIO"). textContent.trim();
11
let regex = /^[A-яё\s]+$/;
12
document.queryselector result").textContent = regex. test(name) ? "Данные корректы" : "ФИО содер»
13

index.html > @html body
<DOCTYPE htm>
‹html lang="ru">
<head>
<meta charset="UTF-8">
‹meta name="viewport"
‹link rel="stylesheet" href="style.css"›
</head>
<body>
<! -- Основная форма
‹div class="form">
‹div class="container"›
‹button onclick="getData() ›Получить данные</button>
‹p class="FIO">...</p>
</div>
‹div class="container">
‹p class="result"›...</p>
</div>
</div>
‹script src="scripts. js"›/script>
</ body>
</html>