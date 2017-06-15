# Title

The chart title defines text to draw at the top of the chart.

## Title Configuration
The title configuration is passed into the `options.title` namespace. The global options for the chart title is defined in `Chart.defaults.global.title`.

| Name | Type | Default | Description
| -----| ---- | --------| -----------
| `display` | `Boolean` | `false` | is the title shown
| `position` | `String` | `'top'` | Position of title. [more...](#position)
| `fontSize` | `Number` | `12` | Font size
| `fontFamily` | `String` |  `"'Helvetica Neue', 'Helvetica', 'Arial', sans-serif"` | Font family for the title text.
| `fontColor` | Color | `'#666'` | Font color
| `fontStyle` | `String` | `'bold'` | Font style
| `padding` | `Number` | `10` | Number of pixels to add above and below the title text.
| `lineSpacing` | `Number` | `5` | Number of pixels between lines of the text when `text` is specified as an array of strings.
| `text` | `String/String[]`  | `''` | Title text to display. If specified as an array, text is rendered on multiple lines.

### Position
Possible title position values are:
* `'top'`
* `'left'`
* `'bottom'`
* `'right'`

## Example Usage

The example below would enable a title of 'Custom Chart Title' on the chart that is created.

```javascript
var chart = new Chart(ctx, {
    type: 'line',
    data: data,
    options: {
        title: {
            display: true,
            text: 'Custom Chart Title'
        }
    }
})
```
