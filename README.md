# Hover Block Animation

###### Sandbox
Animations on hover on blocks elements with background image - made with CSS3

[Demo](http://www.theomesnil.com/demo/HoverBlockAnimation/) / [Direct Download](http://www.theomesnil.com/demo/HoverBlockAnimation/HoverBlockAnimation.zip)

<img src="https://github.com/mesniltheo/HoverBlockAnimation/blob/master/og-img.jpg?raw=true">

## How to contribute

1. Fork this repo
2. Edit the `index.html` and `hover-block-animation.css`

##### index.html

```html
<section>
  <div class="title">Block | 1</div>
  <div class="block block-1">
    <div class="block-image">
    </div>
    <div class="block-text">
      <div class="block-text-center">
        <div>
          Lorem impsum dolor sit amet
        </div>
      </div>
    </div>
  </div>
</section>
```

##### css/hover-block-animation.css

```css
/***/
/*** 1 ***/

.block-1 {
  transition: transform 500ms;
}
.block-1:hover {
  transform: scale(.95);
  transition: transform 500ms;
}
.block-1 .block-image {
  background-image: url('../images/block1.jpeg');
}
.block-1 .block-text {
  height: 100px;
  background: linear-gradient(to bottom, rgba(0,0,0,0) 0%,rgba(0,162,164,0.8) 100%);
  transition: opacity 300ms;
  bottom: 0;
  top: auto;
}
.block-1:hover .block-text {
  opacity: 1;
  transition: opacity 1000ms;
}
.block-1 .block-text-center div {
  opacity: 0;
  color: white;
  padding-left: 40px;
  font-size: 25px;
  transform: translate(0, 10px);
  transition: opacity 200ms, transform 300ms;
}
.block-1:hover .block-text-center div {
  opacity: 1;
  transition: opacity 300ms, transform 500ms;
  transform: translate(0, 0);
  transition-delay: 100ms;
}
@media screen and (max-width: 640px) {
  .block-1 .block-text-center div {
    font-size: 15px;
    padding-left: 20px;
  }
  .block-1 .block-text {
    height: 50px;
  }
}
```

And push to create a pull request

## Ressources

Pictures from [unsplash](https://unsplash.com)

## ![alt text](https://avatars2.githubusercontent.com/u/11488084?v=3&s=25 "theomesnil.com") About me

Follow me on [Twitter](https://twitter.com/theomesnil) - [Github](https://github.com/mesniltheo) -  [Dribbble](https://dribbble.com/theomesnil)

[© Théo Mesnil - 2016](http://www.theomesnil.com)
