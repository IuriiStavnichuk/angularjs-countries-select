##AngularJS countries select

###Countries select is an AngularJS directive for picking countries from a list.

Since the data is retrieved from the external JSON file the developer does not need to worry about generating data within the program. This makes the module more flexible and maintainable so this approach allows us to place uncountable amount of these charts on the page in the neat way without polluting your HTML.

### How to install
 + Copy `countriesSelect.js` wherever you want
 + Reference it in your index.html file
 + Reference the module in your app file :
     angular.module('MainWebApp', [ 'ngResource','countriesSelect'])

### How to use
The countries select is called using this syntax :

```html
<countries-select class="countries-list" array-countries-list = "arrayCountriesList"></countries-select>
```

The countries select directive attribute : `array-countries-list`.


#### array-countries-list
Your data must be JSON object.
```js
{
    "id": 1,
    "jsonrpc": "2.0",
    "totalCountry": 33,
    "result": [
        {
            "continent": "Northern America",
            "id": 1,
            "isSelected": false,
            "country": [
                {
                    "id": 287,
                    "name": "Antigua and Barbuda",
                    "isSelected": false
                },
                {
                    "id": 288,
                    "name": "Canada",
                    "isSelected": false
                }
            ]
        },
        {
            "continent": "Oceania",
            "id": 7,
            "isSelected": false,
            "country": [
                {
                    "id": 320,
                    "name": "Nauru",
                    "isSelected": false
                },
                {
                    "id": 322,
                    "name": "Tonga",
                    "isSelected": false
                }
            ]
        }
    ]
}
```

