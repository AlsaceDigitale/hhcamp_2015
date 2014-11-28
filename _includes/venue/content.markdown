
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
