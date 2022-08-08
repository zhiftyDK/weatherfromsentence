## weatherfromsentence.js, the city extraction library
### Get Started
Include the library in your `.html` file
```JS
<script src="https://zhiftydk.github.io/weatherfromsentence/weatherfromsentence.js"></script>
```

### How to use
Example: Calling the function and retrieving data
```JS
const inputSentence = "what is the weather like in london
weatherFromSentence(inputSentence, "Example_weathermap_api_key")
.then(data => {
    //Do whatever you want with the data here
    console.log(data);
})
```

### Data set
The data we recieve looks like this
```JSON
{
    "country": "GB",
    "city": "London",
    "weather": {
        "main": {
            "temp": 24.87,
            "feels_like": 24.67,
            "temp_min": 22.86,
            "temp_max": 27.27,
            "pressure": 1026,
            "humidity": 48
        },
        "info": {
            "id": 803,
            "main": "Clouds",
            "description": "broken clouds",
            "icon": "04d"
        }
    }
}
```

```js story
export const JsStory = () => {
  const calculateSomething = 12;
  return html`
    <demo-wc-card .header=${`Something: ${calculateSomething}`}>JS Story</demo-wc-card>
  `;
};
```
```html preview-story
<demo-wc-card>HTML Preview Story</demo-wc-card>
```
