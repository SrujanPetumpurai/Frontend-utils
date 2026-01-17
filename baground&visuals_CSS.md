# Background && Visuals
## Background Image
1.background-image:`.box{background-image:url('image.jpg')}`
2.background-size -- controls how the background image scales
  - `.box{background-size:cover |contain|100px 200px }`
  - image fills box,may crop | image fully visible , may leave space 
3.background-position -- controls where the image sits
  - `.box{background-position:center | top right | 50% 20px}
  - first x value second y value
4.background-repeat -- controls tiling of the image
  - `.box{background-repeat:repeat|no-repeat|repeat-x|repeat-y}`
  - repeat image(default)|single image only|repeat in the horizontal direction|repeat in the vertical direction

## Gradient
- Gradients are treated as background images
1.linear `linear-gradient(direction,color-stop1,color-stop2,...)` 
  - Values for direction: to right, to top, to left, to bottom, to top right
  Or Angles:0deg(bottom to top), 90deg(left to right), 180deg(top to bottom),270deg(right to left)
  - Values for colors: red 30% , blue 70% -- red occupies from 0 to 30% completely, blue occupies from 70 to 100% completely and then the blend happens inbetween
2.radial-gradient() `radial-gradient(shape size at position,color-stop1,color-stop2,...)
  - shape: circle, ellipse(default)
  - size :closest-side|farthest-side|closest-side|farthest-corner (default)
  - position:center | top | left | right | 50% 50%
  - ex: `.box{radial-graident(circle at center,red,blue)}`
3.repeating-gradient:
  - linear-graident(to right, red 0 20px, blue 20px 40px) -- red starts from 0 to 20 and blue start from 20 to 40 , and the pattern keep on repeating creating stips
## Box-shadow
- Adds shadow to an element box `box-shadow:x-offset y-offset blur spread color intact`
  - 10px  (x-offset: right / left) | 5px     (y-offset: down / up) | 20px    (blur radius) | 0px     (spread) | rgba(0,0,0,0.3)  (color) | inset   (optional: inner shadow) 
## Opacity
`opacity:value` 0,0.5,1
- *background transparent* `background-color:rgba(0,0,0,0.5)`