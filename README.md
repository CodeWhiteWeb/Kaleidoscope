# Kaleidoscope
Working Kaleidoscope
-
Tilt your phone or hover with mouse

created using `DeviceOrientationEvent` in js

```js
if (window.DeviceOrientationEvent) {
    window.addEventListener('deviceorientation', function(event) {
        var x = Math.round(event.beta);
        var y = Math.round(event.gamma);
        var factorx = y / $(window).width();
        var factory = x / $(window).height();
        scope.angleTarget = factorx + 2;
        scope.zoomTarget = 0.5 + 4.0 * factory;
    });
}```
