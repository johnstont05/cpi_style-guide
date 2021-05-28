# Data Visualization Style Guide
## Colors
### Main Colors
| Swatch | Name | Hex | SCSS Variable |
| :----- | :--- | :-- | :------------ |
| ![#f35d26](https://via.placeholder.com/15/f35d26/000000?text=+) | Coral | #f35d26 | $c-coral |
| ![#0276e8](https://via.placeholder.com/15/0276e8/000000?text=+) | Bright Blue | #0276e8 | $c-blue-bright |
| ![#1ebcbc](https://via.placeholder.com/15/1ebcbc/000000?text=+) | Mint | #1ebcbc | $c-mint |
| ![#ffc200](https://via.placeholder.com/15/ffc200/000000?text=+) | Yellow | #ffc200 | $c-yellow |
| ![#04284B](https://via.placeholder.com/15/04284B/000000?text=+) | Dark Blue | #04284B | $c-blue-dark |
| ![#7f7f7d](https://via.placeholder.com/15/7f7f7d/000000?text=+) | Gray | #7f7f7d | $c-gray |
| ![#f35d26](https://via.placeholder.com/15/d8d8d8/000000?text=+) | No data | #d8d8d8 | $c-null |

<hr> 
When creating visualizations, define whether it should be represented as sequential or categorical and choose from the colors below depending on how many variables needed.

#### One Variable
To visualize data with one variable, use **BRIGHT BLUE**.
<br>
![bright blue](https://github.com/PublicI/style-guide/blob/main/images/one-variable.jpg?raw=true)
```html
['#0276e8']
```
#### Two Variables

##### Sequential
![two variables sequential](https://github.com/PublicI/style-guide/blob/main/images/sequential/two-variables_sequential.jpg?raw=true)
```html
['#0276e8', '#00166d']
```
##### Categorical
![two variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/two-variables_categorical-01.jpg?raw=true)
```html
['#0276e8', '#f35d26']
```
![two variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/two-variables_categorical-02.jpg?raw=true)
```html
['#0276e8', '#1ebcbc']
```
![two variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/two-variables_categorical-03.jpg?raw=true)
```html
['#0276e8', '#ffc200']
```

#### Three Variables

##### Sequential
![three variables sequential](https://github.com/PublicI/style-guide/blob/main/images/sequential/three-variables_sequential.jpg?raw=true)
```html
['#8fc7ff', '#0276e8', '#003092']
```
##### Categorical
![three variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/three-variables_categorical.jpg?raw=true)
```html
['#0276e8', '#f35d26', '#1ebcbc']
```
#### Four Variables

##### Sequential
![four variables sequential](https://github.com/PublicI/style-guide/blob/main/images/sequential/four-variables_sequential.jpg?raw=true)
```html
['#76b2ff', '#0276e8', '#0040a6', '#001168']
```
##### Categorical
![four variables sequential](https://github.com/PublicI/style-guide/blob/main/images/categorical/four-variables_categorical.jpg?raw=true)
```html
['#0276e8', '#f35d26', '#ffc200', '#1ebcbc']
```
#### Five Variables

##### Sequential
![five variables sequential](https://github.com/PublicI/style-guide/blob/main/images/sequential/five-variables_sequential.jpg?raw=true)
```html
['#a4d9ff', '#66a6ff', '#0276e8', '#004ab3', '#002380']
```
##### Categorical
![five variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/five-variables_categorical.jpg?raw=true)
```html
['#0276e8', '#f35d26', '#ffc200', '#1ebcbc', '#04284B']
```
#### Six Variables

##### Sequential
![six variables sequential](https://github.com/PublicI/style-guide/blob/main/images/sequential/six-variables_sequential.jpg?raw=true)
```html
['#90c8ff', '#5b9eff', '#0276e8', '#0051bb', '#002f91', '#001068']
```
##### Categorical
![six variables categorical](https://github.com/PublicI/style-guide/blob/main/images/categorical/six-variables_categorical.jpg?raw=true)
```html
['#0276e8', '#f35d26', '#ffc200', '#1ebcbc', '#04284b', '#7f7f7d']
```

## Fonts
Data visualizations follow the "One font/big header" font system. For example, the Maison Neue typeface is used throughout, but with various sizes and weights depending on the content.

#### Header Text
```css
.basic-text h4 {
  font-family: 'Maison Neue', sans-serif;
  font-weight: 600;
  font-size: 20px;
  color: #04284b;
  line-height: 115%;
  max-width: 650px; /* depending on graphic */
  padding-top: 0;
  margin-top: 0;
}
```
#### Subheader Text
```css
.chatter {
  font-family: 'Maison Neue', sans-serif;
  font-weight: normal;
  font-size: 15px;
  line-height: 130%;
  color: #646464;
  max-width: 700px; /* depending on graphic */
}
```
#### Labels/Axis Text
```css
font-family: 'Maison Neue', sans-serif;
font-size: 12px;
```
#### Notes/Sources Text
```css
.source {
  font-family: 'Maison Neue', sans-serif;
  font-size: 14px;
  line-height: 18px;
  color: #666;
  max-width: 700px; /* depending on graphic */
  margin-bottom: 15px;
  padding-top: 8px;
}
```
#### Tooltips
```css
#tooltip {
  font-family: "Maison Neue", sans-serif;
  font-size: 12px;
  backface-visibility: hidden;
  position: fixed;
  top: 0;
  left: 0;
  pointer-events: none;
  text-align: center; /* depending on graphic */
  display: block;
  background-color: #fff;
  border: 1px solid #d3d3d3;
  border-radius: 3px;
  width: 150px; /* depending on graphic */
  padding: 4px;
  pointer-events: none;
}

```
## Examples
### Maps
#### Sequential
Choropleth maps should use the **BRIGHT BLUE** (#0276e8) sequential color palettes as defined above. Use this **[link](https://gka.github.io/palettes/#/6|s|0276e8|f35d26|0|0)** to generate a sequential palette based on your desired number of variables. First, copy and paste the **BRIGHT BLUE** hex code into the "input" box and then select the number of colors (variables) needed for the graphic.
![map sequential](https://github.com/PublicI/style-guide/blob/main/examples/maps/example-map_sequential.png?raw=true)


#### Diverging
Maps displaying positive and negative change/growth or show a comparison should use the **BRIGHT BLUE** (#0276e8) and **CORAL** (#f35d26) colors. Use this **[link](https://gka.github.io/palettes/#/4|d|0276e8|f35d26|1|1)** to generate a diverging palette based on your desired number of variables. First, copy and paste the **BRIGHT BLUE** and **CORAL** hex codes into each "input" box and then select the number of colors (variables) needed for the graphic. A color palette will be generated. 
![map diverging](https://github.com/PublicI/style-guide/blob/main/examples/maps/example-map_diverging.png?raw=true)

### Charts
Datawrapper can be used to create simple charts. Log into the CPI Datawrapper account to see templates for each chart listed below.
#### Bar Charts
![bar chart](https://github.com/PublicI/style-guide/blob/main/examples/charts/example_bar-chart.png?raw=true)
![stacked bar chart](https://github.com/PublicI/style-guide/blob/main/examples/charts/example_stacked-bar-chart.png?raw=true)
#### Line Charts
![line chart](https://github.com/PublicI/style-guide/blob/main/examples/charts/example_line-chart.png?raw=true)
![multiple line chart](https://github.com/PublicI/style-guide/blob/main/examples/charts/example_multiple-line-chart.png?raw=true)
