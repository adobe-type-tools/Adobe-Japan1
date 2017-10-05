# The Adobe-Japan1-6 Character Collection
---
© 1992, 1993, 1998, 2000, 2002, 2004, 2008, 2017 Adobe Systems Incorporated.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file to use, copy, publish, distribute, sublicense, and/or sell copies of the documentation, and to permit others to do the same, provided that:

No modification, editing or other alteration of this document is allowed; and

The above copyright notice and this permission notice shall be included in all copies of the documentation.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file, to create their own derivative works from the content of this document to use, copy, publish, distribute, sublicense, and/or sell the derivative works, and to permit others to do the same, provided that the derived work is not represented as being a copy or version of this document.

Adobe shall not be liable to any party for any loss of revenue or profit or for indirect, incidental, special, consequential, or other similar damages, whether based on tort (including without limitation negligence or strict liability), contract or other legal or equitable grounds even if Adobe has been advised or had reason to know of the possibility of such damages. The Adobe materials are provided on an "AS IS" basis. Adobe specifically disclaims all express, statutory, or implied warranties relating to the Adobe materials, including but not limited to those concerning merchantability or fitness for a particular purpose or non-infringement of any third party rights regarding the Adobe materials.

Adobe holds no patents on the subject matter of this specification.

Last updated 2017-10-05

---
## Introduction
The purpose of this document is to define and describe the *Adobe-Japan1-6* character collection, which enumerates 23,058 glyphs, and whose designation is derived from the following three /CIDSystemInfo dictionary entries:

* /Registry (Adobe)
* /Ordering (Japan1)
* /Supplement 6

CIDFont resources that reference this character collection must include a /CIDSystemInfo dictionary that matches the /Registry and /Ordering strings shown above.

This document is designed for font developers, for the purpose of developing Japanese fonts for use with PostScript products, or for developing OpenType Japanese fonts. It is also useful for application developers and end users who need to know more about the glyphs in this character collection. This document expects that its readers are familiar with the CID-keyed font file format, which is described in [Adobe Technical Note #5014](https://www.adobe.com/devnet/font.html), entitled *Adobe CMap and CIDFont Files Specification*.

A character collection contains the glyphs that are required to develop font products for a specific language, script, or market. Specific encodings are defined through the use of CMap resources that are instantiated as files, and generally reference a subset of the character collection.

The character collection that results from each Supplement includes the glyphs associated with all earlier Supplements. For example, Supplement 6 includes all glyphs defined in Supplements 0 through 5.

The Adobe-Japan1-6 character collection enumerates 23,058 glyphs, specifically CIDs 0 through 23057, among seven Supplements, designated 0 through 6. Adobe-Japan1-6 completely supports the current JIS (*Japanese Industrial Standard*) character set standards, and earlier vintages thereof, specifically JIS X 0208:1997, JIS X 0213:2004, and JIS X 0212-1990. The following table summarizes these seven Supplements, and also provides the pages on which their glyphs are shown in the [*Adobe-Japan1-6.pdf*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/Adobe-Japan1-6.pdf) file:

**Supplement** | **Additional CIDs** | **CID Range** | **Total CIDs** | **Date of Establishment** | **Pages**
--- | --- | --- | --- | --- | ---
0 | *n/a* | 0–8283 | 8,284 | 1992 | 1–17
1 | 75 | 8284–8358 | 8,359 | 1993 | 17
2 | 361 | 8359–8719 | 8,720 | 1993 | 17–18
3 | 634 | 8720–9353 | 9,354 | 1998-09 | 18–19
4 | 6,090 | 9354–15443 | 15,444 | 2000-02-21 | 19–31
5 | 4,873 | 15444–20316 | 20,317 | 2002-09 | 31–41
6 | 2,741 | 20317–23057 | 23,058 | 2004-03-05 | 41–47

Each CID (*Character ID*) in a character collection is associated with a class of character shapes or glyphs. The specific shape of a glyph from a given glyph class is dependent on the typeface style and possibly other factors. Glyphs for all CIDs are illustrated in this document, providing a specific example or instance of the correspondence between a CID and its glyph shape class. Font developers should design glyphs for each CID of the character collection, and may use this document as a reference when proofing or otherwise validating CIDFont resources.

The following sections detail the history and contents of each of the seven Supplements of the Adobe-Japan1-6 character collection.

---
## Supplement 0—Adobe-Japan1-0

Supplement 0, which enumerates 8,284 glyphs, specifically CIDs 0 through 8283, was designed to be glyph-compatible with OCF (*Original Composite Format*) fonts, whose glyph set was published in Adobe Technical Note #5031, entitled *Kanji Glyph Collections and Glyph Sets* (included in this repository as the [*5031.JapaneseOCF.pdf*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/5031.JapaneseOCF.pdf) file). Supplement 0 thus includes the glyphs necessary to support the 1978 and 1983 vintages of the JIS X 0208 character set standard in terms of the number of glyphs, JIS X 0201-1997, and JIS83-based vendor character sets established by Apple (Macintosh KanjiTalk Version 6), Fujitsu, and NEC.

### Special Notes

In order to maintain stability and ensure predictability, CIDs 1125 through 7477 should be designed such that they are JIS90 compatible.

We further recommend that the glyphs for CIDs 243 and 245—along with their pre-rotated counterparts in Supplement 3, specifically CIDs 8962 and 8964—be designed in such a way that their glyphs are centered within their half-width (500-unit) set widths, thus making them look better when used between digits.

---
## Supplement 1—Adobe-Japan1-1

Supplement 1 provides 75 additional glyphs, specifically CIDs 8284 through 8358, that are necessary to support JIS X 0208-1990 (aka, JIS90), Apple’s Macintosh KanjiTalk Version 7.1 character set, and JIS90-based vendor character sets set forth by Fujitsu and NEC. Supplement 1 thus includes glyphs for the two so-called JIS90 kanji, specifically JIS X 0208-1990 凜 (84-05; U+51DC) and 熙 (84-06; U+7199). The 平成 (*heisei*) era-name kanji ligature is also among the glyphs that are included.

### Special Notes

In order to maintain stability and ensure predictability, CIDs 8284 and 8285 should be designed such that they are JIS90 compatible.

---
## Supplement 2—Adobe-Japan1-2

Supplement 2 adds 361 glyphs, specifically CIDs 8359 through 8719, that are used to support the Microsoft Windows Version 3.1J character set. IBM Select Kanji make up the vast majority—359 of the 361 glyphs—of the glyphs that were added for Supplement 2. Those who are familiar with IBM Select Kanji may know that it includes 360 kanji. The reason why Supplement 2 includes only 359 IBM Select Kanji is because one of them, 昂 (IBM 0xFAD0; JIS X 0208:1997 25-23; U+6602), was already included in Supplement 0, specifically at CID+1993.

---
## Supplement 3—Adobe-Japan1-3

Supplement 3 enumerates 634 glyphs, specifically CIDs 8720 through 9353, and was designed to add only pre-rotated versions of all non–full-width Latin and Latin-like glyphs found in Supplement 2 and earlier, for the specific purpose of supporting the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB (*Glyph SUBstitution*) feature.

### Special Notes

We recommend that the glyphs for CIDs 8962 and 8964—along with their unrotated counterparts in Supplement 0, specifically CIDs 243 and 245—be designed in such a way that their glyphs are centered within their half-width (500-unit) set widths, thus making them look better when used between digits.

---
## Supplement 4—Adobe-Japan1-4

Supplement 4 represents the very first “Pro” (short for *Professional*) character collection with its 6,090 additional glyphs, specifically CIDs 9354 through 15443, and is designed to satisfy most professional and commercial printing needs. By comparison, Supplement 3 is referred to as “Std” (short for *Standard*, meaning that their glyph repertoire is largely based on character set standards) character collection. “Pro” fonts thus effectively leap beyond standards, and provide glyphs that are necessary for professional and commercial printing.

### Special Notes

The glyphs for CIDs 12220 through 12227 are intended to be decorative in nature, and thus can vary from typeface to typeface, or from type foundry to type foundry. The representative glyphs for this range of eight CIDs merely illustrate the glyphs that are used for the *Kozuka Mincho* typeface design.

### Adobe-Japan1-4 Design Objectives

In order to satisfy the needs of professional and commercial printing in Japan, a wide variety of character and glyph sets were studied. These included common vendor extensions, proprietary glyph sets, common *gaiji* sets, and the JIS X 0212-1990 character set. Adobe-Japan1-4 was not intended to be a *Gaiji Solution*, but rather was designed to meet most of the professional and commercial printing needs in Japan. Put simply, Supplement 4 was specifically designed to allow sophisticated users to compose complex documents with a minimum use of so-called *gaiji* fonts.

### Adobe-Japan1-4 Technical Details

In order to ensure glyph consistency across fonts of different manufacturers, the JIS X 0208:1997 kanji—CIDs 1125 through 7477, 8284, and 8285 in Supplements 0 and 1—must be JIS90-compliant. This is due to the fact that some of the JIS X 0208:1997 kanji variants in Supplement 4 are sometimes subtle in their difference with their standard (JIS90) forms. The following is a summary of the glyph classes that are included in Adobe-Japan1-4:

* Additional proportional Latin glyphs, such as macroned vowels for transliterating Japanese text, along with genuine italic forms that correspond to the proportional Latin glyph set
* The “Euro” (U+20AC €)currency symbol, in full-width, proportional, and proportional italic forms
* “Horizontal in vertical” (縦中横 *tatechūyoko*) typesetting is enabled by third- and quarter-width forms
* Two styles of fractions­—nut-style with a horizontal bar, and traditional-style with diagonal line as the numerator/denominator separator—ranging from 0/3 to 1/100
* Nearly 2,000 additional annotated forms of the following character classes are included: numerals 0 through 100 (00 through 09 are also supported), upper and lowercase Latin alphabet, hiragana, katakana, and some kanji
* Annotation styles include parentheses, circles, black circles, boxes, black boxes, rounded boxes, and black rounded boxes
* Additional Latin ligatures, kana ligatures with vertical forms, and kanji ligatures with vertical forms
* Additional half- and full-width punctuation and symbols, along with the small hiragana and katakana “ko” in horizontal and vertical forms
* Horizontally- and vertically-optimized kana glyphs
* Ruby glyphs—applications are still expected to shrink the glyphs down to fifty percent size, but because the glyphs are expected to be designed at the reduced size, then scaled up, the results are typographically pleasing
* Pre-rotated forms of all proportional-, half-, third-, and quarter-width glyphs

Over 2,000 kanji and kanji variants are included, and are ordered and categorized as follows:

* Official traditional kanji forms as specified in the *Jōyō Kanji* (常用漢字) specification, dated 1981-10-01
* Additional JIS78 (aka, JIS C 6226-1978) kanji forms
* JIS83 (aka, JIS X 0208-1983) kanji forms
* Other JIS X 0208:1997 kanji variants
* IBM Select Kanji variants
* JIS X 0212-1990 kanji
* JIS X 0212-1990 kanji variants
* Unicode kanji
* K-JIS kanji
* *Dai Kanwa Jiten* (大漢和辞典) kanji

The above list of kanji and kanji variants can be misleading, because some glyphs categorized in an earlier glyph classes may be included in a later glyph classes. For example, all JIS X 0212-1990 kanji are in Unicode, and some JIS X 0212-1990 kanji are also K-JIS kanji. These 2,000 or so kanji and kanji variants include support for the following sets of kanji or kanji variants, some of which were partially supported in Supplement 2 and earlier:

* The remaining official traditional forms as specified in the *Jōyō Kanji* (常用漢字) specification, dated 1981-10-01
* Additional JIS78 (aka, JIS C 6226-1978) kanji forms
* JIS83 (aka, JIS X 0208-1983) kanji forms
* Common JIS X 0208:1997 kanji variants
* IBM Select Kanji variants
* JIS X 0221-1995 Ideographic Supplement 1­—918 kanji from JIS X 0212-1990
* All *Kōsei Hikkei* (校正必携) kanji variants
* All K-JIS kanji
* Other requests

---
## Supplement 5—Adobe-Japan1-5

Supplement 5 continues the expansion of the “Pro” character collection by adding 4,873 glyphs, specifically CIDs 15444 through 20316, and is designed to support the Apple Mac OS X Version 10.2 glyph set, which is also referred to as APGS (*Apple Publishing Glyph Set*). Supplement 5 is also designed to support the JIS X 0213:2000 character set and NLC (*National Language Council*) kanji (published on 2000-12-08).

### JIS X 0213:2000 Coverage

JIS X 0213:2000 includes 4,344 characters. Its 2004 revision, designated JIS X 0213:2004, added ten kanji, bringing its total to 4,354 characters. The glyphs for some JIS X 0213:2004 kanji are found in Supplement 4, but the vast majority are in Supplement 5. The following CIDs and CID ranges represent the Supplement 5 glyphs that correspond to JIS X 0213:2004 and variant forms thereof, vertical or otherwise:

15462, 15463, 15472–15479, 15486–15490, 15505–15516, 15600–15607, 15694–15722, 15725–15882, 15912–15975, 15983, 15984, 16068–16070, 16071–16075, 16162–16190, 16193–16282, 16299–16311, 16327, 16329–16349, 16352–16411, 16414–16447, 16450–16466, 16483–16490, 16497–16501, 16516–16685, 16715–19129, 19312, 19346, 20297–20316

Note that there are three JIS X 0213:2004 kanji in Supplement 6, specifically CIDs 21072 through 21074.

### NLC Glyph Coverage

Supplement 5 includes thirty-eight glyphs that effectively complete the coverage for NLC kanji, which is a set of 1,022 kanji established in 2000. Many NLC kanji are found in JIS X 0208:1997 as-is, or are in Supplement 4. The following is a complete list of the thirty-eight NLC kanji glyphs in Supplement 5, along with their related JIS X 0208:1997 forms in parentheses:

19312 (4570), 19346 (4738), 20175 (5741), 20222 (3505), 20263 (1666), 20264 (5020), 20265 (4036), 20266 (5976), 20267 (5704), 20268 (6662), 20269 (1402), 20270 (1662), 20271 (1243), 20272 (1791), 20273 (1850), 20274 (6481), 20275 (6258), 20276 (1892), 20277 (4368), 20278 (5629), 20279 (1998), 20280 (2171), 20281 (2085), 20282 (2523), 20283 (5707), 20284 (2059), 20285 (5937), 20286 (3086), 20287 (3251), 20288 (3379), 20289 (3538), 20290 (1494), 20291 (3628), 20292 (6325), 20293 (3822), 20294 (3832), 20295 (6537), 20296 (6510)

---
## Supplement 6—Adobe-Japan1-6

Supplement 6 adds 2,741 glyphs, specifically CIDs 20317 through 23057, to completely support the JIS X 0212-1990 character set, and thus obsoletes the Adobe-Japan2-0 character collection, described in [Adobe Technical Note #5097](https://www.adobe.com/devnet/font.html), entitled *Adobe-Japan2-0 Character Collection* for CID-Keyed Fonts. Also included are the glyphs necessary to support Kyodo News’ U-PRESS character set.

### Special Notes

CID+20958 is rendered as a full-width space in this specification, but is allocated for NTT’s *FreeDial* symbol. Font developers who have the right or permission to use this glyph in their font products can thus assign this glyph to CID+20958. Note that the latest Unicode CMap resources map U+27BF ➿ DOUBLE CURLY LOOP to CID+20958.

### JIS C 6226-1978 Coverage

Supplement 6 includes one additional JIS78 (aka, JIS C 6226-1978) glyph, specifically CID+21071 (&#x6EA2;&#xE0102;).

### JIS X 0213:2004 Coverage

Supplement 6 includes three glyphs, specifically CIDs 21072 through 21074, that are intended to complete JIS X 0213:2004 coverage. These three glyphs are for kanji in JIS X 0213:2000 proper, and not among the ten kanji that were added for its 2004 revision.

### JIS X 0212-1990 Coverage

Supplement 6 adds the necessary glyphs to completely cover the JIS X 0212-1990 character set, which contains 6,067 characters. Note that the glyphs for the majority of the JIS X 0212-1990 characters are found in earlier Supplements. The glyphs for CIDs 21075 through 23057 are intended to support JIS X 0212-1990 kanji.

The JIS X 0212-1990 and JIS X 0213:2004 character sets significantly overlap, and some characters shared by them, in terms of sharing the same Unicode mapping, have glyphs that differ, sometimes in very subtle ways. The following list provides thirty-seven pairs of CIDs, specifically the JIS X 0213:2004 form’s CID, followed by the corresponding JIS X 0212-1990 form’s CID in parentheses:

144 (20319), 140 (20320), 7610 (20321), 15739 (20341), 15747 (20359), 16786 (21164), 17469 (21371), 17510 (20107), 15390 (14510), 14541 (21558), 16889 (14609), 17755 (21722), 17850 (21791), 15395 (14741), 14762 (21933), 15397 (14766), 16977 (8561), 18115 (22006), 14160 (22010), 16987 (20177), 13893 (7725), 16994 (22045), 18201 (22063), 17014 (14904), 18316 (22186), 17041 (8592), 18514 (22341), 18713 (22583), 17168 (15238), 18858 (20239), 18854 (22788), 15405 (15269), 18905 (22843), 15319 (22920), 17205 (13372), 19068 (20257), 19091 (23006)

### U-PRESS Coverage

With a couple minor exceptions, the glyphs for CIDs 20473 through 20960 are intended for supporting Kyodo News’ U-PRESS character set. For those font developers who have the right or permission to use NTT’s *FreeDial* symbol in their font products, CID+20958 has been allocated for this specific purpose.

---
## Kana Subset Definitions

In terms of font products developed by Adobe, three different *Kana* subsets have been defined, and are categorized by typeface family and Supplement. Although kana fonts can be used stand-alone, as independent fonts, their limited glyph set means that they are best used as a component of a *Composite Font*, which is functionality found in Adobe InDesign and other higher-end applications. The table below details each kana subset, along with the number of glyphs and their CIDs and CID ranges:

**Kana Subset** | **Supplement** | **Glyphs** | **CIDs & CID Ranges**
--- | --- | --- | ---
*Kamono Kana* Family | 1 | 373 | **0**—0, 232, 233, 238–240, 243, 245–258, 262, 290, 292, 295, 326–331, 503–514, 633–642, 651–655, 659–661, 663, 665, 666, 668, 670–679, 682–693, 695–697, 708, 709, 711–719, 723–739, 780–789, 842–1010, 7612, 7887, 7888, 7891, 7892, 7894, 7895, 7897, 7899–7904, 7907–7939, 7958–7960, 8009–8014, 8210, 8264, 8265, 8268, 8273–8283 & **1**—8307, 8313–8316
*Kamono Kana* Family | 3 | 415 | **0**—0, 232, 233, 238–240, 243, 245–258, 262, 290, 292, 295, 326–331, 503–514, 633–642, 651–655, 659–661, 663, 665, 666, 668, 670–679, 682–693, 695–697, 708, 709, 711–719, 723–739, 780–789, 842–1010, 7612, 7887, 7888, 7891, 7892, 7894, 7895, 7897, 7899–7904, 7907–7939, 7958–7960, 8009–8014, 8210, 8264, 8265, 8268, 8273–8283 & **1**—8307, 8313–8316 & **2**—*none* & **3**—8951, 8952, 8957–8959, 8962, 8964–8977, 8981, 9009, 9011, 9014, 9048, 9084–9089, 9265–9275
*Ryo* Family | 1 | 214 | **0**—0, 633–635, 651–654, 657, 658, 660, 842–1010, 7887, 7888, 7891, 7918–7939, 7958–7960, 8264, 8265 & **1**—8313–8316

For those developers who wish to include a complete set of proportional Latin glyphs with their kana font products, to make the fonts more usable as stand-alone fonts, we suggest that the glyphs for CIDs 1 through 230 (Supplement 0) and 8720 through 8949 (Supplement 3) be included.

## Special Glyphs & Other Notes
The following sections detail special glyphs and other notes that are of interest to font developers. Several glyph classes that are support by Adobe-Japan1-6 are complex, and deserve some amount of explanation and clarification.

### Space Glyphs

The following table lists all of the Adobe-Japan1-6 glyphs that are classified as a space, or are otherwise rendered as a space, and provides information with regard to their intended usage, along with their recommended set widths:

**CID** | **Set Width** | **Description**
--- | --- | ---
1 | Proportional | Latin space—U+0020
231 | Half-width | Latin space—U+2002
326 | Half-width | Katakana space
422 | Half-width | Generic space
515 | Half-width | Hiragana space
633 | Full-width | Ideographic space—U+3000
8229 | Full-width | Generic space
8720 | Full-width | Pre-rotated version of CID+1
8950 | Full-width | Pre-rotated version of CID+231
9084 | Full-width | Pre-rotated version of CID+326
9179 | Full-width | Pre-rotated version of CID+515
9276 | Full-width | Pre-rotated version of CID+422
9444 | Proportional | Italic space
12960 | Full-width | Pre-rotated version of CID+9444
15444 | Full-width | For AAT compatibility—U+F860
15445 | Full-width | For AAT compatibility—U+F861
15446 | Full-width | For AAT compatibility—U+F862
15447 | Full-width | For AAT compatibility—U+F87A
15448 | Full-width | For AAT compatibility—U+F87F
20958 | Full-width | Placeholder for NTT’s *FreeDial* symbol

The space glyphs that are described as a pre-rotated version of another glyph must be assigned full-width set widths in terms of their horizontal set widths, but when instantiated as an OpenType font, their vertical set widths as specified in the OpenType ‘[vmtx](https://www.microsoft.com/typography/otspec/vmtx.htm)’ (*Vertical Metrics*) table should match those of their unrotated counterparts.

### Kana Glyphs

Adobe-Japan1-6 includes a rich variety of kana in terms of glyph classes, specifically half-width, full-width, full-width tuned for horizontal and vertical writing, proportional, ruby, and a special set for U-PRESS.

**Kana Glyph Class** | **Horizontal CIDs & CID Ranges** | **Vertical CIDs & CID Ranges**
--- | --- | ---
Half-width | 332–389, 391–422, 516–598 | 9090–9178, 9180–9262
Full-width | 643, 644, 651–654, 660, 842–1010, 7958–7960, 8313–8316, 12181, 12269, 12271, 16195, 16209–16221, 16236–16252, 16326, 16327 | 7891, 7918–7939, 8264, 8265, 8271, 8272, 12108–12110, 12270, 12272, 16333–16349
Tuned | 12273–12455, 16352–16381 | 12456–12638, 16382–16411
Proportional | 15449–15452, 15455, 15462, 15463, 15517–15724 | 15976–15979, 15982–16192
Ruby | 12649–12652, 12671–12854, 12867, 16414–16449 | 12855–12866, 12868, 16450–16468
U-PRESS | 20473–20496 | *n/a*

### Kanji Glyphs

Adobe-Japan1-6 includes 14,664 glyphs that are classified as kanji (aka, ideographs), and their CIDs and CID ranges, separated by Supplement, are shown in the table below:

**Supplement** | **CIDs & CID Ranges**
--- | ---
0 | 656, 1125–7477, 7633–7886, 7961–8004, 8266–8267
1 | 8284, 8285
2 | 8359–8717
3 | *none*
4 | 13320–15443
5 | 16779–20316
6 | 21071–23057

The *aj16-kanji.txt* datafile provides detailed information for each of these 14,664 kanji.

### Ruby Glyphs

Supplements 4 and 5 include glyphs that are suitable for typesetting ruby glyphs, and the vast majority of the glyphs are for kana, though one kanji and some symbols are also included. Although these glyphs are obviously unencoded, they can be used by applications that support the OpenType ‘[ruby](https://www.microsoft.com/typography/otspec/features_pt.htm#ruby)’ (*Ruby Notation Forms*) GSUB feature. The following table details the CID ranges for the ruby glyphs in Supplements 4 and 5:

**Supplement** | **CID Ranges**
--- | ---
4 | 12639–12869
5 | 16412–16468

### Italic Glyphs

Italic glyphs were introduced in Supplement 4, and are also found in Supplements 5 and 6. The table below explicitly indicates the CID ranges for the italic glyphs in these three Supplements, along with their corresponding pre-rotated glyphs within the same Supplement:

**Supplement** | **Italic CID Ranges** | **Pre-Rotated CID Ranges**
--- | --- | ---
4 | 9444–9737 | 12960–13253
5 | 15912–15975 | 16715–16778
6 | 20372–20426 | 21016–21070

### Pre-Rotated Glyphs

In order to support the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB feature, the Adobe-Japan1-6 character collection includes pre-rotated forms for all Latin and Latin-like glyphs that are not full-width. The table below details how horizontal CIDs and CID ranges map to their corresponding pre-rotated CID ranges:

**Supplement** | **Horizontal CIDs & CID Ranges** | **Pre-Rotated CID Ranges**
--- | --- | ---
3 | 1–325, 390, 501–503, 599–628, 630–632, 8718, 8719, 326–389, 391–421, 515–598, 423, 424, 504–514, 422, 425–500, 629 | 8720–9353
4 | 9354–9778, 12063–12087 | 12870–13319
5 | 15456–15461, 15464–15516, 15725–15975 | 16469–16778
6 | 20317–20426 | 20961–21070

### Glyph Set Widths

The following table provides CIDs and CID ranges that explicitly indicate which glyphs are intended to be designed with proportional-, half-, third-, or quarter-width set widths. All other glyphs are expected to be full-width.

**Set Width** | **CIDs & CID Ranges**
--- | ---
Proportional | 1–230, 9354–9737, 15449–15975, 20317–20426
Half-width | 231–632, 8718, 8719, 12063–12087
Third-width | 9758–9778
Quarter-width | 9738–9757

The glyph tables that are provided in this document include registration marks that serve to indicate relative set width. Explicitly specifying width classes, such as in the above table, is clearly more accurate and reliable than measuring the distance between registration marks. Please use both resources as your guide.

Note that the registration marks used in the glyph tables are in a separate layer, and if their presence is annoying, that layer can be turned off, thus preventing their display.

### Duplicate Kanji Glyphs

For historical reasons and for JIS90-compliance, the following three Supplement 0 kanji glyph pairs represent genuine duplicate glyphs, and their JIS83 (aka, JIS X 0208-1983) forms in Supplement 4 are shown for the sake of comparison:

**Primary Glyph** | **Duplicate Glyph** | **JIS83 Form**
--- | --- | ---
4301—&#x5315;&#xE0100; | 7983—&#x5315;&#xE0101; | 13523—&#x2090E;&#xE0100;
4411—&#x55A9;&#xE0100; | 7984—&#x55A9;&#xE0101; | 13526—&#x55A9;&#xE0102;
5459—&#x6E23;&#xE0100; | 7994—&#x6E23;&#xE0101; | 13558—&#x6E23;&#xE0102;

For the purposes of full compliance and character collection integrity, the duplicate glyphs shown above shall be maintained.

In addition, the glyphs for CIDs 3603 (Supplement 0) and 13505 (Supplement 4) are identical when rendered with the *Kozuka Mincho* typeface design, but may be rendered differently for other typeface designs.

### Glyph Variation

In order for fonts based on the Adobe-Japan1-6 character collection to be useful, meaningful, consistent, and predictable, the glyphs that correspond to the kanji in the JIS X 0208:1997 character set must be designed in such a way that they are JIS90-compliant, meaning that their glyphs match the prototypical glyphs set forth in the JIS X 0208-1990 standard. As mentioned earlier, this affects CIDs 1125 through 7477 (6,353 glyphs) in Supplement 0, along with CIDs 8284 and 8285 in Supplement 1, in order to completely cover all possible JIS90 glyphs. Subtle glyph variations in Supplement 4 and beyond make this necessary.

For font developers who wish to build JIS2004-savvy OpenType fonts, specifically those whose default glyphs match the prototypical glyphs set forth in the JIS X 0213:2004 standard, the strong JIS90-compliance recommendation still applies, because the JIS2004-savviness is achieved at the character code, not CID, level, through the use of JIS2004-savvy CMap resources that map the same Unicode code points to CIDs whose glyphs match the JIS X 0213:2004 prototypical glyphs. JIS2004-savvy font development is covered later in this document.

The JIS standards, specifically JIS X 0208:1997, JIS X 0212-1990, and JIS X 0213:2004, and earlier versions thereof, along with JIS-related material found in the appendixes of the book entitled [*CJKV Information Processing*, Second Edition](http://shop.oreilly.com/product/9780596514471.do) (O’Reilly, 2009), serve as the ideal glyph references for Adobe-Japan1-6, at least for the glyphs that correspond to these standards. Some glyphs do not correspond to characters found in any JIS standard, in which case Unicode and ISO 10646 serve as the ideal glyph reference, and in some cases the only glyph reference beyond this document. The [*aj16-kanji.txt*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/aj16-kanji.txt) datafile, described in the section that follows, also provides references to other standards that can also be consulted in terms of glyph references.

## CMap Resources

The CMap resources associated with the Adobe-Japan1-6 character collection, along with the [*cid2code.txt*](https://raw.githubusercontent.com/adobe-type-tools/cmap-resources/master/Adobe-Japan1-6/cid2code.txt) datafile that provides additional details for font developers, are available as part of the [*CMap Resources*](https://github.com/adobe-type-tools/cmap-resources/) open source project.

The [*aj16-kanji.txt*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/aj16-kanji.txt) datafile provides additional information for all 14,664 kanji in Adobe-Japan1-6.

More complete descriptions of the individual Adobe-Japan1-6 CMap resources can be found in [Adobe Technical Note #5094](https://www.adobe.com/devnet/font.html), entitled *Adobe CJKV Character Collections and CMap Files for CID-Keyed Fonts*.

In general, the CMap resources that are based on legacy encodings, such as Shift-JIS, are no longer being updated. Rather, the Unicode CMap resources—available for UTF-8, UTF-16 (UTF-16BE), and UTF-32 (UTF-32BE) encodings, and kept perfectly synchronized—are updated on a regular basis, with new mappings being triggered by a new Supplement or a new version of Unicode. Furthermore, the UCS-2 CMap resources are obsolete and deprecated. Developers should use the UTF-16 CMap resources instead, because they are forward compatible with the now-obsolete UCS-2 ones.

## Unicode Variation Sequences

The Ideographic Variation Sequences (IVSes) that are specified in the [*Adobe-Japan1_sequences.txt*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/Adobe-Japan1_sequences.txt) datafile are registered by The Unicode Consortium in the [IVD](http://www.unicode.org/ivd/) (*Ideographic Variation Database*) per [UTS #37](http://www.unicode.org/reports/tr37/) (*Unicode Ideographic Variation Database*). This datafile also includes a small number of [Standardized Variation Sequences](http://www.unicode.org/Public/UCD/latest/ucd/StandardizedVariants.txt) (SVSes), and all but one of them correspond to CJK Compatibility Ideographs.

## OpenType Font Development

Given today’s dominance of OpenType fonts, this section provides information intended to help with OpenType font development efforts with regard to those built based on the Adobe-Japan1-6 character collection. Adobe considers the minimum Supplement for an OpenType Japanese font to be 3, specifically Adobe-Japan1-3. The sections that follow provide information on building JIS2004-savvy OpenType fonts, and detail an industry-standard naming convention.

### JIS2004-Savvy OpenType Fonts

All Adobe-Japan1-6 fonts are JIS2004-*compatible*, because all of the prototypical glyphs shown in JIS X 0213:2004 proper are included, but may not be the default, in terms of whether they are encoded. Whether a glyph is encoded is a function of the CMap resource that is used, and in the case of OpenType fonts, it is a function of what CMap resource is used to build the Formats 4 and 12 ‘[cmap](https://www.microsoft.com/typography/otspec/cmap.htm)’ subtable.

When developing JIS2004-*savvy* OpenType fonts, specifically those whose default glyphs match the prototypical glyphs set forth in the JIS X 0213:2004 character set standard, the appropriate UTF-32–encoded CMap resource must be used to build the Formats 4 and 12 ‘[cmap](https://www.microsoft.com/typography/otspec/cmap.htm)’ subtables. For fonts based on Supplements 3 through 5, additional glyphs beyond each Supplement are necessary for JIS2004-compliance, which requires the advertised Supplement to be set to 6. For Supplements 3 through 5, the following table details the number of glyphs that are necessary beyond those in each of these Supplements, and also indicates which JIS2004-savvy CMap resources should be used to build their Formats 4 and 12 ‘[cmap](https://www.microsoft.com/typography/otspec/cmap.htm)’ subtables:

**Supplement** | **Advertised Supplement** | **CMap Resource** | **CIDs**
--- | --- | --- | ---
3 | 6 | UniJIS2004-UTF32-H or UniJISX02132004-UTF32-H | Adobe-Japan1-3 + 144 Supplement 4–6 glyphs
4 | 6 | UniJIS2004-UTF32-H or UniJISX02132004-UTF32-H | Adobe-Japan1-4 + 81 Supplement 5 & 6 glyphs
5 | 6 | UniJIS2004-UTF32-H or UniJISX02132004-UTF32-H | Adobe-Japan1-5 + 10 Supplement 6 glyphs

The advertised Supplement is the integer value that is recorded in the /Supplement entry of the /CIDSystemInfo dictionary of the CIDFont resource. The following table provides a complete listing of the additional glyphs necessary for each of these three special-case JIS2004-savvy OpenType font types, distinguished by Supplement:

**Supplement** | **Glyphs** | **CIDs & CID Ranges**
--- | --- | ---
3 | 144 | **4**—9354,  9779, 12101, 12870, 13320–13327, 13330, 13332–13333, 13335–13341, 13343, 13345–13355, 13358–13369, 13371, 13373–13382, 13385–13388, 13391–13400, 13402, 13460, 13495, 13538, 13624, 13650, 13673, 13731, 13803, 13860, 13893, 13915, 13949, 13964, 14013, 14066, 14074, 14111, 14116, 14196, 14272, 14290 & **5**—16977, 17041, 18760, 19312, 19346, 20175, 20222, 20263–20296, 20301–20305, 20307, 20314 & **6**—21072–21074
4 | 81 | **5**—16413, 16444–16449, 16467–16468, 16889, 16905, 16977, 17014, 17041, 17168, 17205, 18759–18760, 19061, 19312, 19346, 20175, 20222, 20263–20296, 20299–20310, 20312–20315 & **6**—21071–21074, 21558, 21933, 22010, 22920
5 | 10 | **6**—21071–21074, 21371, 21558, 21722, 21933, 22010, 22920

Because the scope of each Supplement is different, in terms of coverage of JIS standards, the additional glyphs required beyond each Supplement are not in a subset/superset relationship. For example, the scope of Supplements 3 and 4 is JIS X 0208, for Supplement 5 is it JIS X 0208 and JIS X 0213, and for Supplement 6 it is JIS X 0208, JIS X 0213, and JIS X 0212.

### OpenType Font Naming Conventions

In order to clearly distinguish OpenType Japanese fonts based on different Supplements, we strongly recommend that the names used for the fonts, specifically the /CIDFontName string and the OpenType menu names in the ‘name’ table, include a designator for this purpose. The table below illustrates the naming convention that is in current use, and thus industry standard, and provides example /CIDFontName and OpenType menu name strings with the designator emboldened:

**Supplement** | **Designator** | **JIS2004-Savvy Designator** | **/CIDFontName & Menu Name Examples**
--- | --- | --- | ---
3 | Std | StdN | KozMinStd-Regular, 小塚明朝 Std R & KozMinStdN-Regular, 小塚明朝 StdN R
4 | Pro | ProN | KozMinPro-Regular, 小塚明朝 Pro R & KozMinProN-Regular, 小塚明朝 ProN R
5 | Pr5 | Pr5N | KozMinPr5-Regular, 小塚明朝 Pr5 R & KozMinPr5N-Regular, 小塚明朝 Pr5N R
6 | Pr6 | Pr6N | KozMinPr6-Regular, 小塚明朝 Pr6 R & KozMinPr6N-Regular, 小塚明朝 Pr6N R

This naming convention also allows JIS2004-savvy OpenType fonts to coexist with earlier versions of the same font, even if they are based on the same Supplement. Also, the advertised Supplement does not affect which designator is used. For example, a JIS2004-savvy Adobe-Japan1-3 font includes 144 additional glyphs from Supplements 4 through 6, but “StdN” shall be used as its designator.

## Glyph Tables

Representative glyphs for CIDs 0 through 23057 are provided in the [*Adobe-Japan1-6.pdf*](https://github.com/adobe-type-tools/Adobe-Japan1/raw/master/Adobe-Japan1-6.pdf) file that is included in this repository, with 500 glyphs shown per page. And, for reader convenience, the beginning of each Supplement is clearly marked. The typeface used to exemplify each glyph is *Kozuka Mincho Pr6N R* (aka, KozMinPr6N-Regular or 小塚明朝 Pr6N R), designed by Adobe, and an Adobe Original typeface available for license. The specific font instance is Version 6.004, as reflected in its /CIDFontVersion dictionary entry.

## Changes Since Earlier Versions

The following sections detail the history of this document, which was originally referred to as Adobe Technical Note #5078. Note that references to specific sections no longer correspond to the sections found in the current version of this specification.

### Since the 1993-06-11—Supplement 0—Version

Supplements 1 and 2 were added, with the glyphs shown in Sections 4 and 5, respectively.

### Since the 1994-10-04—Supplement 2—Version

Morisawa’s RyuminPro-Light (Ryumin Light KL) typeface design is now used for the representative glyphs for each CID—FDPC’s HeiseiMin-W3 (*Heisei Mincho W3*) was previously used. Supplements 3 and 4 were added, with the glyphs shown in Sections 6 and 7, respectively.

### Since the 2000-03-31—Supplement 4—Version

KozMinPro-Light (*Kozuka Mincho Pro L*), an Adobe Original typeface design, is now used for the representative glyphs for each CID—RyuminPro-Light was previously used. The representative glyphs for CIDs 13863 and 15438 were corrected, and the representative glyphs of the following CID pairs were exchanged:

* 7776 & 13982
* 7777 & 13983

### Since the 2000-08-12—Supplement 4—Version

The representative glyphs for CIDs 15408 and 15435 were corrected.

### Since the 2000-11-01—Supplement 4—Version

The representative glyphs are from KozMinPro-Light (*Kozuka Mincho Pro L*) with /CIDFontVersion value 1.011. The representative glyphs for CIDs 740, 8270, 12068, and 13300 were modified, and the representative glyphs for CIDs 7879 and 8002 were corrected.

### Since the 2002-06-21—Supplement 4—Version

All 23,058 representative glyphs are from KozMinProVI-Light (*Kozuka Mincho Pro-VI L*) with /CIDFontVersion value 6.004. The representative glyphs for Supplements 5 (CIDs 15444 through 20316) and 6 (CIDs 20317 through 32057) were added as Sections 8 and 9, respectively. The following 24 additional glyphs were added to the Adobe-Japan1-0 kana subset definition in Section 1.1: CIDs 7958–7960, 8009–8014, 8210, 8264–8265, 8268, and 8273–8283. Glyph variation notes for CIDs 140, 144, 9583, and 9587 were removed from Section 1.4. Special notes for CIDs 243 and 245 were added in Section 3.1. Special notes for CIDs 8962 and 8964 were added in Section 6.1. Special notes for CIDs 12220 through 12227 were added in Section 7.1. The representative glyphs for CIDs 243, 245, 8962, and 8964 were modified so that they are centered within their half-width (500-unit) set widths, and the representative glyphs for CIDs 6510, 7803, 7967, 7981, 9437, 12953, 14935, and 15310 were corrected.

### Since the 2004-06-11—Supplement 6—Version

The representative glyphs for CIDs 740, 1879, 8270, 12068, and 13300 were corrected. KozMinPr6N-Regular (*Kozuka Mincho Pr6N R*) with /CIDFontVersion value 6.002 was used for the representative glyphs. The entire specification was completely revised.

### Since the 2008-02-15—Supplement 6—Version

The representative glyphs for CIDs 7721, 7752, 7780, 7984, 8547, 15825, and 16628 were corrected, and the representative glyphs for CIDs 8721–8949, 12870–12959, 12961–13253, 16469–16778, and 20961–21070 were shifted 47 units to the right. KozMinPr6N-Regular (*Kozuka Mincho Pr6N R*) with /CIDFontVersion value 6.004 was used for the representative glyphs. The entire specification was ported to GitHub markdown syntax and revised.

### Since the 2017-10-03—Supplement 6—Version

The *Anticipated Changes* section was moved to the project's [Wiki](https://github.com/adobe-type-tools/Adobe-Japan1/wiki) for easier maintenance.

That is all.
