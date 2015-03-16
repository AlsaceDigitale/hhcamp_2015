<div id="map_canvas"></div>
<h3 style="text-align: center;"><a href="https://www.google.com/maps/d/edit?mid=zvONMy3YPLvI.kIohr3SUGc24">MORE INFORMATIONS ON DETAILED MAP WITH BUS, TRAMWAY, HOTELS, PLACES</a></h3>
<div class="row">
  <div class="col-md-6">

<h3>Future of Health and Health Pitch Challenge location</h3>

<p>Auditorium du conservatoire de musique</p>

<p>1, Place Dauphine (near Place de l'étoile)</p>

<p>67000 Strasbourg</p>

<h3>Health Data Day and Health Hackathon</h3>

<p>Faculté de médecine</p>

<p>4, rue kirschleger</p>

<p>67000 Strasbourg</p>

<h3>Further informations</h3>

<p>You wish to have further informations about events or to participate as a developer, a designer, a health professionnal or an entrepreneur ?</p>

<p>Contact our Hacking Health team. We're at your disposal to answer all your questions.</p>

<p>Mail : <a href="mailto:sebastien.letelie@gmail.com" target="_blank">sebastien.letelie@gmail.com</a></p>

<p>Tel : +33 (0)6 24 72 04 96</p>

  </div>
  <div class="col-md-6">

<h3>Hotels suggestions</h3>
<h4>We negociate a discount for Hacking Health Camp attendees for a limited number of rooms. <br>If you book early you can benefit of this discound by telling you come for Hacking Health Camp</h4>

<p><a href="http://www.ibis.com/fr/hotel-1428-ibis-strasbourg-centre-ponts-couverts/index.shtml" target="_blank">Hôtel ibis Strasbourg Centre Ponts Couverts ***</a></p>
<p>7 RUE DE MOLSHEIM - 67000 - STRASBOURG</p>
<p>Tél. : +33 (0)3 90 22 48 70</p>
<p>IMPORTANT : ask to Virginie or Diane for discount</p>

<p><a href="http://www.les-haras-hotel.com/" target="_blank">Hôtel Les Haras ****</a></p>
<p>23, rue des Glacières - 67000 - STRASBOURG</p>
<p>Tel. : +33 (0)3 90 20 50 00</p>

<p><a href="http://www.cour-corbeau.com/" target="_blank">Hôtel Cour du Corbeau ****</a></p>
<p>6-8, rue des Couples - 67000 - STRASBOURG</p>
<p>Tel. : +33 (0)3 90 00 26 26</p>
<p><a href="mailto:info@cour-corbeau.com">info@cour-corbeau.com</a></p>

<p><a href="http://www.cerf-dor-strasbourg.fr/" target="_blank">Hôtel au Cerf d'or ***</a></p>
<p>6 Place de l’Hôpital - 67000 STRASBOURG</p>
<p>Tél. : +33 (0)3 88 36 20 05</p>
<p><a href="mailto:reservation@cerf-dor.com">reservation@cerf-dor.com</a></p>

<p><a href="http://www.dragon.fr/" target="_blank">Hôtel du Dragon ***</a></p>
<p>12 rue du Dragon - 67000 STRASBOURG</p>
<p>Tél. : +33 (0)3 88 35 79 80</p>
<p><a href="mailto:hotel@dragon.fr">hotel@dragon.fr</a></p>

<p><a href="http://www.hotel-beaucour.com/fr/" target="_blank">Hôtel Beaucour</a></p>
<p>5, rue des Bouchers - 67000 STRASBOURG</p>
<p>Tél. : +33 (0)3 88 76 72 00</p>
<p><a href="mailto:info@hotel-beacour.fr">info@hotel-beaucour.fr</a></p>

<!--<p><a href="http://www.hotel-diana-dauphine.com/fr/hotel-3-etoiles-strasbourg.php" target="_blank">Hôtel Diana Dauphine</a></p>
<p>30 Rue de la 1ère Armée - 67000 Strasbourg</p>
<p>Tél. : +33 (0)3 88 36 26 61</p>
<p><a href="mailto:info@hotel-diana-dauphine.com">info@hotel-diana-dauphine.com</a></p>

<p><a href="http://www.hotel-ettenheim-strasbourg.fr/" target="_blank">Hôtel Ettenheim</a></p>
<p>3 place de l’Hôpital - 67000 Strasbourg</p>
<p>Tél. +33 (0)3 88 24 90 70</p>

<p><a href="http://www.holidayinn-strasbourg.fr/" target="_blank">Holliday Inn Strasbourg Centre</a></p>
<p>Rue de la corderie - 67000 Strasbourg  France</p>
<p>Tél. : +33 (0) 388 10 99 99</p>
<p><a href="mailto:contact@holidayinn-strasbourg.fr">contact@holidayinn-strasbourg.fr</a></p>-->

  </div>
</div>

<div id="legend">
    <div>
        <span>Health Data Day & Hackathon</span>

        <h1>Faculté de médecine</h1>

        <h2>4, rue kirschleger <br/>67000 Strasbourg <br/> FRANCE</h2>

    </div>
</div>
<div id="legend2">
    <div>
        <span>Future of Health & Health Pitch Challenge</span>

        <h1>Auditorium du <br/>conservatoire de musique</h1>

        <h2>1 Place Dauphine (near Place de l'étoile)<br/>67000 Strasbourg <br/> FRANCE</h2>

    </div>
</div>


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
