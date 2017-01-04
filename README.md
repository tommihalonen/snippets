# snippets
Code snippets for quick access

## custom Google Map
```html
<script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY"></script>
<script>
  var map = new google.maps.Map(
    document.getElementById('map'),
    {
      zoom: 15,
      center: { lat: 123.4567, lng: 123.4567 },
      disableDefaultUI: true,
      styles: [
        {"featureType":"landscape.man_made","elementType":"all","stylers":[{"color":"#faf5ed"},{"lightness":"0"},{"gamma":"1"}]},
        {"featureType":"poi.park","elementType":"geometry.fill","stylers":[{"color":"#bae5a6"}]},
        {"featureType":"road","elementType":"all","stylers":[{"weight":"1.00"},{"gamma":"1.8"},{"saturation":"0"}]},
        {"featureType":"road","elementType":"geometry.fill","stylers":[{"hue":"#ffb200"}]},
        {"featureType":"road.arterial","elementType":"geometry.fill","stylers":[{"lightness":"0"},{"gamma":"1"}]},
        {"featureType":"transit.station.airport","elementType":"all","stylers":[{"hue":"#b000ff"},{"saturation":"23"},{"lightness":"-4"},{"gamma":"0.80"}]},
        {"featureType":"water","elementType":"all","stylers":[{"color":"#a0daf2"}]}
      ]
    }
  );

  var marker = new google.maps.Marker({
    position: { lat: 123.4567, lng: 123.4567 },
    map: map,
    icon: location.protocol + '//' + location.host + '/wp-content/themes/xxx/img/marker.png'
  });
</script>
```
