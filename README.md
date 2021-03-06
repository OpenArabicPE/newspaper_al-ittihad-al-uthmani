---
title: "newspaper_al-ittihad-al-uthmani: read me"
author: Till Grallert
date: 2021-05-26
ORCID: orcid.org/0000-0002-5739-8094
---

This repository contains bibliographic metadata for the newspaper *al-Ittiḥād al-ʿUthmānī* published by Aḥmad Ḥasan Ṭabbārā in Beirut after 1908.

# some technical details

This repository contains the following files:

1. a [TEI XML](metadata/thamarat-al-funun.TEIP5.xml) file containing one `<biblStruct>` for each issue of *al-Ittiḥād al-ʿUthmānī*. This file is produced through automatic iteration making use of [this code developed for OpenArabicPE](https://github.com/OpenArabicPE/generate_metadata-through-iteration/tree/al-ittihad-al-uthmani) and manual validation against the digital facsimiles.
2. individual TEI files for every issue of *al-Ittiḥād al-ʿUthmānī*. These are generated from the output of step 1 using the XSLT stylesheet [`generate_tei-from-biblstruct.xsl`](https://github.com/OpenArabicPE/generate_metadata-through-iteration/blob/thamarat-al-funun/xslt/generate_tei-from-biblstruct.xsl) from the same repository. TEI files contain links to the locally available facsimiles.
3. all bibliographic data is then [automatically converted](https://www.github.com/OpenArabicPE/convert_tei-to-mods) from TEI XML to MODS XML for integration into reference management software etc (such as Zotero).
4. The TEI files for individual issues were [converted to TSS XML](https://github.com/OpenArabicPE/convert_tei-to-sente/) for use with the now discontinued reference manager Sente.