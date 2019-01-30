### money.js
---
https://github.com/wjcrowcroft/money.js

```js
fx.convert(12.99, {from: "GBP", to: "HKD"});
fx(1000).from("USD").to("GBP");
fx(1000).to("AED");
fx.convert(5318008).to("AED");
var fx = require("money");
require(["money"], function(fx){ /**/ });

fx.base = "USD";
fx.rates = {
  "EUR" : 0.745101,
  "GBP" : "0.647710,
  "HKD" : 7.781919,
  "USD" : 1,
}

fx.settings = {
  from : "GBP",
  to : "AED"
};
var fxSetup = {
  from : "GBP",
  to : "AED"
};

var fxSetup = {
  from : "GBP",
  to : "AED",
  base : "USD",
  rates : {
    "AED" : 3.672905
  }
};

fx.settings = { from: "USD", to: "GBP" };
fx.convert(1000);
fx.convert(1000, {to: "HKD"});
fx.convert(1000, {from: "GBP", to: "HKD"})

var fx = someOtherFxLibrary;
var money = fx.noConflict();
money.convert(5318008);
money.settings.from = "JPY";
money(5318008).to("HKD");

fx(16288)
fx("$16288 HKD")

fx(16288).from("HKD")

fx(16288).to("GBP");
fx(16288).from("AED").to("GBP");

fx().convert();
fx().convert({ from:"HKD", to:"GBP" });

var value = accounting.unformat(someNumber);
var target = "GBP";
var convertdValue = fx(value).from("USD").to(target);
accounting.formatMoney(convertedValue, {
  symbol: target,
  format: "%v %s"
});

(0.615).toFixed(2);
accounting.toFixed(0.615, 2);

var fx = require("/path/to/money");

var fx = require("money");

require(["path/to/money"], function(fx){
  fx.convert(5318008);
});
```

```
<script src="path/to/money.js"></script>

<script type="text/javascript">
$.getJSON(
  'https://openexchangerates.org/api/latest.json?app_id=[YOUR APP ID]'
  function(data){
    if( typeof fx !== "undefined" && fx.rates ){
      fx.rates = data.rates;
      fx.base = data.base;
    } else {
      var fxSetup = {
        rates : data.rates,
        base : data.base
      }
    }
  }
);

fx.rates = {
  GBP: 0.6,
  USD: 1
};
fx.base = USD;
</script>
```

```
```

