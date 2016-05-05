# Menu Animation

###### Sandbox
Simple animations on element :before for menu hover with CSS3

[Demo](http://www.theomesnil.com/demo/MenuAnimation/) / [Direct Download](http://www.theomesnil.com/demo/MenuAnimation/MenuAnimation.zip)

![alt text](http://www.theomesnil.com/data/images/MenuAnimation.gif "theomesnil.com")

## How to contribute

1. Fork this repo
2. Edit the `index.html` and `menu-animation.css`

##### index.html

```html
<section class="navigation navigation-NEXT-NUMBER">
  <div class="title">Menu | NEXT-NUMBER</div>
  <ul>
    <li class="active"><a href="#">Home</a></li>
    <li><a href="#">Gallery</a></li>
    <li><a href="#">Shop</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</section>
```

##### css/menu-animation.css

```css
/***/
/*** NEXT-NUMBER ***/

.navigation-NEXT-NUMBER li a {
  transition: color 500ms ease-in-out;
}
.navigation-NEXT-NUMBER li a::before {
  height: 3px;
  background: #00A29A;
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  transform: scale3d(0, 1, 1);
  transition: transform 500ms;
}
.navigation-NEXT-NUMBER li:hover a {
  color: #00A29A;
}
.navigation-NEXT-NUMBER li.active a::before {
  transform: scale3d(1, 1, 1);
  transition: transform 500ms cubic-bezier(.57,1,.3,1.73);
}
```

And push to create a pull request

## ![alt text](https://avatars2.githubusercontent.com/u/11488084?v=3&s=25 "theomesnil.com") About me

Follow me on [Twitter](https://twitter.com/theomesnil) - [Github](https://github.com/mesniltheo) -  [Dribbble](https://dribbble.com/theomesnil)

[© Théo Mesnil - 2016](http://www.theomesnil.com)
