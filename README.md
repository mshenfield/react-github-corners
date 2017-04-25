# React Github Corners
A small React wrapper around [@tholman](https://github.com/tholman)'s [github-corners](https://github.com/tholman/github-corners). See [the example site](http://tholman.com/github-corners/) to see the corner live with the smal animations.

## Installation
Add `react-github-corners` to your project from npm using your favorite package management tool

## Usage
If you have [Webpack](https://webpack.js.org/) configured to [load CSS](https://webpack.github.io/docs/stylesheets.html) and [transpile JSX](https://github.com/babel/babel-loader), this can simply be imported and used. This also plays nice with [create-react-app](https://github.com/facebookincubator/create-react-app).

```js
import GithubCorner from 'react-github-corners'

const App = (props) => (<GithubCorner/>)
```

You can override the color using the `color` and `backgrounColor` props:

```js
const App = (props) => (<GithubCorner color="orange" backgroundColor="white"/>)
```

Class names try to follow [BEM](http://getbem.com/introduction/) principles, so you can dig around the source code to find the class names and take direct control of the components using plain CSS. You can also override the SVG style by passing an `svgStyle` attribute to your component:

```js
const App = (props) => (<GithubCorner svgStyle={{"stroke": "blue"}})
```

If you want to help this library support other build configurations, [file an issue](issues).

## API
**Props**

`url` _(required)_: the URL of your project, e.g. https://github.com/github/gitignore

`backgroundColor` _(default: `"black"`)_: the background color of the corner

`color` _(default: `"white"`)_: the color of the octocat

`svgStyle` _(default: `{}`)_: override the style of the SVG

`target` *(default: `"_self"`)* : override the target attribute of the link

## License
From [github-corners](https://github.com/tholman/github-corners)
> Naturally, these aren't built by GitHub, or endorsed by them.

Ditto for this.

Copyright (c) 2016 Tim Holman
