# Responsive

1.@media
  - ```js
   @medica(max-width:768px){  //Apply this when width is equal or smaller then 768px
   .box{width:100%}
   }
  ```
2.aspect-ratio -- controls width height ratio of a element
  - ```js
  .box{
    width:200px;
    aspect-ratio:1/1; //Height become 1
  }
   ```
  - common use is for image and video

3. object-fit:value
  - Values:fill(fills the box but may distor) | contain(shows full image, keeps ratio, may leave empty space) | cover(fills box crops extra parts) | none | scale-down(uses none or cotain)
  - we have object-position too.

4. clamp -- response values with limits
  - clamp(min,preferred,max)
  - .box{font:clamp(14px,2vw,20px)} -- 14px minimum size, 20px max, and most 2vw.
  
