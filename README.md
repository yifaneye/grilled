# grilled

A library for responsive grid system 🏁

![Grilled](https://yifanai.s3-ap-southeast-2.amazonaws.com/grilled/grilled.jpg)

## Demo

👉 [Website Demo](https://unpkg.com/grilled@1.1.0/dist/grid.html)

OR

![GIF Demo](https://yifanai.s3-ap-southeast-2.amazonaws.com/grilled/grilled.gif)

## Background

I really love responsive grid systems to create responsive websites!

The libraries I use, namely Bootstrap and Material UI only offers 12 columns, and NG-ZORRO only offers 24 columns.

I sometimes wanted to have 10 columns, sometimes 5 columns, sometimes 9 columns ... 😞

## Getting Started

### Using CDN

Add this line to HTML file

```
<link rel="stylesheet" type="text/css" href="https://unpkg.com/grilled@1.1.0/dist/css/grid.min.css">
```

✅

### Using NPM

Install the 'grilled' package using npm

```
npm i grilled
```

then \
add this line to index.js

```
require('grilled');
```

OR \
add this line to HTML file

```
<link rel="stylesheet" type="text/css" href="grilled/dist/css/grid.min.css">
```

✅

## Usage

Containers: grid1 ~ grid12 \
Items: xs0 ~ xs12, sm0 ~ sm12, md0 ~ md12, lg0 ~ lg12, xl0 ~ xl12, g0 ~ g12

| Screen Width    |<600px|<960px|<1280px|<1920px|\>=1920px|
|----------------:|:-----|:-----|:------|:------|:--------|
|Range Key        |xs    |sm    |md     |lg     |xl       |
|Number of Columns|0 ~ 12|0 ~ 12|0 ~ 12 |0 ~ 12 |0 ~ 12   |

e.g.

```html
<div class="grid10">
	<div class="xs10 g7">Big Item</div>
	<div class="xs10 g3">Small Item</div>
	<div class="xs10 sm5 g0">Item only on xs and sm</div>
</div>
```

```html
<div class="grid12">
	<div class="box sm0 lg8 g12">sm0 lg8 g12</div>

	<div class="box md12 g8">xs12 sm12 g8</div>
	<div class="box md12 g4">xs12 sm12 g4</div>

	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box g0">0</div>

	<div class="box xs4 sm2 g1">xs4 sm2 g1</div>
	<div class="box xs8 sm4 g2">xs8 sm4 g2</div>
	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box xs12 sm6 g3">xs12 sm6 g3</div>
	<div class="box xs8 sm4 g2">xs8 sm4 g2</div>
	<div class="box xs4 sm2 g1">xs4 sm2 g1</div>
</div>

```

![Grilled](https://yifanai.s3-ap-southeast-2.amazonaws.com/grilled/xs.jpg)
![Grilled](https://yifanai.s3-ap-southeast-2.amazonaws.com/grilled/sm.jpg)
![Grilled](https://yifanai.s3-ap-southeast-2.amazonaws.com/grilled/md.jpg)

## Package Structure

```
.
|-- LICENSE
|-- README.md
|-- dist
|   |-- grid.html
|   `-- css
|       `-- grid.min.css
|-- gulpfile.js
|-- index.js
|-- package-lock.json
|-- package.json
`-- src
    |-- grid.html
    `-- scss
        |-- grid
        |   |-- _breakpoints.css
        |   |-- _breakpoints.css.map
        |   |-- _breakpoints.scss
        |   |-- _grid.css
        |   |-- _grid.css.map
        |   `-- _grid.scss
        |-- grid.css
        |-- grid.css.map
        `-- grid.scss
```

## Authors

* **Yifan Ai** - *Initial work*

See also the list of [contributors](https://github.com/yifaneye/grilled/graphs/contributors) who participated in this project.

## License

This project is licensed under the MIT License
