# sleeker

A atomic-class CSS library, closer to css syntax

## status:
This library is not stable yet. We do not recommend using it in production. Expect breaking changes before version v1.0.0

## Setup:

‍‍‍‍‍‍‍`npm i sleeker‍‍‍‍‍‍‍`

import sleeker variables and atomic classes in the root of your project

‍‍‍‍‍‍‍`import 'sleeker/variables.css'‍‍‍‍‍‍‍`
‍‍‍‍‍‍‍`‍import 'sleeker/atomic-classes.css'‍‍‍‍‍‍‍`

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

`justify-content:center` ---> `js:center`

`background-color:red` ---> `bg:red`

`border-color:blue` ---> `br:blue`

`border-radius:l` ---> `rd:l`


## List of classes 

### sizes (t-shirt sizes)


 #### padding 

 pd (to get the default sizes do not write pd:m or pd:md. just write `pd` )

 pd:s pd:xs pd:2xs ... pd:9xs

 pd:l pd:xl pd:2xl ... pd:9xl


 padding-block ---> pd-bl

 padding-inline-start ---> pd-inl-start:4xs

 padding-block-end ---> pd-bl-end:xl

 #### gap: 

 gap 

 gap:s gap:xs gap:2xs ... gap:9xs

 gap:l gap:xl gap:2xl ... gap:9xl


 column-gap ---> col-gap

 row-gap ---> row-gap:4xs

#### border-radius

 rd 

 rd:s rd:xs rd:2xs ... rd:9xs

 rd:l rd:xl rd:2xl ... rd:9xl


#### font-size:

 fs 

 fs:s fs:xs fs:2xs ... fs:9xs

 fs:l fs:xl fs:2xl ... fs:9xl

 #### line-spacing:

 ls

 ls:s ls:xs

 ls:l ls:xl

#### margin: 

 mg 

 mg:s mg:xs mg:2xs ... mg:9xs

 mg:l mg:xl mg:2xl ... mg:9xl

 margin-block ---> mg-bl:s 

 margin-inline-start ---> mg-inl-start:9xs

 margin-block-end ---> mg-bl-end

#### box-shadow:

bx-shd

bx-shd:s

bx-shd:l 

bx-shd:modal

### sizes (with unit)

#### border-width 

br-w:1px br-w:2px  ... br-w:10px

br-w:0.1em br-w:0.2em  ... br-w:1em

br-w:0.1rem br-w:0.2rem  ... br-w:1rem


#### outline-width:

outl-w:1px outl-w:2px  ... outl-w:10px

outl-w:0.1em outl-w:0.2em  ... outl-w:1em

outl-w:0.1rem outl-w:0.2rem  ... outl-w:1rem


#### outline-offset:

outl-offset:1px outl-offset:2px  ... outl-offset:10px

outl-offset:0.1em outl-offset:0.2em  ... outl-offset:1em

outl-offset:0.1rem outl-offset:0.2rem  ... outl-offset:1rem


### colors 

** we use radix colors. **

expect this to be changed while sleeker is not stabled if we found a better coloring system.
radix colors have built in dark mode. each scale has 12 shades. 

Each shade has a purpose. 12 is for normal (high contrast) text and 11 is for low contrast text.
got to [radix color docs](https://www.radix-ui.com/colors) to see where to use each shad.

scales: Tomato, Red, Crimson, Pink, Plum , Purple, Violet, Indigo, Blue, Cyan, Teal, Green, Grass, Orange, Brown

Bright scales: Sky, Mint, Lime, Yellow, Amber

gray scales: Gray, Mauve, Slate, Sage, Olive, Sand

metal scales: Gold, Bronze

#### color: (setting text-color/currentColor)

  clr:red clr:red1 clr:red2 ... clr:red12 (same for all scales)

#### background-color:

  bg:red bg:red1 bg:red2 ... bg:red12 (same for all scales)

#### border-color:

  br:red br:red1 br:red2 ... br:red12 (same for all scales)

#### outline-color:

  outl:red outl:red1 outl:red2 ... outl:red12 (same for all scales)

### layout:


#### display:

d:bl d:inl d:inl-bl d:flex d:inl-flex d:grid d:inl-grid d:flow-root d:none d:content d:list-item d:table d:table-row

#### position:

pos:static pos:rel pos:fixed pos:abs pos:sticky

### typography:

#### font-weight:

fw:50 fw:100 fw:200 fw:300 fw:400 fw:500 fw:600 fw:700 fw:800 fw:900 fw:950 fw:1000

#### line-spacing:

ls

ls:s ls:xs

ls:l ls:xl

#### text-align:

tx-align:center

text-align:start text-align:end 

text-align:left text-align:right 

text-align:justify text-align:justify-all 

text-align:match-parent

#### object-fit:

obj-fit:contain obj-fit:cover obj-fit:fill obj-fit:none

#### border-collapse:

br-collapse:collapse br-collapse:separate

#### border-style:

br-style:none br-style:hidden br-style:dotted br-style:dashed br-style:solid br-style:double br-style:groove br-style:ridge br-style:inset br-style:outset

#### outline-style:

outl-style:none outl-style:auto outl-style:dotted outl-style:dashed outl-style:solid outl-style:double outl-style:groove outl-style:ridge outl-style:inset outl-style:outset

### flex related properties

#### display:flex

d:flex d:inl-flex

#### flex-direction:

flex-dir:row flex-dir:row-reverse flex-dir:column flex-dir:column-reverse

#### justify-content:

jc:start jc:end jc:center jc:space-between jc:space-around jc:space-evenly

#### align-items:

ai:start ai:end ai:center ai:baseline ai:stretch 

#### align-content:

ac:start ac:end  ac:normal  ac:center ac:baseline ac:first-baseline ac:last-baseline  ac:space-between ac:space-around ac:space-evenly ac:stretch

#### flex-wrap:

flex-wrap:wrap flex-wrap:nowrap flex-wrap:wrap-reverse 

#### flex:

flex:0

flex:0.1 flex:0.2 flex:0.3 flex:0.4 flex:0.5 flex:0.6 flex:0.7 flex:0.8 flex:0.9 

flex:1

flex:2 flex:3 flex:4 flex:5 flex:6 flex:7 flex:8 flex:9 flex:10 

#### flex:basis: 

flex-basis:auto, flex-basis:min-content, flex-basis:max-content, flex-basis:fit-content 

flex-basis:0

flex-basis:5% flex-basis:10% flex-basis:15% ... flex-basis:90% flex-basis:95% flex-basis:100% 

#### flex-grow: 

flex-grow:0

flex-grow:01 flex-grow:02 ... flex-grow:08 flex-grow:09 

flex-grow:1 flex-grow:2 ... flex-grow:8 flex-grow:9 flex-grow:10 

#### flex-shrink:

flex-shrink:0

flex-shrink:01 flex-shrink:02 ... flex-shrink:08 flex-shrink:09 

flex-shrink:1 flex-shrink:2 ... flex-shrink:8 flex-shrink:9 flex-shrink:10


#### order:

order:0 

order:1 order:2 ... order:8 order:9 order:10 

order:-1  order:-2 ... order:-8 order:-9 order:-10 

#### align-self:

align-self:auto  align-self:normal  align-self:center  align-self:start  align-self:end  align-self:self-start  align-self:self-end align-self:flex-start align-self:flex-end  align-self:baseline  align-self:first-baseline  align-self:last-baseline  align-self:stretch  

### other properties

#### all:

all:unset all:initial all:inherit all:revert all:revert-layer 

#### top:

top:auto

top:100% top:99% top:98% top:97% top:96% top:95% top:90%

top:85% top:80% top:75% ... top:15% top:10% top:5% 

top:4% top:3% top:2% top:1% 

#### bottom:

bottom:auto

bottom:100% bottom:99% bottom:98% bottom:97% bottom:96% bottom:95%

bottom:90% bottom:85% bottom:80% bottom:75% ... bottom:15% bottom:10% bottom:5% 

bottom:4% bottom:3% bottom:2% bottom:1% 

#### left:

left:auto

left:100% left:99% left:98% left:97% left:96% left:95%

left:90% left:85% left:80% left:75% ... left:15% left:10% left:5% 

left:4% left:3% left:2% left:1% 

#### right:

right:auto

right:100% right:99% right:98% right:97% right:96% right:95% 

right:90% right:85% right:80% right:75% ... right:15% right:10% right:5% 

right:4% right:3% right:2% right:1% 

#### overflow

overflow:hidden overflow:scroll overflow:auto overflow:visible overflow:clip 

overflow-x:hidden overflow-x:scroll overflow-x:auto overflow-x:visible overflow-x:clip 

overflow-y:hidden overflow-y:scroll overflow-y:auto overflow-y:visible overflow-y:clip 

#### table-layout:

table-layout:auto

table-layout:fixed

#### vertical-align:


vertical-align:baseline vertical-align:sub vertical-align:super vertical-align:text-top vertical-align:text-bottom vertical-align:middle vertical-align:top vertical-align:bottom 

vertical-align:1px vertical-align:2px vertical-align:3px ... vertical-align:9px vertical-align:10px 

vertical-align:0.1rem  vertical-align:0.2rem  vertical-align:0.3rem  ...  vertical-align:0.9rem  vertical-align:1rem 

vertical-align:0.1em

vertical-align:0.2em vertical-align:0.3em ... vertical-align:0.9em vertical-align:1em

#### writing-mode:

writing-mode:horizontal-tb 

writing-mode:vertical-rl

writing-mode:vertical-lr