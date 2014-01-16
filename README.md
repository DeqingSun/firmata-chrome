firmata-chrome
==============

Chrome extension to connect to an arduino that's been loaded with firmata.  

You can click a checkbox on a pin to send output.

Enable (chrome://flags/#debug-packed-apps) so you can use dev tools to access the arduino board directly.

Once you're connected, you can use chrome's console to set a pin to INPUT and listen for input events:

```javascript
board.digitalRead(2, function (value) {
  if(value == 1){ 
    console.log('Hello Pin 2!');
  }
});

```
