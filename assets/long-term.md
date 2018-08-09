

# Maybe later 


## Document doesn't use legible font sizes
Document doesn&#39;t use legible font sizes

Description:<br>
Font sizes less than 12px are too small to be legible and require mobile visitors to “pinch to zoom” in order to read. Strive to have &gt;60% of page text ≥12px. [Learn more](https://developers.google.com/web/tools/lighthouse/audits/font-sizes).

<br>

<hr> 

<br>


## `<html>` element does not have a `[lang]` attribute

If a page doesn&#39;t specify a lang attribute, a screen reader assumes that the page is in the default language that the user chose when setting up the screen reader. If the page isn&#39;t actually in the default language, then the screen reader might not announce the page&#39;s text correctly. [Learn more](https://dequeuniversity.com/rules/axe/2.2/html-lang?application=lighthouse).



### Add `lang` attribute.

__HTML location:__

```html
<html xmlns="http://www.w3.org/1999/xhtml" class="">
```

#### Suggested solution:
Add a `lang` attribute. For websites in english use `<html lang="en">`. [Other languages references](https://www.w3schools.com/tags/ref_language_codes.asp)

<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML</code>

Path:<br>
`html`

More detailed explanation:<br>
Fix any of the following:
<br>The &lt;html&gt; element does not have a lang attribute
</details>

<hr>

<br>




## `[id]` attributes on the page are not unique

The value of an id attribute must be unique to prevent other instances from being overlooked by assistive technologies. [Learn more](https://dequeuniversity.com/rules/axe/2.2/duplicate-id?application=lighthouse).



### 
  Document has multiple elements with the same id attribute: closeFacet

__Visual location:__

![ Subject element with duplicate ID](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a class="facetName" id="closeFacet" facetname="Subject" href="?Ntk=Keyword&amp;Nr=OR%28210969%2cOR%28206474%29%29&amp;Ne=200043+206474+210899+210956&amp;N=0&amp;Ntt=cats#2">
<img src="images/DUKE_downarrow.gif">
&nbsp;<strong>Subject</strong></a>
```

####Suggested solution:

1. Check if the page needs that ID for CSS for visual reasons.
2. Check if the page needs that ID for JS for interactive behaviors.
3. If it needs the IDs edit the dependent code, then remove duplicate IDs from the HTML.

<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,0,TD,0,DIV,3,TABLE,0,TBODY,1,TR,0,TD,1,A</code>

Path:<br>
<code>a[facetname="Subject"]</code>
</details>

<hr>

<br>


### 
  Document has multiple elements with the same id attribute: openFacet

__Visual location:__

![ Medical Subject element with duplicate ID](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a class="facetName" id="openFacet" facetname="Medical Subject" href="?Ntk=Keyword&amp;Nr=OR%28210969%2cOR%28206474%29%29&amp;Ne=2+200043+206474+210899+210956+206473&amp;N=0&amp;Ntt=cats#206473">
<img src="images/DUKE_rightarrow.gif">
&nbsp;<strong>Medical Subject</strong></a>
```

####Suggested solution:

1. Check if the page needs that ID for CSS for visual reasons.
2. Check if the page needs that ID for JS for interactive behaviors.
3. If it needs the IDs edit the dependent code, then remove duplicate IDs from the HTML.

<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,0,TD,0,DIV,3,TABLE,0,TBODY,2,TR,0,TD,1,A</code>

Path:<br>
<code>a[facetname="Medical\ Subject"]</code>
</details>

<hr>

<br>


### 
  Document has multiple elements with the same id attribute: getit@Duke

__Visual location:__

![ element with duplicate ID](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a href="http://proxy.lib.duke.edu/login?url=https://duke.kanopy.com/node/2874859" target="_blank" id="getit@Duke" tracking="DUKE008360616" title="get it@Duke"><img src="//library.duke.edu/imgs/SerSols/GetItAtDuke.gif" alt="get it@Duke"></a>
```

####Suggested solution:

1. Check if the page needs that ID for CSS for visual reasons.
2. Check if the page needs that ID for JS for interactive behaviors.
3. If it needs the IDs edit the dependent code, then remove duplicate IDs from the HTML.

<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,3,TR,2,TD,0,DIV,0,A</code>

Path:<br>
<code>a[tracking="DUKE008360616"]</code>
</details>

<hr>

<br>


### 
  Document has multiple elements with the same id attribute: googlePartialPreview

__Visual location:__

![Limited preview - Google Books element with duplicate ID](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a id="googlePartialPreview" href="https://books.google.com/books?id=f1InDwAAQBAJ&amp;printsec=frontcover&amp;source=gbs_ViewAPI" target="_blank">Limited preview - Google Books</a>
```

####Suggested solution:

1. Check if the page needs that ID for CSS for visual reasons.
2. Check if the page needs that ID for JS for interactive behaviors.
3. If it needs the IDs edit the dependent code, then remove duplicate IDs from the HTML.

<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,5,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,5,TR,1,TD,0,A</code>

Path:<br>
<code>.itemRecord:nth-child(6) > tbody > tr:nth-child(1) > td[valign="top"][align="left"] > .table.table-condensed.itemRecordDetails > tbody > .gbsContainer > .brieflibrary[width="\36 5\%"][colspan="\33 "] > a[target="_blank"]</code>
</details>

<hr>

<br>









## Background and foreground colors do not have a sufficient contrast ratio.

Low-contrast text is difficult or impossible for many users to read. [Learn more](https://dequeuniversity.com/rules/axe/2.2/color-contrast?application=lighthouse).

<br>


### The element _"On Order."_ has low contrast.

__Visual location:__


![On Order. text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<span class="resultAvailabilityCheckedOut">On Order.</span>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,8,TR,4,TD,0,SPAN</code>

Path:<br>
<code>td[itembarcode="D05222956V"] > .resultAvailabilityCheckedOut</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<br> 

<hr>

<br>

### The element _"Checked Out (Due 08/14/18)."_ has low contrast.

__Visual location:__


![Checked Out (Due 08/14/18). text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<span class="resultAvailabilityCheckedOut">Checked Out (Due 08/14/18).</span>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,3,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,7,TR,4,TD,0,SPAN</code>

Path:<br>
<code>td[itembarcode="F00097248U"] > .resultAvailabilityCheckedOut</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<br>

<hr>

<br>


### The element _"Checked Out (Due 05/31/19)."_ has low contrast.

__Visual location:__


![Checked Out (Due 05/31/19). text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<span class="resultAvailabilityCheckedOut">Checked Out (Due 05/31/19).</span>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,4,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,7,TR,4,TD,0,SPAN</code>

Path:<br>
<code>td[itembarcode="D05184456X"] > .resultAvailabilityCheckedOut</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<br>

<hr>

<br>








### The element _"Checked Out (Due 11/26/18)."_ has low contrast.

__Visual location:__


![Checked Out (Due 11/26/18). text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<span class="resultAvailabilityCheckedOut">Checked Out (Due 11/26/18).</span>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,11,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,8,TR,4,TD,0,SPAN</code>

Path:<br>
<code>td[itembarcode="D05045967-"] > .resultAvailabilityCheckedOut</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.99 (foreground color: #ff0000, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>





### The element _"Format:"_ has low contrast.

__Visual location:__


![Format: text with low contrast](assets/low-contrast--textlablels.png)

__HTML location:__

```html
<td width="18%" class="lightText" valign="top">Format: </td>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,16,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,1,TD</code>

Path:<br>
<code>.itemRecord:nth-child(17) > tbody > tr:nth-child(1) > td[valign="top"][align="left"] > .table.table-condensed.itemRecordDetails > tbody > tr:nth-child(3) > .lightText[width="\31 8\%"][valign="top"]</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>






<br>


### The element _"Published:"_ has low contrast.

__Visual location:__


![Published: text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<td width="18%" class="lightText" valign="top">Published: </td>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,17,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,3,TR,1,TD</code>

Path:<br>
<code>.itemRecord:nth-child(18) > tbody > tr:nth-child(1) > td[valign="top"][align="left"] > .table.table-condensed.itemRecordDetails > tbody > tr:nth-child(4) > .lightText[width="\31 8\%"][valign="top"]</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>


### The element _"Author:"_ has low contrast.

__Visual location:__


![Author: text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<td width="18%" class="lightText" valign="top">Author:</td>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,18,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,1,TR,1,TD</code>

Path:<br>
<code>.itemRecord:nth-child(19) > tbody > tr:nth-child(1) > td[valign="top"][align="left"] > .table.table-condensed.itemRecordDetails > tbody > tr:nth-child(2) > .lightText[width="\31 8\%"][valign="top"]</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>


### The element _"Online Access:"_ has low contrast.

__Visual location:__


![Online Access: text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<td class="lightText" valign="top" width="18%">Online Access:</td>
```

#### Suggested solution:

  Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,4,TR,2,TD,0,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,2,TR,0,TD,1,TABLE,0,TBODY,0,TR,0,TD,8,TABLE,0,TBODY,0,TR,0,TD,0,TABLE,0,TBODY,4,TR,1,TD</code>

Path:<br>
<code>tr:nth-child(5) > .lightText[width="\31 8\%"][valign="top"]</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 3.94 (foreground color: #808080, background color: #ffffff, font size: 9.0pt, font weight: normal). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>





### The element _"Contact Us"_ has low contrast.

__Visual location:__


![Contact Us text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a href="//library.duke.edu/about/contact">Contact Us</a>
```

#### Suggested solution:

  Element has insufficient color contrast of 1.94 (foreground color: #a1b70d, background color: #eeeeee, font size: 9.0pt, font weight: bold). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,5,TR,0,TD,3,DIV,1,DIV,0,H3,0,A</code>

Path:<br>
<code>#region-footer-contact > h3 > a</code>

More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 1.94 (foreground color: #a1b70d, background color: #eeeeee, font size: 9.0pt, font weight: bold). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>


### The element _"Services for..."_ has low contrast.

__Visual location:__


![Services for... text with low contrast](https://via.placeholder.com/150x50)

__HTML location:__

```html
<a href="//library.duke.edu/services">Services for...</a>
```

#### Suggested solution:

  Element has insufficient color contrast of 1.94 (foreground color: #a1b70d, background color: #eeeeee, font size: 9.0pt, font weight: bold). Expected contrast ratio of 4.5:1



<details>
<summary>_Additional debugging details_</summary>
Selector:<br>
<code>1,HTML,1,BODY,1,TABLE,0,TBODY,5,TR,0,TD,3,DIV,2,DIV,0,H3,0,A</code>


More detailed explanation:<br>
Fix any of the following:
<br>Element has insufficient color contrast of 1.94 (foreground color: #a1b70d, background color: #eeeeee, font size: 9.0pt, font weight: bold). Expected contrast ratio of 4.5:1
</details>

<hr>

<br>






