# openCampus2019

<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <title>Picture separator</title>
    <style>
        img {
            width: 600px;

        }
        section{
            display: none;
        }
        h1{
            border-left: solid 10px red;
            border-bottom: solid 2px red;
            padding-left: 5px;
        }
        #secFuji{
            display: block;
        }
        
        .container{
            display: flex;
            flex-direction: row;


        }
        .parts{
            flex-direction: column;
            width: 195px;
            height: 3ex;
            vertical-align: middle;;
            /* border: solid 1px red; */
        }

    </style>
    <script>
        function moveKitadake(){
            var item = document.getElementById( "secFuji");
            item.style.display = "none";
            var item = document.getElementById( "secKitadake");
            item.style.display="block"
        }
        function movesecOkuhodakadake(){
            var item = document.getElementById( "secKitadake");
            item.style.display = "none";
            var item = document.getElementById( "secOkuhodakadake");
            item.style.display="block"

        }
    </script>
</head>

<body>
    <header>
        <h1>JavaScriptで画面を移動 する</h1>

    </header>
    <section id="secFuji">
        <h1>みんなが登りたい富士山</h1>
        <img src="aaa.jpg" alt="Mt.Fuji">
        <div class="container">
            <div class="parts"></div>
            <div class="parts"></div>
            <div class="parts" onclick="moveKitadake()">Next</div>
        </div>
    </section>
    <section id="secKitadake">
        <h1>意外と2番目に高い山は知らない北岳</h1>
        <img src="bbb.jpg" alt="Mt.Kitadake">
        <div class="container">
            <div class="parts">Beofre</div>
            <div class="parts"></div>
            <div class="parts" onclick="movesecOkuhodakadake()">Next</div>
        </div>

    </section>
    <section id="secOkuhodakadake">
        <h1>3番目に高い山は知らないでしょ？奥穂高岳</h1>
        <img src="ccc.jpg" alt="Mt.okuhodaka">
        <div class="container">
            <div class="parts">before</div>
            <div class="parts"></div>
            <div class="parts">Next</div>
        </div>

    </section>
    <section id="secYaridake">
        <h1>山をのぼる人のあこがれ槍岳</h1>
        <img src="ddd.jpg" alt="Mt.Yaridake">
        <div class="container">
            <div class="parts">before</div>
            <div class="parts"></div>
            <div class="parts"></div>
        </div>

    </section>
</body>

</html>
