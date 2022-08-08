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

```js preview-story
// will be visible when platform web is selected
export const JsPreviewStory = () => html` <demo-wc-card>JS Preview Story</demo-wc-card> `;
```

```xml story-code
<!-- will be visible when platform android is selected -->
<Button
    android:id="@+id/demoWcCard"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Android Code"
    style="@style/Widget.FooComponents.Demo.Wc.Card"
/>
```

```swift story-code
// will be visible when platform ios is selected
import DemoWc.Card

let card = DemoWcButton()
```
