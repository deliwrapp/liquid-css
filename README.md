# LIQUID THEME

# PROJECT OVERVIEW

Liquid Theme Framework

## Description
LIQUID THEME based on the liquid precept

## Visuals

In progress

## Installation
Look DOC

## Usage
To liquidize theming !!!

## Support
By Deliwrapp Production team

## Roadmap
Currently in development

## Contributing
As you want !!!

## Authors and acknowledgment
By the Deliwrapp Production Team

## License
LGPL

## Project status
Currently in development


# DOC

## Introduction
The DELIWRAPP CLIENT APP

## Getting Started
Install locally or downland directly in you dev directory.

A CSS Liquid Framework using Flexbox.

- **Simple**: Provides just 2 base classes `liquid-grid` and `col` and some modifiers.
- **Flexible**: Easy to use Flexbox features.

[Flexible Box Layout Module](http://caniuse.com/#search=flex) and [`calc()` as CSS unit value](http://caniuse.com/#search=calc) used in Liquid-Theme are available on modern browsers (Chrome, Firefox, Safari, Opera, Edge and IE11).

### The Grid and the Col

```html
<div class="liquid-grid">
  <div class="col -3of12">3of12</div>
  <div class="col -9of12">9of12</div>
</div>
```

#### `liquid-grid` modifiers

| Vertical layout | Description |
|---|---|
| `-top` | Pull items to top |
| `-middle` |  Pull items to middle |
| `-bottom` |  Pull items to bottom |
| `-stretch` | Stretch items |
| `-baseline` |  Pull items to baseline |

| Horizontal layout | Description |
|---|---|
| `-left` | Layout items to left |
| `-center` | Layout items To center |
| `-right` | Layout items to right |
| `-between` | Add spaces between items |
| `-around` | Add spaces around items |

#### `col` modifiers

| Col width | Description |
|---|---|
| `-fill` | Set item width to left |
| `-col-1` | Set item width to 8.3% |
| `-col-2` | Set item width to 16.7% |
| `-col-3` | Set item width to 25% |
| `-col-4` | Set item width to 33% |
| `-col-5` | Set item width to 41.7% |
| `-col-6` | Set item width to 50% |
| `-col-7` | Set item width to 58.3% |
| `-col-8_` | Set item width to 66.7% |
| `-col-9` | Set item width to 75% |
| `-col-10` | Set item width to 83.3% |
| `-col-11` | Set item width to 91.7% |
| `-col-12` | Set item width to 100% |


#### Skeleton `GRID` Full / Tablett / Desktop

```css
.liquid-grid            { display: flex; flex-wrap: wrap; }
.liquid-grid.\-top      { align-items: flex-start; }
.liquid-grid.\-middle   { align-items: center; }
.liquid-grid.\-bottom   { align-items: flex-end; }
.liquid-grid.\-stretch  { align-items: stretch; }
.liquid-grid.\-baseline { align-items: baseline; }
.liquid-grid.\-left     { justify-content: flex-start; }
.liquid-grid.\-center   { justify-content: center; }
.liquid-grid.\-right    { justify-content: flex-end; }
.liquid-grid.\-between  { justify-content: space-between; }
.liquid-grid.\-around   { justify-content: space-around; }

.col          { box-sizing: border-box; flex-shrink: 0; padding: 0.5rem; }
.col.\-fill   { width: 0; min-width: 0; flex-grow: 1; }
.col.\-col-1  { width: calc(100% * 1 / 12); }
.col.\-col-2  { width: calc(100% * 2 / 12); }
.col.\-col-3  { width: calc(100% * 3 / 12); }
.col.\-col-4  { width: calc(100% * 4 / 12); }
.col.\-col-5  { width: calc(100% * 5 / 12); }
.col.\-col-6  { width: calc(100% * 6 / 12); }
.col.\-col-7  { width: calc(100% * 7 / 12); }
.col.\-col-8  { width: calc(100% * 8 / 12); }
.col.\-col-9  { width: calc(100% * 9 / 12); }
.col.\-col-10 { width: calc(100% * 10 / 12); }
.col.\-col-11 { width: calc(100% * 11 / 12); }
.col.\-col-12 { width: 100%; }

.col.\-xs1  { width: calc(100% * 1 / 12); }
.col.\-xs2  { width: calc(100% * 2 / 12); }
.col.\-xs3  { width: calc(100% * 3 / 12); }
.col.\-xs4  { width: calc(100% * 4 / 12); }
.col.\-xs5  { width: calc(100% * 5 / 12); }
.col.\-xs6  { width: calc(100% * 6 / 12); }
.col.\-xs7  { width: calc(100% * 7 / 12); }
.col.\-xs8  { width: calc(100% * 8 / 12); }
.col.\-xs9  { width: calc(100% * 9 / 12); }
.col.\-xs10 { width: calc(100% * 10 / 12); }
.col.\-xs11 { width: calc(100% * 11 / 12); }
.col.\-xs12 { width: 100%; }

.grid {
    display: grid;
    grid-gap: 0.5rem;
    grid-template-columns: repeat(12, 1fr);
    margin: 0 auto;
    width: 100%;
    max-width: 100x;
}
.grid.\-text-center {text-align: center;}
.grid.\-text-left {text-align: left;}
.grid.\-text-right {text-align: right;}
.grid.\-text-end {text-align: end;}
.grid.\-text-start {text-align: start;}
.grid.\-baseline {justify-items: baseline;}
.grid.\-stretch {justify-items: stretch;}
.grid.\-center {justify-items: center;}
.grid.\-left {justify-items: left;}
.grid.\-right {justify-items: right;}
.grid.\-end {justify-items: flex-end;}
.grid.\-start {justify-items: flex-start;}
.grid.\-baseline {align-items: baseline;}
.grid.\-align-center {align-items: center;}
.grid.\-align-stretch {align-items: stretch;}
.grid.\-align-end {align-items: flex-end;}
.grid.\-align-start {align-items: flex-start;}

.g-1, .g-2, .g-3, .g-4, .g-5, .g-6,
.g-7, .g-8, .g-9, .g-10, .g-11, .g-12 {
    grid-column-end: span 12;
}

.grid-nested {
    display: grid;
    grid-gap: 10px;
    grid-template-columns: repeat(12, 1fr);
}

.g-2-rows { grid-row-end: span 2 }
.g-3-rows { grid-row-end: span 3 }
.g-4-rows { grid-row-end: span 4 }
.g-5-rows { grid-row-end: span 5 }
.g-6-rows { grid-row-end: span 6 }
.g-7-rows { grid-row-end: span 7 }
.g-8-rows { grid-row-end: span 8 }
.g-9-rows { grid-row-end: span 9 }
.g-10-rows { grid-row-end: span 10 }
.g-11-rows { grid-row-end: span 11 }
.g-12-rows { grid-row-end: span 12 }

.g-1 { grid-column-end: span 1 }
.g-2 { grid-column-end: span 2 }
.g-3 { grid-column-end: span 3 }
.g-4 { grid-column-end: span 4 }
.g-5 { grid-column-end: span 5 }
.g-6 { grid-column-end: span 6 }
.g-7 { grid-column-end: span 7 }
.g-8 { grid-column-end: span 8 }
.g-9 { grid-column-end: span 9 }
.g-10 { grid-column-end: span 10 }
.g-11 { grid-column-end: span 11 }
.g-12 { grid-column-end: span 12 }


@media (min-width: 476px) {

    .col.\-sm1  { width: calc(100% * 1 / 12); }
    .col.\-sm2  { width: calc(100% * 2 / 12); }
    .col.\-sm3  { width: calc(100% * 3 / 12); }
    .col.\-sm4  { width: calc(100% * 4 / 12); }
    .col.\-sm5  { width: calc(100% * 5 / 12); }
    .col.\-sm6  { width: calc(100% * 6 / 12); }
    .col.\-sm7  { width: calc(100% * 7 / 12); }
    .col.\-sm8  { width: calc(100% * 8 / 12); }
    .col.\-sm9  { width: calc(100% * 9 / 12); }
    .col.\-sm10 { width: calc(100% * 10 / 12); }
    .col.\-sm11 { width: calc(100% * 11 / 12); }
    .col.\-sm12 { width: 100%; }
}


```

TABLETT
```css

```

DESKTOP
```css

@media (min-width: 996px) {   
    .col.\-l1  { width: calc(100% * 1 / 12); }
    .col.\-l2  { width: calc(100% * 2 / 12); }
    .col.\-l3  { width: calc(100% * 3 / 12); }
    .col.\-l4  { width: calc(100% * 4 / 12); }
    .col.\-l5  { width: calc(100% * 5 / 12); }
    .col.\-l6  { width: calc(100% * 6 / 12); }
    .col.\-l7  { width: calc(100% * 7 / 12); }
    .col.\-l8  { width: calc(100% * 8 / 12); }
    .col.\-l9  { width: calc(100% * 9 / 12); }
    .col.\-l10 { width: calc(100% * 10 / 12); }
    .col.\-l11 { width: calc(100% * 11 / 12); }
    .col.\-l12 { width: 100%; } 
}

@media (min-width: 1250px) { 
    
    .col.\-xl1  { width: calc(100% * 1 / 12); }
    .col.\-xl2  { width: calc(100% * 2 / 12); }
    .col.\-xl3  { width: calc(100% * 3 / 12); }
    .col.\-xl4  { width: calc(100% * 4 / 12); }
    .col.\-xl5  { width: calc(100% * 5 / 12); }
    .col.\-xl6  { width: calc(100% * 6 / 12); }
    .col.\-xl7  { width: calc(100% * 7 / 12); }
    .col.\-xl8  { width: calc(100% * 8 / 12); }
    .col.\-xl9  { width: calc(100% * 9 / 12); }
    .col.\-xl10 { width: calc(100% * 10 / 12); }
    .col.\-xl11 { width: calc(100% * 11 / 12); }
    .col.\-xl12 { width: 100%; }
    
}

```



#### Skeleton `FLUID` 

```css



```

#### Skeleton `CONTAINER` 

```css

.liquid-container  { 
    height: 100%;
    width: 100%;
}

```

#### Skeleton `HEADING` 

```css



```

#### Skeleton `TYPO` 

```css



```

#### Skeleton `Z-INDEX` 

```css



```

#### Helper`POSITION` 

```css

.position.\-relative  { position: relative; }
.position.\-absolute  { position: absolute; }
.position.\-fixed  { position: fixed; }
.position.\-static  { position: static; }
.position.\-sticky  { position: sticky; }
.position.\-pos-unset  { position: unset; }

.order-before {order: -1}
.order-after {order: 1}

```

#### Helper `FLEX HELPERS` 

```css
.flex-fade {flex: 0 1 auto}
.flex-fame {flex: 1 0 auto}
.flex-auto {flex: 1 1 auto}
.flex-none {flex: 0 0 auto}
.flex-inline {display: inline-flex}
.flex { display: flex;}
.flex-row {flex-direction: row;}
.flex-row-reverse{flex-direction: row-reverse;}
.flex-column {flex-direction: column;}
.flex-row-reverse{flex-direction: column-reverse;}

.wrap{flex-wrap: wrap;}
.nowrap{flex-wrap: nowrap;}
.wrap-reverse{flex-wrap: wrap-reverse;}

.flow-wrap {flex-flow: wrap;}
.flow-nowrap {flex-flow: nowrap;}
.flow-wrap-reverse {flex-flow: wrap-reverse;}
.flow-row {flex-flow: row;}
.flow-row-reverse {flex-flow: row-reverse;}
.flow-column {flex-flow: column;}
.flow-column-reverse {flex-flow: column-reverse;}


.grow-0 {flex-grow: 0}
.grow-1 {flex-grow: 1}
.grow-2 {flex-grow: 2}
.grow-3 {flex-grow: 3}
.grow-4 {flex-grow: 4}
.grow-5 {flex-grow: 5}
.grow-6 {flex-grow: 6}
.grow-7 {flex-grow: 7}
.grow-8 {flex-grow: 8}
.grow-9 {flex-grow: 9}
.grow-10 {flex-grow: 10}
.grow-11 {flex-grow: 11}
.grow-12 {flex-grow: 12}

.shrink-0 {flex-shrink: 0}
.shrink-1 {flex-shrink: 1}
.shrink-2 {flex-shrink: 2}
.shrink-3 {flex-shrink: 3}
.shrink-4 {flex-shrink: 4}
.shrink-5 {flex-shrink: 5}
.shrink-6 {flex-shrink: 6}
.shrink-7 {flex-shrink: 7}
.shrink-8 {flex-shrink: 8}
.shrink-9 {flex-shrink: 9}
.shrink-10 {flex-shrink: 10}
.shrink-11 {flex-shrink: 11}
.shrink-12 {flex-shrink: 12}

.basis-0 {flex-basis: 0%}
.basis-1 {flex-basis: 8.333333333%}
.basis-2 {flex-basis: 16.6666666666%}
.basis-3 {flex-basis: 25%}
.basis-4 {flex-basis: 33.3333333333%}
.basis-5 {flex-basis: 41.6666666666%}
.basis-6 {flex-basis: 50%}
.basis-7 {flex-basis: 58.333333333%}
.basis-8 {flex-basis: 66.6666666666%}
.basis-9 {flex-basis: 75%}
.basis-10 {flex-basis: 83.3333333333%}
.basis-11 {flex-basis: 91.6666666666%}
.basis-12 {flex-basis: 100%}
.basis-100vw {flex-basis: 100vw}
.basis-100vh {flex-basis: 100vh}
.basis-100vmax {flex-basis: 100vmax}
.basis-100vmin {flex-basis: 100vmin}
.basis-golden {flex-basis: 61.803398875%}
.basis-auto {flex-basis: auto}
.basis-content {flex-basis: content}

.flex-container{display: flex; flex-flow: row wrap;  width: 80%; margin: 0 auto}
.fc-10,.fc-12,.fc-17,.fc-20,.fc-25,.fc-33,.fc-40,.fc-50,.fc-60,.fc-67,.fc-75,.fc-80,.fc-83,.fc-100,.fluid {width:100%; margin:0}

.fc-fluid{flex:2}
.fc-clear{width: 100%}
.fc-nomargin{display: flex; flex-flow: row wrap; padding:0 !important; margin:0 !important}


@media (min-width: 576px) {

    .fc-10,.fc-12,.fc-17,.fc-20,.fc-25,.fc-33,.fc-40,.fc-50,.fc-60,.fc-67,.fc-75,.fc-80,.fc-83,.fc-100,.fluid{margin:0 0 0 var(--m)}

    .fc-10{width:calc(10% - var(--flex-container-margin))}
    .fc-12{width:calc(12.5% - var(--flex-container-margin))}
    .fc-17{width:calc(16.6667% - var(--flex-container-margin))}
    .fc-20{width:calc(20% - var(--flex-container-margin))}
    .fc-25{width:calc(25% - var(--flex-container-margin))}
    .fc-33{width:calc(33.3334% - var(--flex-container-margin))}
    .fc-40{width:calc(40% - var(--flex-container-margin))}
    .fc-50{width:calc(50% - var(--flex-container-margin))}
    .fc-60{width:calc(60% - var(--flex-container-margin))}
    .fc-67{width:calc(66.6667% - var(--flex-container-margin))}
    .fc-75{width:calc(75% - var(--flex-container-margin))}
    .fc-80{width:calc(80% - var(--flex-container-margin))}
    .fc-83{width:calc(83.3334% - var(--flex-container-margin))}
    .fc-100{width:calc(100% - var(--flex-container-margin))}
    
}

@media (orientation: portrait) {
    .flex-inline\@portrait {display: inline-flex}
    .flex-block\@portrait {display: flex}
    .flex-row\@portrait {flex-direction: row}
    .flex-row-reverse\@portrait {flex-direction: row-reverse}
    .flex-column\@portrait {flex-direction: column}
    .flex-column-reverse\@portrait {flex-direction: column-reverse}
    .nowrap\@portrait {flex-wrap: nowrap}
    .wrap\@portrait {flex-wrap: wrap}
    .wrap-reverse\@portrait {flex-wrap: wrap-reverse}
  }
  
  @media (orientation: landscape) {
    .flex-inline\@landscape {display: inline-flex}
    .flex\@landscape {display: flex}
    .flex-row\@landscape {flex-direction: row}
    .flex-row-reverse\@landscape {flex-direction: row-reverse}
    .flex-column\@landscape {flex-direction: column}
    .flex-column-reverse\@landscape {flex-direction: column-reverse}
    .nowrap\@landscape {flex-wrap: nowrap}
    .wrap\@landscape {flex-wrap: wrap}
    .wrap-reverse\@landscape {flex-wrap: wrap-reverse}
  }
```

###### [`display`](https://www.w3.org/TR/css-flexbox-1/#flex-containers)
- `.flex-inline` for `inline-flex`
- `.flex` for `flex`

###### [`flex-flow`](https://www.w3.org/TR/css-flexbox-1/#flex-flow-property)

- Compose [`flex-direction`](#flex-direction) [`flex-wrap`](#flex-wrap)
- Default is `row nowrap`

###### [`flex-direction`](https://www.w3.org/TR/css-flexbox-1/#flex-direction-property)

- `.flex-row`
- `.flex-row-reverse`
- `.flex-column`
- `.flex-column-reverse`

###### [`flex-wrap`](https://www.w3.org/TR/css-flexbox-1/#flex-wrap-property)

- `.nowrap` for `nowrap`
- `.wrap` for `wrap`
- `.wrap-reverse` for `wrap-reverse`


###### [`order`](https://www.w3.org/TR/css-flexbox-1/#order-property)
- `.order-before`
- `.order-after`

###### [`align-items`](https://www.w3.org/TR/css-flexbox-1/#align-items-property)

###### [`align-self`](https://www.w3.org/TR/css-flexbox-1/#align-items-property)

###### [`justify-content`](https://www.w3.org/TR/css-flexbox-1/#justify-content-property)

###### [`align-content`](https://www.w3.org/TR/css-flexbox-1/#align-content-property)

###### [`flex`](https://www.w3.org/TR/css-flexbox-1/#flex-property)

<a name="flex-presets"></a>
<a name="flex-shorthand"></a>

Shorthand classes supply [common presets](https://www.w3.org/TR/css-flexbox-1/#flex-common)

- `.flex-fade` for `0 1 auto` aka shrinkable
- `.flex-fame` for `1 0 auto` aka growable
- `.flex-auto` for `1 1 auto` aka flexible
- `.flex-none` for `none` aka inflexible

Compose with [`grow`](#flex-grow) [`shrink`](#flex-shrink) [`basis`](#flex-basis)

###### [`flex-grow`](https://www.w3.org/TR/css-flexbox-1/#flex-grow-property)
- `.grow-0`
- `.grow-1`
- `.grow-2`
- `.grow-3`
- `.grow-4`
- `.grow-5`
- `.grow-6`
- `.grow-8`
- `.grow-7`
- `.grow-9`
- `.grow-10`
- `.grow-11`
- `.grow-12`

###### [`flex-shrink`](https://www.w3.org/TR/css-flexbox-1/#flex-shrink-property)
- `.shrink-0`
- `.shrink-1`
- `.shrink-2`
- `.shrink-3`
- `.shrink-4`
- `.shrink-5`
- `.shrink-6`
- `.shrink-7`
- `.shrink-8`
- `.shrink-9`
- `.shrink-10`
- `.shrink-11`
- `.shrink-12`

###### [`flex-basis`](https://www.w3.org/TR/css-flexbox-1/#flex-basis-property)
- `.basis-0` 0/12 grid
- `.basis-1` 1/12 grid
- `.basis-2` 2/12 grid
- `.basis-3` 3/12 grid
- `.basis-4` 4/12 grid
- `.basis-5` 5/12 grid
- `.basis-6` 6/12 grid
- `.basis-7` 7/12 grid
- `.basis-8` 8/12 grid
- `.basis-9` 9/12 grid
- `.basis-10` 10/12 grid
- `.basis-11` 11/12 grid
- `.basis-12` 12/12 grid
- `.basis-100vw`
- `.basis-100vh`
- `.basis-100vmax`
- `.basis-100vmin`
- `.basis-golden`
- `.basis-content`
- `.basis-auto`

###### area
<a name="size-control"></a>

Some [flexbugs](https://github.com/philipwalton/flexbugs) are solvable via min or max width or height

- `.area-min` sets both mins to `0` [re: nesting](https://goo.gl/3IZRMt)
- `.area-max` sets both maxes to `100%`

###### `@media`

Responsive [`orientation`](https://drafts.csswg.org/mediaqueries-4/#orientation) classes are available for [`flex-flow`](#flex-flow) and [`display`](#display) classes. Append [`@portrait`](#portrait) or [`@landscape`](#landscape) to these classes to limit them to that orientation. This affords layouts that flow or wrap differently based on viewport orientation or layouts that only flex in one orientation. Try the [#fitting](https://ryanve.github.io/flexboxes/#fitting) example in both portrait and landscape to see how it adapts. You can do this on a phone by rotating the phone or on a computer by resizing the browser window.

```html
class="flex flex-row@portrait flex-column@landscape"
```

###### `portrait`

- `flex-row@portrait`
- `flex-row-reverse@portrait`
- `flex-column@portrait`
- `flex-column-reverse@portrait`
- `wrap@portrait`
- `wrap-reverse@portrait`
- `flex-inline@portrait`
- `flex@portrait`

###### `landscape`

- `flex-row@landscape`
- `flow-row-reverse@landscape`
- `flex-column@landscape`
- `flow-column-reverse@landscape`
- `wrap@landscape`
- `wrap-reverse@landscape`
- `flex-inline@landscape`
- `flex@landscape`


##### Flex Container overview
Flex Container is minimal CSS framework made with Flex

* Minimal
* Responsive. 
* No unnecessary nesting.
* Fluid Column (even multiple times in one row)
* Flexible the main width can be any number or uint ex: 960px, 90% or whatever you like.

###### Code Demo

```html
<div class="fc-50">50%</div>
<div class="fc-50">50%</div>

<div class="fc-33">33,3%</div>
<div class="fc-33">33,3%</div>
<div class="fc-33">33,3%</div>

<div class="fc-25">25%</div>
<div class="fc-fluid">Fluid</div>
<div class="fc-17">17%</div>
<div class="fc-clear"></div> /* => Use clear when you have fluid column */

/* Multiple Fluid columns in one row */

<div class="fc-fluid">Fluid</div>
<div class="fc-25">25%</div>
<div class="fc-25">25%</div>
<div class="fc-fluid">Fluid</div>
<div class="fc-clear"></div>
```

#### Helper `PADDING` 

```css

.padding.\-p1  { padding: 0.25rem; }
.padding.\-p2  { padding: 0.50rem; }
.padding.\-p3  { padding: 0.75rem; }
.padding.\-p4  { padding: 1rem; }
.padding.\-p5  { padding: 1.25rem; }
.padding.\-p6  { padding: 1.5rem; }
.padding.\-p7  { padding: 1.75; }
.padding.\-p8  { padding: 2rem; }
.padding.\-p9  { padding: 2.25rem; }
.padding.\-p10 { padding: 2.5rem; }

.padding.\-pt1  { padding-top: 0.25rem; }
.padding.\-pt2  { padding-top: 0.50rem; }
.padding.\-pt3  { padding-top: 0.75rem; }
.padding.\-pt4  { padding-top: 1rem; }
.padding.\-pt5  { padding-top: 1.25rem; }
.padding.\-pt6  { padding-top: 1.5rem; }
.padding.\-pt7  { padding-top: 1.75; }
.padding.\-pt8  { padding-top: 2rem; }
.padding.\-pt9  { padding-top: 2.25rem; }
.padding.\-pt10 { padding-top: 2.5rem; }

.padding.\-pb1  { padding-bottom: 0.25rem; }
.padding.\-pb2  { padding-bottom: 0.50rem; }
.padding.\-pb3  { padding-bottom: 0.75rem; }
.padding.\-pb4  { padding-bottom: 1rem; }
.padding.\-pb5  { padding-bottom: 1.25rem; }
.padding.\-pb6  { padding-bottom: 1.5rem; }
.padding.\-pb7  { padding-bottom: 1.75; }
.padding.\-pb8  { padding-bottom: 2rem; }
.padding.\-pb9  { padding-bottom: 2.25rem; }
.padding.\-pb10 { padding-bottom: 2.5rem; }

.padding.\-pl1  { padding-left: 0.25rem; }
.padding.\-pl2  { padding-left: 0.50rem; }
.padding.\-pl3  { padding-left: 0.75rem; }
.padding.\-pl4  { padding-left: 1rem; }
.padding.\-pl5  { padding-left: 1.25rem; }
.padding.\-pl6  { padding-left: 1.5rem; }
.padding.\-pl7  { padding-left: 1.75; }
.padding.\-pl8  { padding-left: 2rem; }
.padding.\-pl9  { padding-left: 2.25rem; }
.padding.\-pl10 { padding-left: 2.5rem; }

.padding.\-pr1  { padding-right: 0.25rem; }
.padding.\-pr2  { padding-right: 0.50rem; }
.padding.\-pr3  { padding-right: 0.75rem; }
.padding.\-pr4  { padding-right: 1rem; }
.padding.\-pr5  { padding-right: 1.25rem; }
.padding.\-pr6  { padding-right: 1.5rem; }
.padding.\-pr7  { padding-right: 1.75; }
.padding.\-p8  { padding-right: 2rem; }
.padding.\-pr9  { padding-right: 2.25rem; }
.padding.\-pr10 { padding-right: 2.5rem; }

.liquid-padding.\-p1  { padding: 10%; }
.liquid-padding.\-p2  { padding: 20%; }
.liquid-padding.\-p3  { padding: 30%; }
.liquid-padding.\-p4  { padding: 40%; }
.liquid-padding.\-p5  { padding: 50%; }
.liquid-padding.\-p6  { padding: 60%; }
.liquid-padding.\-p7  { padding: 70%; }
.liquid-padding.\-p8  { padding: 80%; }
.liquid-padding.\-p9  { padding: 90%; }
.liquid-padding.\-p10 { padding: 100%; }

.liquid-padding.\-pt1  { padding-top: 10%; }
.liquid-padding.\-pt2  { padding-top: 20%; }
.liquid-padding.\-pt3  { padding-top: 30%; }
.liquid-padding.\-pt4  { padding-top: 40%; }
.liquid-padding.\-pt5  { padding-top: 50%; }
.liquid-padding.\-pt6  { padding-top: 60%; }
.liquid-padding.\-pt7  { padding-top: 70%; }
.liquid-padding.\-pt8  { padding-top: 80%; }
.liquid-padding.\-pt9  { padding-top: 90%; }
.liquid-padding.\-pt10 { padding-top: 100%; }

.liquid-padding.\-pb1  { padding-bottom: 10%; }
.liquid-padding.\-pb2  { padding-bottom: 20%; }
.liquid-padding.\-pb3  { padding-bottom: 30%; }
.liquid-padding.\-pb4  { padding-bottom: 40%; }
.liquid-padding.\-pb5  { padding-bottom: 50%; }
.liquid-padding.\-pb6  { padding-bottom: 60%; }
.liquid-padding.\-pb7  { padding-bottom: 70%; }
.liquid-padding.\-pb8  { padding-bottom: 80%; }
.liquid-padding.\-pb9  { padding-bottom: 90%; }
.liquid-padding.\-pb10 { padding-bottom: 100%; }

.liquid-padding.\-pl1  { padding-left: 10%; }
.liquid-padding.\-pl2  { padding-left: 20%; }
.liquid-padding.\-pl3  { padding-left: 30%; }
.liquid-padding.\-pl4  { padding-left: 40%; }
.liquid-padding.\-pl5  { padding-left: 50%; }
.liquid-padding.\-pl6  { padding-left: 60%; }
.liquid-padding.\-pl7  { padding-left: 70%; }
.liquid-padding.\-pl8  { padding-left: 80%; }
.liquid-padding.\-pl9  { padding-left: 90%; }
.liquid-padding.\-pl10 { padding-left: 100%; }

.liquid-padding.\-pr1  { padding-right: 10%; }
.liquid-padding.\-pr2  { padding-right: 20%; }
.liquid-padding.\-pr3  { padding-right: 30%; }
.liquid-padding.\-pr4  { padding-right: 40%; }
.liquid-padding.\-pr5  { padding-right: 50%; }
.liquid-padding.\-pr6  { padding-right: 60%; }
.liquid-padding.\-pr7  { padding-right: 70%; }
.liquid-padding.\-pr8  { padding-right: 80%; }
.liquid-padding.\-pr9  { padding-right: 90%; }
.liquid-padding.\-pr10 { padding-right: 100%; }

```

#### Helper `MARGIN` 

```css
.margin.\-p1  { margin: 0.25rem; }
.margin.\-p2  { margin: 0.50rem; }
.margin.\-p3  { margin: 0.75rem; }
.margin.\-p4  { margin: 1rem; }
.margin.\-p5  { margin: 1.25rem; }
.margin.\-p6  { margin: 1.5rem; }
.margin.\-p7  { margin: 1.75; }
.margin.\-p8  { margin: 2rem; }
.margin.\-p9  { margin: 2.25rem; }
.margin.\-p10 { margin: 2.5rem; }

.margin.\-pt1  { margin-top: 0.25rem; }
.margin.\-pt2  { margin-top: 0.50rem; }
.margin.\-pt3  { margin-top: 0.75rem; }
.margin.\-pt4  { margin-top: 1rem; }
.margin.\-pt5  { margin-top: 1.25rem; }
.margin.\-pt6  { margin-top: 1.5rem; }
.margin.\-pt7  { margin-top: 1.75; }
.margin.\-pt8  { margin-top: 2rem; }
.margin.\-pt9  { margin-top: 2.25rem; }
.margin.\-pt10 { margin-top: 2.5rem; }

.margin.\-pb1  { margin-bottom: 0.25rem; }
.margin.\-pb2  { margin-bottom: 0.50rem; }
.margin.\-pb3  { margin-bottom: 0.75rem; }
.margin.\-pb4  { margin-bottom: 1rem; }
.margin.\-pb5  { margin-bottom: 1.25rem; }
.margin.\-pb6  { margin-bottom: 1.5rem; }
.margin.\-pb7  { margin-bottom: 1.75; }
.margin.\-pb8  { margin-bottom: 2rem; }
.margin.\-pb9  { margin-bottom: 2.25rem; }
.margin.\-pb10 { margin-bottom: 2.5rem; }

.margin.\-pl1  { margin-left: 0.25rem; }
.margin.\-pl2  { margin-left: 0.50rem; }
.margin.\-pl3  { margin-left: 0.75rem; }
.margin.\-pl4  { margin-left: 1rem; }
.margin.\-pl5  { margin-left: 1.25rem; }
.margin.\-pl6  { margin-left: 1.5rem; }
.margin.\-pl7  { margin-left: 1.75; }
.margin.\-pl8  { margin-left: 2rem; }
.margin.\-pl9  { margin-left: 2.25rem; }
.margin.\-pl10 { margin-left: 2.5rem; }

.margin.\-pr1  { margin-right: 0.25rem; }
.margin.\-pr2  { margin-right: 0.50rem; }
.margin.\-pr3  { margin-right: 0.75rem; }
.margin.\-pr4  { margin-right: 1rem; }
.margin.\-pr5  { margin-right: 1.25rem; }
.margin.\-pr6  { margin-right: 1.5rem; }
.margin.\-pr7  { margin-right: 1.75; }
.margin.\-p8  { margin-right: 2rem; }
.margin.\-pr9  { margin-right: 2.25rem; }
.margin.\-pr10 { margin-right: 2.5rem; }

.liquid-margin.\-p1  { margin: 10%; }
.liquid-margin.\-p2  { margin: 20%; }
.liquid-margin.\-p3  { margin: 30%; }
.liquid-margin.\-p4  { margin: 40%; }
.liquid-margin.\-p5  { margin: 50%; }
.liquid-margin.\-p6  { margin: 60%; }
.liquid-margin.\-p7  { margin: 70%; }
.liquid-margin.\-p8  { margin: 80%; }
.liquid-margin.\-p9  { margin: 90%; }
.liquid-margin.\-p10 { margin: 100%; }

.liquid-margin.\-pt1  { margin-top: 10%; }
.liquid-margin.\-pt2  { margin-top: 20%; }
.liquid-margin.\-pt3  { margin-top: 30%; }
.liquid-margin.\-pt4  { margin-top: 40%; }
.liquid-margin.\-pt5  { margin-top: 50%; }
.liquid-margin.\-pt6  { margin-top: 60%; }
.liquid-margin.\-pt7  { margin-top: 70%; }
.liquid-margin.\-pt8  { margin-top: 80%; }
.liquid-margin.\-pt9  { margin-top: 90%; }
.liquid-margin.\-pt10 { margin-top: 100%; }

.liquid-margin.\-pb1  { margin-bottom: 10%; }
.liquid-margin.\-pb2  { margin-bottom: 20%; }
.liquid-margin.\-pb3  { margin-bottom: 30%; }
.liquid-margin.\-pb4  { margin-bottom: 40%; }
.liquid-margin.\-pb5  { margin-bottom: 50%; }
.liquid-margin.\-pb6  { margin-bottom: 60%; }
.liquid-margin.\-pb7  { margin-bottom: 70%; }
.liquid-margin.\-pb8  { margin-bottom: 80%; }
.liquid-margin.\-pb9  { margin-bottom: 90%; }
.liquid-margin.\-pb10 { margin-bottom: 100%; }

.liquid-margin.\-pl1  { margin-left: 10%; }
.liquid-margin.\-pl2  { margin-left: 20%; }
.liquid-margin.\-pl3  { margin-left: 30%; }
.liquid-margin.\-pl4  { margin-left: 40%; }
.liquid-margin.\-pl5  { margin-left: 50%; }
.liquid-margin.\-pl6  { margin-left: 60%; }
.liquid-margin.\-pl7  { margin-left: 70%; }
.liquid-margin.\-pl8  { margin-left: 80%; }
.liquid-margin.\-pl9  { margin-left: 90%; }
.liquid-margin.\-pl10 { margin-left: 100%; }

.liquid-margin.\-pr1  { margin-right: 10%; }
.liquid-margin.\-pr2  { margin-right: 20%; }
.liquid-margin.\-pr3  { margin-right: 30%; }
.liquid-margin.\-pr4  { margin-right: 40%; }
.liquid-margin.\-pr5  { margin-right: 50%; }
.liquid-margin.\-pr6  { margin-right: 60%; }
.liquid-margin.\-pr7  { margin-right: 70%; }
.liquid-margin.\-pr8  { margin-right: 80%; }
.liquid-margin.\-pr9  { margin-right: 90%; }
.liquid-margin.\-pr10 { margin-right: 100%; }

```

#### Helper `ALIGN` 

```css
.align.\-content-space-around  { align-content: space-around; }
.align.\-content-space-between  { align-content: space-between;}
.align.\-content-center  { align-content: center; }
.align.\-content-start  { align-content: flex-start; }
.align.\-content-end  { align-content: flex-start; }
.align.\-content-stretch  { align-content: stretch; }
.align.\-content-unset  { align-content: unset; }
.align.\-content-inherit  { align-content: inherit; }

.align.\-self-baseline  { align-self: baseline; }
.align.\-self-center  { align-self: center; }
.align.\-self-start  { align-self: flex-start; }
.align.\-self-end  { align-self: flex-start; }
.align.\-self-stretch  { align-self: stretch; }
.align.\-self-unset  { align-self: unset; }
.align.\-self-inherit  { align-self: inherit; }

.align.\-items-baseline  { align-items: baseline; }
.align.\-items-center  { align-items: center; }
.align.\--items-start  { align-items: flex-start; }
.align.\-items-end  { align-items: flex-start; }
.align.\-items-stretch  { align-items: stretch; }
.align.\-items-unset  { align-items: unset; }
.align.\-items-inherit  { align-items: inherit; }


.justify-center  { justify-content: center; }
.justify-left  { justify-content: left; }
.justify-right  { justify-content: right; }
.justify-space-around  { justify-content: space-around; }
.justify-space-between  { justify-content: space-between; }
.justify-start  { justify-content: start; }
.justify-end  { justify-content: start; }
.justify-stretch  { justify-content: stretch; }
.justify-unset  { justify-content: unset; }
.justify-inherit  { justify-content: inherit; }
.justify-safe  { justify-content: safe; }
.justify-space-around  { justify-content: unsafe; }

.justify-self-center  { justify-self: center; }
.justify-self-left  { justify-self: left; }
.justify-self-right  { justify-self: right; }
.justify-self-space-around  { justify-self: space-around; }
.justify-self-space-between  { justify-self: space-between; }
.justify-self-start  { justify-self: flex-start; }
.justify-self-end  { justify-self: flex-start; }
.justify-self-stretch  { justify-self: stretch; }
.justify-self-unset  { justify-self: unset; }
.justify-self-inherit  { justify-self: inherit; }

.justify-items-center  { justify-items: center; }
.justify-items-left  { justify-items: left; }
.justify-items-right  { justify-items: right; }
.justify-items-space-around  { justify-items: space-around; }
.justify-items-space-between  { justify-items: space-between; }
.justify-items-start  { justify-items: flex-start; }
.justify-items-end  { justify-items: flex-start; }
.justify-items-stretch  { justify-items: stretch; }
.justify-items-unset  { justify-items: unset; }
.justify-items-inherit  { justify-items: inherit; }

```

#### Helper `SIZING` 

```css
.area-min {min-height: 0; min-width: 0}
.area-max {max-height: 100%; max-width: 100%}

.area-min {min-height: 0; min-width: 0}
.area-max {max-height: 100%; max-width: 100%}

.width-zero { width: 0 }
.width-full { width: 100% }
.width-em { width: 1em }
.width-rem { width: 1rem }
.width-viewport { width: 100vw }
.width-auto { width: auto }

.height-zero { height: 0 }
.height-full { height: 100% }
.height-em { height: 1em }
.height-rem { height: 1rem }
.height-viewport { height: 100vh }
.height-auto { height: auto }

.max-none { max-width: none; max-height: none }
.max-zero { max-width: 0; max-height: 0 }
.min-zero { min-width: 0; min-height: 0 }
.min-auto { min-width: auto; min-height: auto }
.max-viewport { max-width: 100vw; max-height: 100vh }
.min-viewport { min-width: 100vw; min-height: 100vh }

.width-free { max-width: none }
.width-fit { max-width: 100% }
.width-clip { max-width: 0 }
.width-force { min-width: 100% }

.height-free { max-height: none }
.height-fit { max-height: 100% }
.height-clip { max-height: 0 }
.height-force { min-height: 100% }

```
##### [classes](area.css)

###### `width`

- `.width-zero` sets width to `0`
- `.width-full` sets width to `100%`
- `.width-em` sets width to `1em`
- `.width-rem` sets width to `1rem`
- `.width-viewport` sets width to `100vw`
- `.width-auto` sets width to `auto`

###### `height`

- `.height-zero` sets height to `0`
- `.height-full` sets height to `100%`
- `.height-em` sets height to `1em`
- `.height-rem` sets height to `1rem`
- `.height-viewport` sets height to `100vh`
- `.height-auto` sets height to `auto`

###### `max`
- `.max-none` sets maxes to `none`
- `.max-zero` sets maxes to `0`
- `.max-viewport` sets maxes to viewport size
- `.width-free` sets max-width to `none`
- `.height-free` sets max-height to `none`
- `.width-fit` sets max-width to `100%`
- `.height-fit` sets max-height to `100%`
- `.width-clip` sets max-width to `0`
- `.height-clip` sets max-height to `0`

###### `min`
- `.min-zero` sets mins to `0`
- `.min-auto` sets mins to `auto`
- `.min-viewport` sets mins to viewport size
- `.width-force` sets min-width to `100%`
- `.height-force` sets min-height to `100%`

###### usage

```html
<img class="width-fit height-auto" src="example.png" alt="example">
```

#### Helper`HEADING` 

```css



```

#### Effect`DISPLAY` 

```css



```

#### Effect`OPACITY` 

```css



```

#### Effect`COLORS` 

```css



```

#### Effect`PERSPECTIVE` 

```css



```


#### Effect`SHADOWS` 

```css



```

#### Ui-Component`ALL` 

Alert
```css



```

Badge

```css



```

Breadcrumb

```css



```

Button

```css



```

Buttons

```css



```

Dropdown

```css



```

Form
```css



```

Form-label
```css



```

Form-input
```css



```

Form-checkbox
```css



```

Form-radio
```css



```

Form-select
```css



```

Form-range
```css



```


Form-date
```css



```

Icon
```css



```

Icons
```css



```

Placeholders
```css



```

Popovers
```css



```

Progress
```css



```

Tooltip
```css



```


#### Layout-Component`ALL` 

Page

```css



```

Header

```css



```

Footer

```css



```

Main-content

```css



```

Nav

```css



```

Tab

```css



```

Img

```css



```

Figure

```css



```

Bar-side

```css



```

Bar-bottom

```css



```

Bar-top

```css



```

Modal

```css



```

List

```css



```

Table

```css



```

## Features Examples


## Changelog
- 1.0.0.alpha: Currently
