wchar.h
=======

**Overview**\ 
--------------

**Related Modules:**

`UTILS <utils.md>`__

**Description:**

Declares commonly used functions related to wide characters.

You can use functions provided in this file to perform operations such
as reading, writing, comparing, concatenating, copying, and searching
wide characters.

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

   <tr id="row1970225323084834">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1">

.. raw:: html

   <p id="p617083537084834">

Function Name

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2">

.. raw:: html

   <p id="p922726369084834">

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

   <tr id="row167638882084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1393971376084834">

wcscpy (wchar_t *dest, const wchar_t*\ src)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1935171726084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1391496898084834">

Copies the wide characters pointed to by src to the wide character array
pointed to by dest, including the terminating null character ‘\\0’. .

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1299309393084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p196617395084834">

wcsncpy (wchar_t *dest, const wchar_t*\ src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p136819028084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p692848306084834">

Copies the first n wide characters pointed to by src to the wide
character array pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row818989592084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1639997542084834">

wcscat (wchar_t *dest, const wchar_t*\ src)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1522806891084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p863909130084834">

Appends a copy of the wide characters pointed to by src to the end of
the wide character array pointed to by dest and adds a terminating null
character ‘\\0’.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row439055162084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2131119126084834">

wcsncat (wchar_t *dest, const wchar_t*\ src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1786112921084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p523884705084834">

Appends a copy of the first n wide characters pointed to by src to the
end of the wide characters pointed to by dest and adds a terminating
null character ‘\\0’.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1193136098084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1702346872084834">

wcscmp (const wchar_t *s1, const wchar_t*\ s2)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p980644348084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p265049712084834">

Compares each character in the string pointed to by s1 with that in the
string pointed to by s2 in ASCII-code order.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1747559067084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p721537511084834">

wcsncmp (const wchar_t *s1, const wchar_t*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1899537806084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1515057158084834">

Compares the first n characters in the string pointed to by s1 with
those in the string pointed to by s2 in ASCII-code order.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1063273339084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p327014331084834">

wcscoll (const wchar_t *ws1, const wchar_t*\ ws2)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1016890811084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p403685315084834">

Compares the wide characters in the string pointed to by ws1 with those
in the string pointed to by ws2 based on the specified locale
LC_COLLATE.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row952081792084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1752994385084834">

wcsxfrm (wchar_t *s1, const wchar_t*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p367545042084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1482320556084834">

Compares the first n wide characters in the string pointed to by s1 with
those in the string pointed to by s2.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1337887026084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1271954259084834">

wcschr (const wchar_t \*wcs, wchar_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1606239833084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p81481095084834">

Locates the first occurrence of the wide character pointed to by wc in
the wide character string pointed to by wcs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row120546154084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1867403508084834">

wcsrchr (const wchar_t \*wcs, wchar_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p734546575084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p536730820084834">

Locates the last occurrence of the wide character pointed to by wc in
the wide character string pointed to by wcs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row572538716084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1489223472084834">

wcscspn (const wchar_t *wcs, const wchar_t*\ accept)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p650989281084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1615744462084834">

Scans the wide character string pointed to by wcs for any wide
characters specified in reject and obtains the number of unmatched
characters in wcs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row942821231084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p919204145084834">

wcsspn (const wchar_t *wcs, const wchar_t*\ accept)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2140966317084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1993665549084834">

Scans the wide character string pointed to by wcs for any wide
characters specified in reject and obtains the number matched characters
in wcs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row653523509084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p281061487084834">

wcspbrk (const wchar_t *wcs, const wchar_t*\ accept)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1349076550084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1640216198084834">

Scans the wide character string pointed to by wcs for any wide
characters specified in accept and obtains the first occurrence of the
matched character.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row783253843084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p270137968084834">

wcstok (wchar_t *wcs, const wchar_t*\ delim, wchar_t \**ptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1707703817084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1914675577084834">

Splits a wide character string pointed to by wcs into tokens using the
given delimiter.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1218477583084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p662015837084834">

wcslen (const wchar_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1721908433084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p2064043634084834">

Calculates the length of a wide character string pointed to by s.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row918512661084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1623899841084834">

wcswcs (const wchar_t *haystack, const wchar_t*\ needle)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p980936544084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1340847275084834">

Searches the wide character string pointed to by dest for the first
occurrence of the wide character string pointed to by src.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1890990468084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1941982230084834">

wmemchr (const wchar_t \*s, wchar_t c, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1402560394084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1895487872084834">

Searches for the first position of the matched wide character within the
specified number of characters in a wide character string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1099780064084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1662242062084834">

wmemcmp (const wchar_t *lhs, const wchar_t*\ rhs, size_t count)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p265277583084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p301435275084834">

Compares the first count characters in the string pointed to by lhs with
the first count characters in the string pointed to by rhs.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row54753138084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p190187853084834">

wmemcpy (wchar_t *dest, const wchar_t*\ src, size_t count)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1355997663084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1874131295084834">

Copies count successive characters from the wide character array pointed
to by src to the wide character array pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1757320961084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1834370212084834">

wmemmove (wchar_t *dest, const wchar_t*\ src, size_t count)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p994710321084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p211233023084834">

Copies count successive characters from the wide character array pointed
to by src to the wide character array pointed to by dest (with possible
array overlapping).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2147411263084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1753379252084834">

wmemset (wchar_t \*dest, wchar_t ch, size_t count)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1544860459084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p150307219084834">

Fills count characters specified by ch to the wide character array
pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row701174646084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1144527222084834">

btowc (int c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1069514173084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1081453469084834">

Converts a single-byte character c into its wide-character
representation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1539090636084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1643585164084834">

wctob (wint_t c)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p740036474084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1096476566084834">

Converts a wide character c into its single-byte representation.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row44606727084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1396227919084834">

mbsinit (const mbstate_t \*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1490892437084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p78753967084834">

Checks whether the mbstate_t object pointed to by ps is in the initial
state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1175262659084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1040252195084834">

wcrtomb (char *s, wchar_t wc, mbstate_t*\ ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p167750538084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p439472974084834">

Converts the wide character specified by wc into a character string and
stores the string to the beginning of the character array pointed to by
s.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1095130153084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p9809842084834">

mbrlen (const char *s, size_t n, mbstate_t*\ ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1390768482084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1759519578084834">

Determines the number of bytes in a character string pointed to by s.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1681495587084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1847070383084834">

mbsrtowcs (wchar_t \*dest, const char \**src, size_t len, mbstate_t
\*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1480474581084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1893004506084834">

Converts a multi-byte character string with a length of len into a wide
character string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1311521552084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p75055554084834">

wcsrtombs (char \*dest, const wchar_t \**src, size_t len, mbstate_t
\*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p616229612084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p360698395084834">

Converts a wide character string into a multi-byte string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1963244607084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1313260087084834">

wcstof (const wchar_t \*str, wchar_t \**endptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p475862926084834">

float

.. raw:: html

   </p>

.. raw:: html

   <p id="p2088193383084834">

Converts a wide character string pointed to by str into a floating-point
value and assigns the next character in str after the floating-point
value to endptr.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row306519621084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1119363705084834">

wcstod (const wchar_t \*str, wchar_t \**endptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p135603164084834">

double

.. raw:: html

   </p>

.. raw:: html

   <p id="p778543396084834">

Converts a wide character string pointed to by str into a double value
and assigns the next character in str after the double value to endptr.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row284176323084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1782442108084834">

wcstold (const wchar_t \*str, wchar_t \**endptr)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p311281995084834">

long double

.. raw:: html

   </p>

.. raw:: html

   <p id="p1789674390084834">

Converts a wide character string pointed to by str into a long double
value and assigns the next character in str after the long double value
to endptr.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1516884025084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1001694827084834">

wcstol (const wchar_t \*str, wchar_t \**endptr, int base)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1601741131084834">

long

.. raw:: html

   </p>

.. raw:: html

   <p id="p849910344084834">

Converts a wide character string pointed to by str into a long value.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row857185679084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2044061999084834">

wcstoul (const wchar_t \*str, wchar_t \**endptr, int base)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p299712757084834">

unsigned long

.. raw:: html

   </p>

.. raw:: html

   <p id="p269451959084834">

Converts a wide character string pointed to by str into an unsigned long
value of a specified base.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2013335549084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1469596614084834">

wcstoll (const wchar_t \*str, wchar_t \**endptr, int base)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1103882092084834">

long long

.. raw:: html

   </p>

.. raw:: html

   <p id="p742828242084834">

Converts a wide character string pointed to by str into a long long
value of a specified base.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1289362298084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2137536280084834">

wcstoull (const wchar_t \*str, wchar_t \**endptr, int base)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1593970826084834">

unsigned long long

.. raw:: html

   </p>

.. raw:: html

   <p id="p359005930084834">

Converts a wide character string pointed to by str into an unsigned long
long value of a specified base.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row992280149084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1098752580084834">

fwide (FILE \*stream, int mode)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p748002868084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1079101225084834">

Sets and determines the orientation of the file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row552513067084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1101038167084834">

wprintf (const wchar_t \*format,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1274798115084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p633076324084834">

Prints formatted data to the standard output (stdout).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1907600750084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1785592434084834">

fwprintf (FILE \*__restrict fp, const wchar_t \*__restrict fmt,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1988075618084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p400937249084834">

Prints wide character strings to a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1522653703084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1958031611084834">

swprintf (wchar_t *wcs, size_t maxlen, const wchar_t*\ format,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1870943283084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1101904523084834">

Prints formatted data to a specified string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1084960799084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2079718576084834">

vwprintf (const wchar_t \*format, va_list args)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p577538311084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p484433250084834">

Prints formatted data from a variable argument list to the standard
output (stdout).

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1314163013084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1698480288084834">

vfwprintf (FILE *stream, const wchar_t*\ format, \__isoc_va_list args)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2034097334084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p809154784084834">

Prints formatted data from a variable argument list specified by args to
a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1420179472084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1584347177084834">

vswprintf (wchar_t *wcs, size_t maxlen, const wchar_t*\ format,
\__isoc_va_list args)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1424545387084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1302898109084834">

Prints formatted data from a variable argument list specified by args to
a specified string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row372196632084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p888848622084834">

wscanf (const wchar_t \*format,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1175393816084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p94469205084834">

Reads formatted data from the standard input (stdin) and stores it based
on the wide string format into the locations pointed to by the variable
arguments.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row440830629084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p256787217084834">

fwscanf (FILE *stream, const wchar_t*\ format,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p983669620084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1893379505084834">

Reads formatted data from a specified stream and stores it based on the
wide string format into the locations pointed to by the variable
arguments.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1695322403084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1880990654084834">

swscanf (const wchar_t *ws, const wchar_t*\ format,…)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1983878883084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p599191152084834">

Reads data from a wide character string pointed to by ws and stores it
based on the wide string format into the locations pointed to by the
variable arguments.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1115932274084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1712039360084834">

vwscanf (const wchar_t \*format, va_list arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1484128307084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p932710823084834">

Reads data from the stdin and stores it based on the wide string format
into the locations pointed to by the elements in the variable argument
list identified by arg.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1085440638084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1413750229084834">

vfwscanf (FILE *stream, const wchar_t*\ format, va_list arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1638168517084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p732422936084834">

Reads data from a specified file stream and stores it based on the wide
string format into the locations pointed to by the elements in the
variable argument list identified by arg.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1248559136084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1684115351084834">

vswscanf (const wchar_t *ws, const wchar_t*\ format, va_list arg)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1391669361084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p538682495084834">

Reads data from a string pointed to by ws and stores it based on the
wide string format into the locations pointed to by the elements in the
variable argument list identified by arg.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1739946327084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1659816230084834">

fgetwc (FILE \*stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1624176469084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p30966041084834">

Reads a wide character from a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row156634705084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1715658925084834">

getwc (FILE \*stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p311035726084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p148312436084834">

Reads the first wide character from a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1668862563084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2012167869084834">

getwchar (void)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p166130898084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1720248341084834">

Reads a wide character from the stdin.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row914983542084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p613302456084834">

fputwc (wchar_t wc, FILE \*stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1165329179084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1520720578084834">

Writes a wide character wc to a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1162461101084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1472139846084834">

putwc (wchar_t wc, FILE \*stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p47399125084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1529326529084834">

Writes a wide character wc to a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2117355403084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1492359717084834">

putwchar (wchar_t wc)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1542261011084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p154119086084834">

Writes a wide character wc to the stdout.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1230254125084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1379318232084834">

fgetws (wchar_t *ws, int n, FILE*\ stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p605864746084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1815045362084834">

Reads wide characters from a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1203808267084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p876053562084834">

fputws (const wchar_t *ws, FILE*\ stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p164334091084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p96917575084834">

Writes a wide string pointed to by ws to a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row118682033084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1912223739084834">

ungetwc (wint_t ch, FILE \*stream)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1505340426084834">

wint_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p772000585084834">

Pushes a character back into a specified file stream.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1291593909084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1994841038084834">

mbrtowc (wchar_t *pwc, const char*\ s, size_t n, mbstate_t \*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2094627129084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1030486889084834">

Converts a multi-byte character string with a length of n into a wide
character string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row963164442084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p2057465348084834">

mbsnrtowcs (wchar_t \*dest, const char \**src, size_t nwc, size_t len,
mbstate_t \*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2004239525084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p856625795084834">

Converts a multi-byte character string with a length of n into a wide
character string that can hold a total of nwc wide characters.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1677927843084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1445951319084834">

wcsnrtombs (char \*dest, const wchar_t \**src, size_t nwc, size_t len,
mbstate_t \*ps)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1566712237084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p128608007084834">

Converts nwc wide characters in the string pointed to by src into a
character string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1465685408084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p94537508084834">

wcsdup (const wchar_t \*s)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p678376994084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p828980934084834">

Copies a specified wide character string to a newly allocated buffer.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1500764059084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p818317922084834">

wcsnlen (const wchar_t \*s, size_t maxlen)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p987747401084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1483050357084834">

Calculates the length of a wide character string pointed to by s.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row240529430084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p208658740084834">

wcpcpy (wchar_t *dest, const wchar_t*\ src)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1311988987084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p979447884084834">

Copies the wide characters (including the terminating null character
‘\\0’) pointed to by src to the wide character array pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1640419816084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p646998882084834">

wcpncpy (wchar_t *dest, const wchar_t*\ src, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1722219990084834">

wchar_t \*

.. raw:: html

   </p>

.. raw:: html

   <p id="p1229339689084834">

Copies n wide characters (including the terminating null character
‘\\0’) pointed to by src to the wide character array pointed to by dest.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2137378921084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1778690127084834">

wcscasecmp (const wchar_t *s1, const wchar_t*\ s2)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1540802193084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1856057821084834">

Compares the wide characters in the string pointed to by s1 with those
in the string pointed to by s2, with their case differences ignored.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1019124845084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1757855308084834">

wcscasecmp_l (const wchar_t *s1, const wchar_t*\ s2, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1562160699084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p238984724084834">

Compares the wide characters in the string pointed to by s1 with those
in the string pointed to by s2 based on the specified locale
environment, with their case differences ignored.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row296075646084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p531853184084834">

wcsncasecmp (const wchar_t *s1, const wchar_t*\ s2, size_t n)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1834490778084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1874717670084834">

Compares a maximum of n wide characters in the string pointed to by s1
with those in the string pointed to by s2, with their case differences
ignored.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row544289111084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p604668733084834">

wcsncasecmp_l (const wchar_t *s1, const wchar_t*\ s2, size_t n, locale_t
locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1773196915084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1076431737084834">

Compares a maximum of n wide characters in the string pointed to by s1
with those in the string pointed to by s2 based on the specified locale
environment, with their case differences ignored.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row214481559084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1896442894084834">

wcscoll_l (const wchar_t *s1, const wchar_t*\ s2, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p1513619486084834">

int

.. raw:: html

   </p>

.. raw:: html

   <p id="p1607315292084834">

Compares wide characters in the string pointed to by s1 with those in
the string pointed to by s2 based on the specified locale environment.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1508745774084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p1217723987084834">

wcsftime (wchar_t \*__restrict wcs, size_t n, const wchar_t \*__restrict
f, const struct tm \*__restrict tm)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2063873487084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p1612925509084834">

Converts the date and time in the tm structure to a wide character
string.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1899844758084834">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 ">

.. raw:: html

   <p id="p206263866084834">

wcsxfrm_l (wchar_t *s1, const wchar_t*\ s2, size_t n, locale_t locale)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 ">

.. raw:: html

   <p id="p2129932035084834">

size_t

.. raw:: html

   </p>

.. raw:: html

   <p id="p834997624084834">

Compares the first n wide characters in the string pointed to by s1 with
those in the string pointed to by s2 based on the specified locale
environment.

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
