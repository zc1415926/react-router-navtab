# React Router Navtab
A wrapper of the Link tab in React Router to make navigation bar have an active style. See the detail: https://zc1415926.github.io/react-router-navtab/

##You can use it easily
```js
npm install --save react-router-navtab

//and import it
var NavTab = require('react-router-navtab');

//then use it in a Bootstrap navigation bar
<ul className="nav navbar-nav">
    <NavTab to="/">Home</NavTab>
</ul>
```

##Extends the Link tab of the React Router
It only can genterate an a tab, using the Link tab built in React Router. 
```js
//use a Link in React
<Link to="/">Home</Link>

//an a tab you can get
<a href="/">Home</a>
```
To make navigation tab(button) be actived, there should be a li tab on the outside of the a tab,
when coding a navigation bar of the website using Bootstrap.
```js
//You need a li tab with a "active" to active navigation tab
<li class="active">
    <a href="/">Home</a>
</li>
```

Put li tab outside every Link tab?
```js
<li className="active">
    <Link to="/">Home</Link>
</li>
```
No, We wrap it！

Then you can build a navigation bar using React Router Navtab.

##Reference
I build the React Router Navtab refer to the [Nav Link Wrappers](https://github.com/reactjs/react-router-tutorial/tree/master/lessons/05-active-links#nav-link-wrappers).
