
<head>
    <meta charset="UTF-8">
    <meta http-equiv="Page-Enter" content="blendTrans(Duration=1.0)">
    <meta http-equiv="Page-Exit" content="blendTrans(Duration=1.0)">
    <title>Главная страница</title>
</head>
<body background="https://www.transparenttextures.com/patterns/white-wall-3.png" style="margin:20px;">

<center>
<h1><u>Добро пожаловать на сайт</u></h1>
</center>

<hr size="2" color="black">

<font size="5"><b>О сайте</b></font><br><br>
<font size="4">Этот сайт создан в учебных целях.</font><br>
<font size="3">Здесь собрана информация, таблицы, списки и другие элементы.</font><br>
<font size="2">Используйте меню для навигации между страницами.</font>

<hr size="2" color="black">

<div style="border:1px solid gray; padding:10px; margin:10px; background:#f0f0f0;">
Последнее обновление: <span id="date"></span>
</div>

<script>
document.getElementById("date").innerHTML = new Date().toLocaleDateString("ru-RU");
</script>

<ol type="I">
<li>Главная страница</li>
<li>Медиа страница</li>
<li>Анкета</li>
</ol>

<table align="center" border="4" cellpadding="10" cellspacing="0" background="https://www.transparenttextures.com/patterns/soft-wallpaper.png">
<tr>
<th colspan="3"><font size="4">Заголовок таблицы</font></th>
</tr>
<tr align="center">
<td>Ячейка 2-1</td>
<td>Ячейка 2-2</td>
<td>Ячейка 2-3</td>
</tr>
<tr align="center">
<td>Ячейка 3-1</td>
<td>Ячейка 3-2</td>
<td>Ячейка 3-3</td>
</tr>
<tr align="center">
<td>Ячейка 4-1</td>
<td>Ячейка 4-2</td>
<td>Ячейка 4-3</td>
</tr>
</table>

<br>

<center>
<div style="border:2px solid black; padding:10px; width:200px; background:lightyellow;">
Счётчик посещений:<br>
<span id="counter">0</span>
</div>
</center>

<script>
if (localStorage.getItem("visits")) {
    var count = parseInt(localStorage.getItem("visits")) + 1;
} else {
    var count = 1;
}
localStorage.setItem("visits", count);
document.getElementById("counter").innerHTML = count;
</script>

<br><br>

<center>
<a href="page2.html">Страница 2 (Медиа)</a> &nbsp;|&nbsp;
<a href="page3.html">Страница 3 (Анкета)</a>
</center>

</body>
</html>
