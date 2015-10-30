<!DOCTYPE html>

<html>

<head>

<title> CURRICULUM VITAE </title>


<link rel="stylesheet" type="text/css" href="bootstrap.css">

<link rel="stylesheet" type="text/css" href="Marcin Midzio-CV.css">


</head>

<body>
<img src="obrazek_1.jpg" width="250" height="300" align="right" alt="Uhhh!..." id="obrazek" />


<script type="text/javascript">
if (document.images) {
    var Image_off = new Image();
    Image_off.src = 'obrazek_1.jpg';

    var Image_on = new Image();
    Image_on.src = 'obrazek_2.jpg';

    var obr = document.getElementById('obrazek');

    obr.onmouseover = function() {
        this.src = Image_on.src
    }
    obr.onmouseout = function() {
        this.src = Image_off.src
    }
}
</script>

<div class="container">
  <div class="jumbotron">
    <h1>Curiculum Vitae</h1>
 </div>
  <div class="row">
    <div class="col-sm-12">
     <h2>Dane Osobowe</h2>
  Imię:Marcin  <br />
  Nazwisko:Midzio <br />
  Data urodzenia:07.09.1994  <br />
  Adres:Grędzice ul.Ogrodowa 4 <br />
  Telefon:794531777 <br />
  E-mail : m.midzio7@gmail.com <br />
</div>
    <div class="col-sm-12">
<h3>Wykształcenie</h3>


2013- obecnie – Studia na kierunku „Informatyka ” w Państwowej
Wyższej Szkole Zawodowej w Ciechanowie <br />

2010-2013 – IV Liceum Ogólnokształcące im.Generała Józefa Bema w
Ciechanowie    <br />

</div>
    <div class="col-sm-12">
<h4>Umiejętnosci</h4>

  Bardzo dobra znajomosc pakietu Office <br />

  Podstawowa wiedza w zakresie C++ i Java <br />

  Znajomosć języka angielskiego – w stopniu dobrym <br />
</div>
    <div class="col-sm-12">

<h5>Dodatkowe Predyspozycje</h5>

  bezwzrokowe pisanie <br />

  praca w zespole <br />

  punktualnosc <br />

  prawo jazdy kat.B <br />

</div>
    <div class="col-sm-12">
<h6>Zainteresowania </h6>

Sport<br />

Muzyka<br />

Film<br />

Jazda na rowerze<br />

</div>
    <div class="col-sm-6">
 </div>
  </div>
</div>
</body>

<div id="fCzas"></div>
<div id="fData"></div>
<center>
<script type="text/javascript">
function zeroWiodace(i) {
    return (i < 10)? '0'+i : i;
}

function pokaz_czas() {
    var czas = new Date();
    var dni = new Array("Niedziela", "Poniedziałek", "Wtorek", "¦roda", "Czwartek", "Piatek", "Sobota");
    var data = zeroWiodace(czas.getDate()) + "." + zeroWiodace((czas.getMonth()+1)) + "." + czas.getFullYear() + " - " + dni[czas.getDay()];
    var czas_na_zegarku = zeroWiodace(czas.getHours()) + ":" + zeroWiodace(czas.getMinutes()) + ":" + zeroWiodace(czas.getSeconds());

    document.getElementById('fCzas').innerHTML = czas_na_zegarku
    document.getElementById('fData').innerHTML = data;

    setTimeout("pokaz_czas()",1000)
}

pokaz_czas();
</script>
</center>

</html>
