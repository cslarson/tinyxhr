tinyxhr
=======

tinyxhr by Shimon Doodkin - licanse: public doamin - https://gist.github.com/4706967

tinyxhr("http://site.com/ajaxaction",function (err,data,xhr){ if (err) console.log("goterr ",err,'status='+xhr.status); console.log(data)  });

tinyxhr("http://site.com/ajaxaction",function (err,data,xhr){ if (err) console.log("goterr ",err,'status='+xhr.status); console.log(data)  },'POST','value1=1&value2=2');

tinyxhr("http://site.com/ajaxaction.json",function (err,data,xhr){ if (err) console.log("goterr ",err,'status='+xhr.status); console.log(data); console.log(JSON.parse(data))  },'POST',JSON.stringify({value:1}),'application/javascript'); 

cb - a callback function like: function (err,data,XMLHttpRequestObject){ if (err) throw err;   }
