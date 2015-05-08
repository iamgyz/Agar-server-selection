# Agar-server-selection
Allow you to specify your server IP

### Usage  
For Chrome:  
Open "Javascript Console" and paste the following code

```javascript
(function() {
    var _ws = window.WebSocket;
    window.WebSocket = function(url) {
        url = prompt("Hi!I am GY!\nYou can specify your server  here!",url)
        if(!url) url = 'ws://106.184.7.253:443'
        console.log('Hi!I am GY, I will redirect you to my specific server '+url);
        return (new _ws(url));
    };
})();
```

Have fun with your friends!!
