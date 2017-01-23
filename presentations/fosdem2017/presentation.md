
class: center, middle

<img class=fullscreen src=images/logo.png />

---



![](images/bls_125_banner.gif)

In the US: 
- 1,114,000 Software Developers
- 315,900 Electrical and Electronic Engineers


![](images/reddit.jpg)

Reddit: 
- /r/programming 720,000 subscribers
- /r/electronics 66,000 subscribers

---

# Where is the Linux of electronics?

<img style="height:400px;float:right" src=images/ohr_logo.svg />

---

# We do share projects 
- GitHub
  - 3000 KiCAD Projects
  - 7000 Eagle Projects

- OshPark
  - Over 9000 shared projects

- Hackaday.io, EEVblog Forums, etc

---
<br>
<br>
<br>
<center><img src=images/pease.jpg /></center>

---
<img class=fullscreen src=images/meat1.jpg />

---
<img class=fullscreen src=images/meat2.jpg />
---
<img class=fullscreen src=images/meat3.jpg />

---
<img src=images/1_click_logo.png />1-click BOM browser extension

<img src=images/kitnic_logo.png />kitnic.it

<center>
<img class=fullscreen src=images/meat_apart.jpg>
</center>
---
# 1-click BOM extension 

- Replicate the web requests that are sent when you use retailer sites.
  - Digikey 
  - Mouser 
  - RS
  - Newark / Farnell / Element14
---
#Same origin policy

"The same-origin policy restricts how a document or script loaded from one origin can interact with a resource from another origin." - MDN

---

<img class=fullheight src=images/cors.jpeg />

---
```
curl
'http://uk.mouser.com/ProductDetail/Cree-Inc/CGHV96100F2/?Cree-Inc
%2fCGHV96100F2%2f&qs=sGAEpiMZZMvplms98TlKY6zbNRoARc
Ug8gg333Al67kStE%252bN8N0%2fKg%3d%3d'
-H 'Cookie: g11n=Up9NRXFGLVs=;
ME_Main=&ME_DSN=kJ0slznDUsNJMyNjQRiw8Q==&ME_DSU=YyaQEeoCnLc=;
ASP.NET_SessionId=zxtlgy45oobekaaphyv5n0z1;
_op_aixPageId=a2_60d31424-8123-4e84-b3f9-a18a6f8bfc3d-3648-87767;
CARTCOOKIEUUID=c46df9ef-39bb-4ada-bfcd-2452ed49bc8a; _gat=1;
__ar_v4=5UM3NRP3LFFG5JUPQ2VEXA%3A20150203%3A12%7CVPQ73SPSLBEPXM7QJ2MJRL%3A20150203%3A12%7CA463QQQT6VD37AVLWC4RZU%3A20150203%3A12;
SDG1=12; SDG2=40; SDG3=0; preferences=ps=gb&pl=en-GB&pc_gb=GBP;
_ga=GA1.2.91020740.1409853093;
__utma=261309969.91020740.1409853093.1417720020.1422769855.8;
__utmb=261309969.15.10.1422769855; __utmc=261309969;
__utmz=261309969.1409853093.1.1.utmcsr=(direct)|utmccn=(direct)|utmcmd=(none);
__utmv=261309969.|14=MYM=1638924=1^16=UV=5423887=1^18=Sub=1795089=1^19=PCAT=5367B8=1;
__atuvc=1%7C5; __atuvs=54cdc5eabb3480fd000; __utmli=ctl00_ContentMain_btnBuy2'
-H 'Origin: http://uk.mouser.com' -H 'Accept-Encoding: gzip, deflate' -H
'Accept-Language: en-GB,en-US;q=0.8,en;q=0.6' -H 'User-Agent: Mozilla/5.0 (X11;
Linux i686) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/39.0.2171.65
Chrome/39.0.2171.65 Safari/537.36' -H 'Content-Type:
application/x-www-form-urlencoded' -H 'Accept:
text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8' -H
'Cache-Control: max-age=0' -H 'Referer:
http://uk.mouser.com/ProductDetail/Cree-Inc/CGHV96100F2/?qs=sGAEpiMZZMvplms98TlKY6zbNRoARcUg8gg333Al67kStE%252bN8N0%2fKg%3d%3d'
-H 'Connection: keep-alive' --data
'__EVENTTARGET=&__EVENTARGUMENT=&__VIEWSTATE=skTHKc%2BTu8q1ptksBWazoqW1jH%2F9s
30wKeqLaG6vPBO92Ae4BJFGniiNMJOdrxMC0BKNq0OgMPn9jzXyEnh%2BhZElrKrDDEwTj6wDz%2BB
5Mc8596z13lM4bwTtSkhsckjY87ZWffCEhuwhyb5YCmSMivmI453lwnERDa8eObcoNnPPaM0TNaN0o
X6eY%2FQ0eiyT%2FJsDR6vWe4u1sV0sPkLebGRRWfI4chXx3bL9X0CXPlXzEjYBjSMVFvahuPicHdx
N4QG31f8teVRA4a6JqwXeveNQi8J4yp2Euq3lgQnEjPAWpjeUEq5tXJbII8qczxQBrYBFu7ebLbyl
PNsPfrOeY6REXhUiEV1...
```
---

<img class=fullscreen src=images/unit_test.png />

---

<img class=fullscreen src=images/extension.png />

---

# 1-click BOM extension

- Available for Chrome and Firefox
- Takes in tab separated values
- Can load a on-line BOM 
- Able to add/remove to cart 
- Can have a guess at what part you mean
- Open source (CPAL)
- About 500 users

---
<img class=fullscreen src=images/meat3.jpg />

---
#Kitnic.it
- Git repository
- Tab separated values
  - 1-click-bom.tsv
  - At minumum: References, Quantity and Part Number
- RS274-X Gerbers and Excellon drills

```
.
├── 1-click-bom.tsv
└── gerbers
    ├── board.cmp
    ├── board.drd
    ├── board.dri
    ├── board.gko
    ├── board.gpi
    ├── board.gto
    ├── board.stc
    └── board.sts
```

---

<br>
<br>
<br>
<br>
<br>
<br>
<center><h1><a href=https://kitnic.it>kitnic.it</a><h1></center>

---
# The Virtual Kit
<img src=images/kit.jpg />

---

# Planned Features

- Accounts
- File upload and user project management
- Tagged releases and versioning
- Connect to PCB batching services
- Assembly aide
---
<img class=fullscreen src=images/aide.png />
- GitHub Pages & Travis CI
  - The boards.txt file

---

# More Planned Features
- Connect to assembly services
- Better tools for making BOMs
- Live pricing data

---
<br/>
<br/>
<center><img class=fullscreen src=images/bicyle_incremental.jpg /></center>
---
<img style="left:0;" height=150px src=images/travis_pipeline.png />
- Static site hosting on Netlify and AWS
- Travis CI builds every branch
- All branches are deployed to `*.preview.kitnic.it` sub-domains
- Master branch is deployed to `kitnic.it`
- Register by editing the boards.txt file

```
https://github.com/kasbah/push-on-hold-off
https://github.com/kitnic/BQ25570_Harvester
https://github.com/JarrettR/USBvil
https://github.com/8BitMixtape/NextLevelEdition
https://github.com/dvdfreitag/Signal-Detector

```

---
<br/>
<br/>
<br/>
<br/>
<br/>
 <center><h1>Show me the code!<h1><center>
---
<br/>
<br/>
<center><img src=images/javascript_everywhere.jpg /></center>
---

##1-click BOM
- No more Coffeescript
- But we still compile from ES6 to ES5!

##Kitnic 
- React front-end
- Services using node.js and Express
  - e.g a service to clone git repos and serve the files
  - [github.com/kasbah/git-clone-server](https://github.com/kasbah/git-clone-server)

---
<svg width=400px viewBox="0 0 18 7">
  	<path fill="#CB3837" d="M0,0v6h5v1h4v-1h9v-6"></path>
  	<path fill="#FFF" d="M1,1v4h2v-3h1v3h1v-4h1v5h2v-4h1v2h-1v1h2v-4h1v4h2v-3h1v3h1v-3h1v3h1v-4"></path>
</svg>

Over 350,000 javascript packages

e.g. left-pad:

```js
module.exports = leftpad;
function leftpad (str, len, ch) {
  str = String(str);
  var i = -1;
  if (!ch && ch !== 0) ch = ' ';
  len = len - str.length;
  while (++i < len) {
    str = ch + str;
  }
  return str;
}
```
---
# [tracespace/pcb-stackup](https://github.com/tracespace/pcb-stackup)

<p align=middle><img width=80% src=images/stackup.svg></p>
---
## Let's build an equality function for resistor descriptions!
<img style="max-width:300px;float:right;" src=images/resistors.jpg />
E.g.
  - 100 Ohm
  - 100R
  - 1k5
  - 1M Ω

---

```sh
npm install js-quantities resistor-data
```

```js
const Qty          = require('js-quantities')
const resistorData = require('resistor-data')

function extract(R) {
    //"1 Ohm" style
    const match1 = /\d+\.?\d* ?(ohm|Ω|Ω)/i.exec(R)
    if (match1) {
        return Qty(match1[0])
    }
    //"1k5" style
    const match2 = /\d+(k|m)\d+/i.exec(R)
    if (match2) {
        const v = resistorData.notationToValue(match2[0]) + ' ohm'
        return Qty(v)
    }
}

function equal(R1, R2) {
    return extract(R1) === extract(R2)
}

```
[Common Parts Library - CC-By Octopart in YAML format](https://github.com/octopart/cpl-data)
---

<video controls=true class=fullscreen src=images/demo.mp4 />

---



# How to get involved?
- Add your project and you'll get free PCB manufacturing (8/20 left)
- Web development
- Spread the word
<br />
<br />
<img style="float:right" width=200 src=images/divide.gif />

</font>
---
#Questions?
- [kitnic.it](https://kitnic.it)
- [@kitnic_it](https://twitter.com/kitnic_it)
- [github.com/monostable/kitnic](https://github.com/monostable/kitnic)
<font size=3>
<br />
<br />
<br />
<br />

Image credits

<li>ohwr.org logo - CC-BY-SA 4.0, CERN, 2014
<li>Cover of Troubleshooting Analog Circuits by Robert A. Pease - © 1991 by Butterworth-Heinemann
<li>Meat grinder & Disassembled hand-powered grinder - CC-BY-SA 3.0 - Wikipedia - Photos taken by de:user:Kku. Modified by de:user:Rainer Zenz</li>
<li>Bleep Drum Kit with MIDI - CC-BY-SA 2.0 - SparkFun Electronics</li>
<li>3 Resistors - CC-BY-SA https://commons.wikimedia.org/wiki/User:Afrank99 
<li> GFP-tagged Cln2 - CC-BY - Jean Peccoud - https://www.youtube.com/watch?v=sG2Zd3vRdvQ
