# treygolnik
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Аляска.</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<!--
   Подключаем API карт 2.x
    Параметры:
      - load=package.full - полная сборка;
      - lang=ru-RU - язык русский.
      -->
<script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
type="text/javascript"></script>
<script type="text/javascript">
// Как только будет загружен API и готов DOM, выполняем инициализацию
ymaps.ready(init);
    function init() {
    var myMap = new ymaps.Map('map', {
        center: [65.171457, -152.076289],
        zoom: 8
});
 var myPolygon = new ymaps.Polygon([
 [
     [65.64, -152.43],
      
       [65.46, -152.50],
   
       [65.46, -152.27]
        ]
    ],
 {
 hintContent: "Многоугольник"
    }, {
 fillColor: '#00FF0088',
strokeWidth: 0.5
 });
 myMap.geoObjects.add(myPolygon);
}

</script>
</head>
<body>
<h2>Аляска</h2>
<div id="map" style="width:600px;height:400px"></div>
</body>
</html>
