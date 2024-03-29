<p id="header"><p>

<table><tr>
<td> <a href="https://github.com/emjose/js-notes-app/#header"><img src="https://res.cloudinary.com/dn1e07eul/image/upload/v1659330996/Readme%20Headers/header-left_ctkix5.png" alt="previous" style="width: 200px;"/></a> </td>
<td> <a href="https://github.com/emjose/one-hundred/#header"><img src="https://res.cloudinary.com/dn1e07eul/image/upload/v1659330606/Readme%20Headers/header-center_bkbdbt.png" alt="100 days of code" style="width: 580px;"/></a> </td>
<td> <a href="https://github.com/emjose/wordle-2/#header"><img src="https://res.cloudinary.com/dn1e07eul/image/upload/v1659330646/Readme%20Headers/header-right_eftaz9.png" alt="next" style="width: 200px;"/></a> </td>

</tr></table>

<br>

<p id="project-title"><p>

<a href=#table-of-contents>![Design Patterns 101](https://res.cloudinary.com/dn1e07eul/image/upload/v1659385856/Readme%20Headers/inter-033-design-patterns_qz9lji.png)</a>

<br>

<a href="https://design-patterns-101.vercel.app/">![Design Patterns 101](Assets/preview-033-design-patterns.png)</a>

#

<p id="table-of-contents"><p>

<a href=#table-of-contents>![Table of Contents](https://res.cloudinary.com/dn1e07eul/image/upload/v1659241355/Readme%20Headers/inter-toc_euxbbw.png)</a>

-   [100 Days of Code](#100days)
-   [Installation](#installation)
-   [Live Site](#live-site)
-   [Issues](#issues)
-   [Resources](#resources)
-   [Copyright](#copyright)
-   [Let's Connect!](#lets-connect)

<br>

#

<p id="100days"><p>

<a href=#100days>![#100DaysOfCode](https://res.cloudinary.com/dn1e07eul/image/upload/v1659389776/Readme%20Headers/inter-100hash_kjpgmt.png)</a>

### Day 33: February 1, 2022

-   To begin learning about design patterns, I made flip cards by adapting my <a href="https://github.com/emjose/agile-101/#header">Agile 101 project</a>.

-   Design patterns are general solutions to commonly occurring problems in software design.

-   Design patterns can be described as reusable and customizable blueprints or templates.

-   The flip cards feature the 23 design patterns first described in the book:

    <a href="http://www.javier8a.com/itc/bd1/articulo.pdf">**_Design Patterns: Elements of Reusable Object-Oriented Software_**</a> (1994)

    by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides (known as the the **Gang of Four**)

-   The material and art are from <a href="https://refactoring.guru/">Refactoring.Guru</a> and <a href="https://zhart.us/">Dmitry Zhart</a>. Images formatted with Adobe Photoshop.

-   **This app is best viewed on a desktop computer or a laptop, using a Chrome, Firefox, or Edge browser.**

<br>

#

<p id="installation"><p>

<a href=#installation>![Installation](https://res.cloudinary.com/dn1e07eul/image/upload/v1659389842/Readme%20Headers/inter-installation_j9ixlq.png)</a>

#### 1. Git clone and cd into the repo folder:

```console
git clone git@github.com:emjose/design-patterns-101.git && cd design-patterns-101
```

#### 2. Run the command:

```console
open index.html
```

<br>

#

<p id="live-site"><p>

<a href="https://design-patterns-101.vercel.app/">![Live Site](https://res.cloudinary.com/dn1e07eul/image/upload/v1659389947/Readme%20Headers/inter-live-site_ngkqcf.png)</a>

<a href="https://design-patterns-101.vercel.app/">![Live Site](Assets/033-design-patterns.gif)</a>

<br>

• **[Design Patterns 101](https://design-patterns-101.vercel.app/)** is keyboard accessible, and a mouse hover will flip a card over.

• **[Design Patterns 101](https://design-patterns-101.vercel.app/)** is a [progressive web app](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps).

• Pressing the tab key (or a mouse click) will **pause** a selected card in its flipped state.

• A tab key press or a mouse click **outside** of the flipped card reverts that card to its original state.

• On a touchscreen device: tapping another card will flip the previously selected card back to its initial state.

<br>

#

<p id="issues"><p>

<a href=#issues>![Issues](https://res.cloudinary.com/dn1e07eul/image/upload/v1659392574/Readme%20Headers/inter-issues_mzq4o7.png)</a>

-   **This app is best viewed on a desktop computer or a laptop, using a Chrome, Firefox, or Edge browser.**

-   Like its sister project **[Agile 101](https://agile-101.vercel.app/)**, the **[Design Patterns 101](https://design-patterns-101.vercel.app/)** cards didn't flip correctly on a mobile phone.

-   The primary issue is that <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/:hover">the `:hover` pseudo class is problematic on touchscreens</a>.

-   Stack Overflow questions ( <a href="https://stackoverflow.com/questions/22559756/changing-hover-to-touch-click-for-mobile-devices">One</a> • <a href="https://stackoverflow.com/questions/19792575/css3-flip-functionality-problems-with-backface-visibility">Two</a> ) led to the solutions of adding **`:focus`** to CSS properties and **`tabindex="0"`** to HTML elements.

-   The <a href="https://developer.mozilla.org/en-US/docs/Glossary/Vendor_Prefix">vendor prefixes</a> (`-webkit-`, `-moz-`, `-ms-`, `-o-`) were also added to the transform and backface-visibility CSS properties.

-   **An issue with some touchscreen devices:** Tapping a card may yield a partial blue outline that doesn't correctly surround the card. However, cards will flip correctly when tapped.

-   **August 2022 update:** The partial blue outline issue was resolved by disabling the outline property and enabling the border property for the **`:focus`** state in a mobile media query.

<br>

<a href="https://design-patterns-101.vercel.app/">![Live Site](Assets/inter-issue-example.png)</a>

The partial blue outline that may appear on touchscreen or mobile devices.

<br>

#

<p id="resources"><p>

<a href=#resources>![Resources](https://res.cloudinary.com/dn1e07eul/image/upload/v1659314247/Readme%20Headers/inter-resources_ncevbw.png)</a>

-   #### [Creating a Card Flip by Dong Xia](https://dong-xia.medium.com/creating-a-card-flip-i-challenge-you-to-a-duel-4e4e124c5060)

-   #### [How TO - Flip Card](https://www.w3schools.com/howto/howto_css_flip_card.asp)

-   #### [Flaticon](https://www.flaticon.com/)

-   #### [Adobe Photoshop](https://www.adobe.com/products/photoshop/free-trial-download.html)

-   #### [Interpreter Design Pattern](https://sourcemaking.com/design_patterns/interpreter)

-   #### [JavaScript Design Patterns](https://www.dofactory.com/javascript/design-patterns)

-   #### [Design Patterns: Notes by Ray Toal](https://cs.lmu.edu/~ray/notes/designpatterns/)

-   #### [Design Patterns JS](https://github.com/fbeline/design-patterns-JS) by [Felipe Beline](https://github.com/fbeline)

-   #### [Gang of Four (GoF) Design Patterns](https://www.journaldev.com/31902/gangs-of-four-gof-design-patterns)

-   #### [Learning JavaScript Design Patterns](https://www.patterns.dev/posts/classic-design-patterns/)

-   #### [PDF - _Design Patterns: Elements of Reusable Object-Oriented Software_](http://www.javier8a.com/itc/bd1/articulo.pdf)

-   #### [My blog on how I created my Github READMEs](https://emmanueljose.medium.com/readme-a-makeover-story-b9c7be37a6de?sk=7ae6623d365409d875753e4604e42ffd)

<br>

#

<p id="copyright"><p>

<a href=#copyright>![Copyright](https://res.cloudinary.com/dn1e07eul/image/upload/v1659391383/Readme%20Headers/inter-copyright_ax53yz.png)</a>

-   This project is for made for educational purposes only.

-   Material copyright of © <a href="https://refactoring.guru/">Refactoring.Guru</a>. All Rights Reserved.

-   Art copyright of © <a href="https://zhart.us/">Dmitry Zhart</a>. All Rights Reserved.

<br>

#

<p id="lets-connect"><p>

<a href=#lets-connect>![Let's Connect!](https://res.cloudinary.com/dn1e07eul/image/upload/v1659314257/Readme%20Headers/inter-lets-connect_bv3kcd.png)</a>

<p><a href="https://twitter.com/Emmanuel_Labor"><img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" height=30 width=90 alt="Twitter badge"></a> <a href="https://www.linkedin.com/in/emmanuelpjose/"><img src="https://img.shields.io/badge/linkedin-%230064e7.svg?&style=for-the-badge&logo=linkedin&logoColor=white" height=30 width=90 alt="Linkedin badge"></a> <a href="https://emmanueljose.medium.com/"><img src="https://img.shields.io/badge/medium-%238700f5.svg?&style=for-the-badge&logo=medium&logoColor=white" height=30 width=90 alt="Medium badge"></a> <a href="https://www.instagram.com/emmanuel_jose/"><img src="https://img.shields.io/badge/instagram-%23ff0077.svg?&style=for-the-badge&logo=instagram&logoColor=white" height=30 width=90 alt="Instagram badge"></a> <a href="mailto:emjose@gmail.com"><img src="https://img.shields.io/badge/gmail-%23fd1745.svg?&style=for-the-badge&logo=gmail&logoColor=white" height=30 width=90 alt="Gmail badge"></a> <a href="https://www.emmanuel-jose.com/"><img src="https://img.shields.io/badge/portfolio-%23FF0000.svg?&style=for-the-badge&logoColor=white" height=30 width=90 alt="Portfolio badge"></a> <a href="https://github.com/emjose"><img src="https://img.shields.io/badge/github-%23ff8e44.svg?&style=for-the-badge&logo=github&logoColor=white" height=30 width=90 alt="Github badge"></a></p>

#

<a href=#header>![Back to Top](https://res.cloudinary.com/dn1e07eul/image/upload/v1659314281/Readme%20Headers/inter-congrats_m4p3ck.png)</a>
