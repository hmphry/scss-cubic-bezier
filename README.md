# scss-cubic-bezier

## overview

A list of SCSS variable of common cubic bezier formulas. Please visit [http://easings.net/](http://easings.net/) for visual examples.

## installation

npm install --save scss-cubic-bezier

## usage

```scss

@import "scss-cubic-bezier/scss-cubic-bezier";

.box-1 {
  transform: translateY(0);
  opacity: 0;
  transition: .3s $easeOutSine;
}
.box-1:hover {
  transform: translateY(-10px);
  opacity: 1;
  transition: .3s $easeInQuad;
}

```

## output

```scss

.box-1 {
  transform: translateY(0);
  opacity: 0;
  transition: .3s cubic-bezier(0.39, 0.575, 0.565, 1);
}
.box-1:hover {
  transform: translateY(-10px);
  opacity: 1;
  transition: .3s cubic-bezier(0.55, 0.085, 0.68, 0.53);
}

```
