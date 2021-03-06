# AndcultureCode.Scss.Grid

[![Build Status](https://travis-ci.org/AndcultureCode/AndcultureCode.Scss.Grid.svg?branch=master)](https://travis-ci.org/AndcultureCode/AndcultureCode.Scss.Grid)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

A Sass (scss) based grid library inspired by bourbon neat and flexbox.

Written by Zach McCleaf.

Published by Dylan Justice.

# Getting Started

```shell
#npm
npm install --save-dev andculturecode-scss-grid

# yarn
yarn add andculturecode-scss-grid --dev
```

```scss
@import andculturecode-scss-grid;
```

# Usage

```html
<div class="o-grid__container">
    <div class="o-grid__row -space-above"></div>
    <div class="o-grid__row -space-between"></div>
    <div class="o-grid__row -border-bottom"></div>
    <div class="o-grid__row">... More to come</div>
    <div class="o-grid__row">
        <div class="o-grid__col -span-one"></div>
        <div class="o-grid__col -span-two"></div>
        <div class="o-grid__col -span-twelve"></div>
    </div>
    <div class="o-grid__row">
        <div class="o-grid__col -push-one"></div>
        <div class="o-grid__col -push-eleven"></div>
    </div>
    <div class="o-grid__row">
        <div class="o-grid__col -span-one -y-align-top"></div>
        <div class="o-grid__col -span-one -y-align-center"></div>
        <div class="o-grid__col -span-one -y-align-bottom"></div>
        <div class="o-grid__col -span-one -justify-right"></div>
        <div class="o-grid__col -span-one -justify-center"></div>
    </div>
</div>
```

Add a Custom grid!

```scss
$my-custom-grid: (
        columns: 12,
        gutter: 20px
    )
    .c-row-of-stuff {
    &__column {
        @include span-col(8, $my-custom-grid);
    }
}
```

Add your own breakpoints

```scss
$breakpoints: (
        "phone": 480px,
        "tablet": 768px,
        "desktop": 1180px
    )
    .c-row-of-stuff {
    &__column {
        @include span-col(8, $my-custom-grid);

        @include respond-to("phone") {
            @include span-col(12, $my-custom-grid);
        }
    }
}
```

## Development

```shell
npm install
npm run watch # automatically builds as changes are made
```

## Documentation

[Full documentation](https://andculturecode.github.io/AndcultureCode.Scss.Grid/docs)

# Community

[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/0)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/0)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/1)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/1)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/2)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/2)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/3)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/3)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/4)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/4)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/5)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/5)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/6)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/6)[![](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/images/7)](https://sourcerer.io/fame/andCulture/AndcultureCode/AndcultureCode.Scss.Grid/links/7)

# Contributing

Information on contributing to this repo is in the [Contributing Guide](CONTRIBUTING.md)
