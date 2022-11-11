# Responsive-layouts
Learning repsonsive layouts with kevin powell

## Use Percentages:
- Giving width in percentages keeps the layout responsive.
- Percentage given to a child is actually that percent  of the parent, i.e., if width of a hild is 80% then it's 80% of the parent. 


### NOTE: Web is responsive by default, it's our css that makes it non responsive.


## Avoid Heights:
- Heights can cause child to overflow vertically so avoid giving heights to the parent.

## EM vs REM

### em:
- BY DEFAULT: 1em = 16px.
- Child div's em changes in proprtion to the parent div,i.e., it works in a compounding way for font size.
- Example: 
  - Here font-size of grid is 16 x 2 = 32px
  - Which will be proportionaly inherited by the child (col--em), which    makes font size of col--em : 32 x 1.5 = 48px
  - Similarly, font-size of col--em-h1: 48 x 2 = 96px.
  - And like that it could go out of control if ont used carefully.
![em-example](em.png)   

- For any other property except for font-size(like margin, padding etc.) it sees the font size of the current div.
  - Here margin will be  2.5 x 1 = 2.5em  
  ![em-example-2](em-2.png)
- **Good** for using in elements like **buttons** to keep parameters prop0rtional just by changing the font-size.


### rem:
- rem(root em) is same as em, that is, 1rem = 16px.
- But it solves the problem of compounding in em.
- It only changes according to the font-size of the root/html.