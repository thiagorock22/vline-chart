# vLine-chart
Simple vertical line chart

The vLine Chart is basicly a table with columns, rows and markers

![Preview](preview.png)

##### To use the vLine Chart, first you need to instanciate the class
```javascript
vline = new VLine()
```

##### Then, you have to setup the font of your chart
```javascript
vline.setupFont('Courier', 16, 20)
```

1. The first parameter is the **font family**
2. The second parameter is the **font size**
3. The third parameter is the **font margin** (It is 20 by default)

##### After setting the font, you need to setup the header of your chart
```javascript
vline.setupVLineHeader('Leadership Attributes', [
	'Low',
	'Medium',
	'High'
])
```
 
1. The first parameter is the **title** of your chart
2. The second parameter is an **array of strings** which are the columns of your chart
 
##### Now you can add your rows to the chart
```javascript
vline.addElement('Business management', 2)
vline.addElement('Entrepreneurial mindset', 3)
vline.addElement('Ambition and resilience', 2)
vline.addElement('Relationship building', 2)
vline.addElement('Project management', 1)
vline.addElement('Taking orders', 1)
```

1. The first parameter is the **description of your item**
2. The second parameter is the **index that your row is scored**

##### After adding your rows you can build the chart
```javascript
vline.buildCanvas()
```
