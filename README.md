tinyxhr
=======

tinyxhr by Shimon Doodkin - licanse: public doamin - https://gist.github.com/4706967

```
var xhr = require("tinyxhr");
```

```
xhr("http://site.com/ajaxaction", function (err,data,xhr){ 
  if (err) {
    console.log("goterr ",err,'status='+xhr.status); 
    console.log(data);
  }
});
```

```
xhr("http://site.com/ajaxaction", function (err,data,xhr){ 
  if (err) {
    console.log("goterr ",err,'status='+xhr.status);
    console.log(data);
  }
}, 'POST', 'value1=1&value2=2');
```

```
xhr("http://site.com/ajaxaction.json", function (err,data,xhr){ 
  if (err) {
    console.log("goterr ",err,'status='+xhr.status); 
    console.log(data); console.log(JSON.parse(data));
  }
}, 'POST', JSON.stringify({value:1}), 'application/javascript');
```
