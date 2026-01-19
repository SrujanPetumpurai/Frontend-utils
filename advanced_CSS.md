# Advance CSS PROPERTIES
## Attributes
In a HTML tag custom made contributes are like this, data-*
ex:
<img src='/image' alt='boxer' data-user='muhamed' />
-- Here src and alt are attributes and data-user is cutom made attribute, they are used to control element or data of the element and custom attributes are for storing developer data.

## Filter
-- Adds visual effects to the element itself.
- Values:
  - blur(px) → blur effect
  - brightness(%) or (number) → lighter/darker
  - contrast(%) → increase/decrease contrast
  - grayscale(%) → black & white
  - invert(%) → invert colors
  - sepia(%) → brown old-photo look
  - saturate(%) → color intensity
  - hue-rotate(deg) → rotate colors
  - drop-shadow(x y blur color) → shadow (like box-shadow but for image shape)
- Example:
  - img{filter:blur(5px) grayscale(100%)}

## Background-filter
-- Applies effect to element behind the element(glass blur)
- Values:
  - blur(px)
  - brightness()  
  - contrast()  
  - grayscale()  
  - sepia()  
  - saturate()  
  - hue-rotate() 

- The element needs to be transparent to look at the effects of the bg.

## Scroll-behaviour
-- controls how scrolling happens
- Values:
  - auto -- instant jump(default)
  - smooth -- animated smooth scroll
- Example:
  - `html{scroll-behaviour:smooth}`
##  Visibility
-- Hides or shows element without removing space
- Values:
  - visibile -- Shown
  - hidden -- invisible but space remains
  - collapse -- collapses rows/collumns (tables)

## Pseudo-elements
-- Why use pseudo-elements?
  - Add icons without HTML
  - Decorative lines
  - Overlays
  - Badges
  - Tooltips
  - Custom UI parts

-- They let you style or create parts of an element that don’t exist in HTML.
- Values:
  - ::before
  - ::after  
  - ::first-letter(styles the first letter of text)
  - ::first-line (styles only the first line of text)
  - ::selection (styles highlighted/selected text)
  - ::marker  (styles list bullets or numbers)
  - ::placeholder(styles input placeholder text)
- Example:
  - `button::before {content: "→ ";}`
- Values content can be:
  - Text ('Hello')
  - attr() -- Used when text already exists in attributes
    - example:
     ```js
        <p data-text='Hello boy'></p>
    p::before{
        content:attr(data-text)
    }
    ```
  - url() -- Inserts an image using css(Used for icons without adding <img> tag.)
    - example: `.icon::before {content: url("icon.png");}`
  - Empty ('') -- For styling
   ```js 
    .h1::after {
        content: "";
        display: block;
        width: 50px;
        height: 4px;
        background: red;
        } //A red line comes, because you put it as block it comes below it
    .card::before {
        content: "";
        position: absolute;
        inset: 0;(top/right/left/bottom =0)
        background: rgba(0,0,0,0.4);
        }
    .btn::before {
        content: "";
        width: 16px;
        height: 16px;
        background: url(icon.svg) no-repeat center/contain;
        display: inline-block;
        }
 
        ```



    