# sleeker

A utility-class CSS library, closer to css syntax

## Setup:

‍‍‍‍‍‍‍`npm i sleeker‍‍‍‍‍‍‍`

import sleeker variables and utility classes in the root of your project

‍‍‍‍‍‍‍`import 'sleeker/variables.css'‍‍‍‍‍‍‍`
‍‍‍‍‍‍‍`‍import 'sleeker/utility-classes.css'‍‍‍‍‍‍‍`

## Usage

sleeker classes are like css rules.
For example, to apply ‍‍‍‍‍‍‍`‍background:red` to a button, do this:
‍‍‍‍‍‍‍`‍<button class="bg:red">I have red background</button>`

## Classes

sleeker provides a compact syntax that is close to CSS and easy to remember. 

** Sleeker rule of thumb: To apply a rule add that rule in class attribute. If there is compact version for the property, use compact version. **

### case 1 - No compact version - exactly like css

for example, to get apply `overflow : hidden ; ` , add ` overflow:hidden ` to the class attribute.

## case 2 - compact version for a css word
if a css word has compact version (for example `dir` is compact version of `direction`), replace css word with compact version in all hyphen separated cases.
`direction:rtl` ---> `dir:rtl`
`flex-direction:row` ---> `flex-dir:row`

## case 3 - compact version for a multiple css words
Sometime (for better DX) two css word are compacted together. 
`font-weight:700` ---> `fw:700`
`background-color:red` ---> `bg:red`
`border-color:blue` ---> `br:blue`
`border-radius:l` ---> `rd:l`


## List of classes (in order of usage frequency)


### sizes (t-shirt sizes)
 padding 
 pd 
 pd:s pd:xs pd:2xs ... pd:9xs
 pd:l pd:xl pd:2xl ... pd:9xl

border-radius
 rd 
 rd:s rd:xs rd:2xs ... rd:9xs
 rd:l rd:xl rd:2xl ... rd:9xl

font-size:
 fs 
 fs:s fs:xs fs:2xs ... fs:9xs
 fs:l fs:xl fs:2xl ... fs:9xl

 line-spacing
 ls
 ls:s ls:xs
 ls:l ls:xl

margin: 
 mg 
 mg:s mg:xs mg:2xs ... mg:9xs
 mg:l mg:xl mg:2xl ... mg:9xl

box-shadow:
bx-shd bx-shd:s bx-shd:l bx-shd:xl

### sizes (pixel sizes)

border-width 
br-w:1px br-w:2px  ... br-w:10px
br-w:0.1em br-w:0.2em  ... br-w:1em
br-w:0.1rem br-w:0.2rem  ... br-w:1rem


outline-width:
outl-w:1px outl-w:2px  ... outl-w:10px
outl-w:0.1em outl-w:0.2em  ... outl-w:1em
outl-w:0.1rem outl-w:0.2rem  ... outl-w:1rem

outline-offset:
outl-offset:1px outl-offset:2px  ... outl-offset:10px
outl-offset:0.1em outl-offset:0.2em  ... outl-offset:1em
outl-offset:0.1rem outl-offset:0.2rem  ... outl-offset:1rem