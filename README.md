# Grid

A library for responsive grid system 🏁

## Background

I really love responsive grid systems to create responsive websites!

The libraries I use, namely Bootstrap and Material UI only offers 12 columns, and NG-ZORRO only offers 24 columns.

I sometimes wanted to have 10 columns, sometimes 5 columns, sometimes 9 columns ... 😞

## Getting Started

### Using CDN

Add this line to HTML file

```
<link rel="stylesheet" type="text/css" href="https://unpkg.com/grid@1.0.0/dist/css/grid.min.css">
```

✅

### Using NPM

Install grid package using npm

```
npm i grid
```

then \
add this line to index.js

```
require('grid');
```

OR \
add this line to HTML file

```
<link rel="stylesheet" type="text/css" href="grid/dist/css/grid.min.css">
```

✅

## Usage

Containers: grid1 ~ grid12 \
Items: xs0 ~ xs12, sm0 ~ sm12, md0 ~ md12, lg0 ~ lg12, g0 ~ g12

| Screen Width    |0px   |600px|960px|1280px|1920px|
|----------------:|:-----|:-----|:-----|:------|:------|
|Range Key        |xs    |sm   |md   |lg    |g     |
|Number of Columns|0 ~ 12|

e.g.

```
<div class="grid10">
    <div class="xs10 g7">Big Item</div>
    <div class="xs10 g3">Small Item</div>
    <div class="xs10 sm5 g0">Only on xs and sm</div>
</div>
```

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

See also the list of [contributors](https://github.com/yifaneye/grid/graphs/contributors) who participated in this project.

## License

This project is licensed under the MIT License