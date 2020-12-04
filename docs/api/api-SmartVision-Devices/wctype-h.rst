wctype.h
========

**Overview**\ 
--------------

**Related Modules:**

`UTILS <utils.md>`__

**Description:**

Provides functions to detect, translate, and map wide characters.

Wide characters are classified into the following types: **alnum**,
**alpha**, **upper**, **lower**, **digit**, **xdigit**, **graph**,
**cntrl**, **punct**, and **space**. You can use these functions to
detect the type of wide characters and translate the type for the
current locale `LC_CTYPE <io.md#ga07c66689961056725d7f50231d740ba9>`__
or a specified locale. You can use these functions to convert the case
of wide characters, map the wide characters, and obtain the mapping
descriptor for conversion.

**Since:**

1.0

**Version:**

1.0

**Summary**\ 
-------------

Functions
---------

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1748385002084834">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p1516023713084834">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p1722859213084834">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   </tr>

.. raw:: html

   </thead>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row1165020260084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p242422474084834">

iswalnum (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1093515948084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p815648615084834">

Checks whether a wide character is a letter or digit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1071126679084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1797116376084834">

iswalpha (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1555581518084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p170337063084834">

Checks whether a wide character is a letter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row890911150084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p139035485084834">

iswblank (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1212008512084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1132429817084834">

Checks whether a wide character is a space or tab character
(:raw-latex:`\t)`.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1239210638084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1664647313084834">

iswcntrl (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p463255313084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1671969373084834">

Checks whether a wide character is a control character.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1546681052084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p906536531084834">

iswdigit (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1261636789084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1801361560084834">

Checks whether a wide character is a decimal digit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row62432113084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1882671652084834">

iswgraph (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p758504571084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1582820365084834">

Checks whether a wide character is visible.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2114086266084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1823892369084834">

iswlower (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p415044682084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p591615422084834">

Checks whether a wide character is a lowercase letter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1507482287084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p457107942084834">

iswprint (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2122035392084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p184363735084834">

Checks whether a wide character is printable.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row446795300084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p542137301084834">

iswpunct (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1818446575084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p290236467084834">

Checks whether a wide character is a punctuation mark.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1101639386084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p937711727084834">

iswupper (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p613456857084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1675621044084834">

Checks whether a wide character is an uppercase letter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1478913183084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1517333929084834">

iswxdigit (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1604865948084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1633291813084834">

Checks whether a wide character is a hexadecimal digit.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1443128938084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p79078001084834">

iswctype (wint_t wc, wctype_t desc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1524351497084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p426138864084834">

Checks whether the character specified by wc belongs to the desc class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row53241037084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1590243021084834">

towctrans (wint_t wc, wctrans_t desc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1751823728084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1620617510084834">

Translates the type of a wide character based on the conversion mapping
relationship.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row413383902084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p453524845084834">

towlower (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1285638174084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p506983339084834">

Converts an uppercase wide character to lowercase.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row306743046084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p297500223084834">

towupper (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1473983314084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p920501741084834">

Converts a lowercase wide character to uppercase.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row910888408084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p35598783084834">

wctrans (const char \*name)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1413902599084834">

wctrans_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p8570963084834">

Determines a mapping which can map a wide character to another wide
character.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row362990612084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1048439885084834">

wctype (const char \*name)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1003044524084834">

wctype_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1589773043084834">

Checks whether a wide character type exists in the LC_CTYPE locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row596508074084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p662304310084834">

iswalnum_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1950459052084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p117591614084834">

Checks whether a wide character is a letter or digit for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1221851836084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1979912602084834">

iswalpha_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p955692743084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p756730207084834">

Checks whether a wide character is alphabetic for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2000256450084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1927862967084834">

iswblank_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p854634175084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p591590761084834">

Checks whether a wide character is a blank or :raw-latex:`\t<`/strong>
character for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row836704471084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p856591055084834">

iswcntrl_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1690996578084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p819293941084834">

Checks whether a wide character is a control character for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1331263695084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p87410379084834">

iswdigit_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p646594757084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p782667173084834">

Checks whether a wide character is a decimal digit for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row801384327084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p832356097084834">

iswgraph_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1612729493084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2126810579084834">

Checks whether a wide character is visible for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row450044527084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p35199908084834">

iswlower_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1489232608084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p2006388677084834">

Checks whether a wide character is in lowercase for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1876756365084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1024283754084834">

iswprint_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p197612491084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1052747756084834">

Checks whether a wide character is printable for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row38909682084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1303935536084834">

iswpunct_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p714991925084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p702858478084834">

Checks whether wc is a punctuation wide character for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2029226177084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1010998690084834">

iswspace (wint_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p367740425084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1027734305084834">

Checks whether a wide character belongs to the wide-character class
space.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1171039547084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p950379629084834">

iswspace_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p188519295084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1491706114084834">

Checks whether a wide character belongs to the wide-character class
space for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row330741008084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1901592076084834">

iswupper_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1060006948084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p245622217084834">

Checks whether a wide character is in uppercase for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row264554648084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p476527472084834">

iswxdigit_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1445369964084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1559762981084834">

Checks whether a wide character is a hexadecimal digit for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1387478527084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p162645229084834">

iswctype_l (wint_t wc, wctype_t desc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1201196898084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p457220824084834">

Checks whether the character specified by wc belongs to the desc class
for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row826034651084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1114387122084834">

towlower_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p260633494084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p687401029084834">

Converts an uppercase wide character to lowercase for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1064054032084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p124236512084834">

towupper_l (wint_t wc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p149701396084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1279478838084834">

Converts a lowercase wide character to uppercase for the specified
locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1617378857084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p42559169084834">

towctrans_l (wint_t wc, wctype_t desc, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p315521554084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p744493548084834">

Translates the type of a wide character based on the translation mapping
relationship for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1357823071084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p270396993084834">

wctrans_l (const char \*name, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p241125124084834">

wctrans_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1577644352084834">

Determines a mapping which can map a wide character to another wide
character.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1983158290084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p451066142084834">

wctype_l (const char \*name, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p52199928084834">

wctype_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1569384530084834">

Checks whether a wide character type exists for the specified locale.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>
