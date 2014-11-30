<div class="row">
  <div class="col-md-6">

<h3>Future of Health and Health Pitch Challenge location</h3>

<p>Auditorium du conservatoire de musique</p>

<p>Place de l'étoile</p>

<p>67000 Strasbourg</p>

<h3>Health Data Day and Health Hackathon</h3>

<p>Faculté de médecine</p>

<p>1, rue Humann</p>

<p>67000 Strasbourg</p>

  </div>
  <div class="col-md-6">

<h3>Hotels suggestions</h3>

<p><a href="http://www.ibis.com/fr/hotel-1428-ibis-strasbourg-centre-ponts-couverts/index.shtml" target="_blank">Hôtel ibis Strasbourg Centre Ponts Couverts</a></p>

<p>7 RUE DE MOLSHEIM - 67000 - STRASBOURG</p>

<p>TEL : +33 (0)3 90 22 48 70 - FAX : +33 (0)3 90 22 48 60</p>

<p><a href="http://www.les-haras-hotel.com/" target="_blank">Hôtel Les Haras ****</a></p>

<p>23, rue des Glacières - 67000 - STRASBOURG</p>

<p>Tel. : +33 (0)3 90 20 50 00 - Fax : +33 (0)3 90 20 50 10</p>

  </div>
</div>

<div id="legend">
    <div>
        <span>Health Data Day & Hackathon</span>

        <h1>Faculté de médecine</h1>

        <h2>1, rue Humann <br/>67000 Strasbourg <br/> FRANCE</h2>

    </div>
</div>
<div id="legend2">
    <div>
        <span>Future of Health & Health Pitch Challenge</span>

        <h1>Auditorium du <br/>conservatoire de musique</h1>

        <h2>Place de l'étoile <br/>67000 Strasbourg <br/> FRANCE</h2>

    </div>
</div>
<div id="map_canvas"></div>

###Further informations

You wish to have further informations about events or to participate as a developer, a designer, a health professionnal or an entrepreneur ?

Contact our Hacking Health team. We're at your disposal to answer all your questions.

Mail : <a href="mailto:s.letelie@hackinghealth.ca" target="_blank">s.letelie@hackinghealth.ca</a>

Tel : 00 336 24 72 04 96

<script src="https://maps.googleapis.com/maps/api/js"></script>
<script>
  function initialize() {
    var map_canvas = document.getElementById('map_canvas');
    var map_options = {
      center: new google.maps.LatLng(48.5778309,7.7410011),
      zoom: 14,
      mapTypeId: google.maps.MapTypeId.ROADMAP
    }
    var map = new google.maps.Map(map_canvas, map_options);
    new google.maps.Marker({
      position: new google.maps.LatLng(48.576504,7.739521),
      icon: 'img/location.png',
      map: map
    });
    new google.maps.Marker({
      position: new google.maps.LatLng(48.574381,7.755759),
      icon: 'img/location.png',
      map: map
    });
    map.controls[google.maps.ControlPosition.TOP_LEFT].push(document.getElementById('legend'));
    map.controls[google.maps.ControlPosition.TOP_RIGHT].push(document.getElementById('legend2'));
  }
  google.maps.event.addDomListener(window, 'load', initialize);
</script>
