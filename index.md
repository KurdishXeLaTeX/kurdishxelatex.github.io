---
layout: default
title: Kurdish XeLaTeX Users Group
nav_order: 1
description: "Kurdish XeLaTeX Users Group homepage."
permalink: /
---

## Welcome to the
# Kurdish XeLaTeX Users Group
{: .fs-9 }

This group promotes the usage of the wonderful XeLaTeX typesetting system for writing Kurdish language by providing educational content and creating a platform to facilitate collaboration within the Kurdish scientific communities. 
{: .fs-6 .fw-300 }

<!-- [Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 } -->

---

## The Kurdish language

Kurdish is an Indo-European language widely spoken among the Kurdish population in the Middle East and the Kurdish diaspora around the world. The Kurdish language is considered as a dialect continuum with mainly three dialects, Sorani, Kurmanji and Southern Kurdish, and also has mutual intelligibility with the Zaza–Gorani languages. Among the Kurdish dialects, Sorani and Kurmanji are widely used in education and media. In addition to the dialect diversity, Kurdish uses various scripts and follows different writing norms, such as the use of numerals and punctuation marks, due to its unique administrative situation. Currently, two scripts are widely used for writing Kurdish: Latin and Persian-Arabic, which are both based on phonemic orthographies. Although these two scripts are widely used for writing all the dialects of Kurdish, among the Kurmanji and Sorani speakers, the Latin and the Persian-Arabic scripts are respectively more popular.


## Kurdish in Polyglossia

[`Polyglossia`](https://github.com/reutenauer/polyglossia) is a modern multilingual typesetting in XeLaTeX and LuaLaTeX which is supporting over 70 languages. Given the diversity in scripts and dialects of Kurdish, `Polyglossia` is an ideal package to support the Kurdish language. Therefore, we added the Kurdish configuration to this package.

The following shows a minimal working example to run Kurdish XeLaTeX with `Polyglossia`:

```tex
\documentclass{article}
\usepackage{polyglossia}

\setdefaultlanguage[variant=sorani,script=Arabic,numerals=eastern]{kurdish}
\newfontfamily\arabicfont[Script=Arabic,Scale=1]{Yas}
\let\arabicfonttt\ttfamily

\title{بەڵگەیەک بۆ نموونە}
\author{نێوی من}
\date{\today}

\begin{document}

\maketitle

\end{document}
```

The configuration of Kurdish in `Polyglossia` includes **Sorani** and **Kurmanji** in both scripts, **Persian-Arabic** and **Latin** with the following options:

| Polyglossia name        | variant          | script | numerals | 
|:-------------|:------------------|:------| :------- |
| Kurdish          | sorani | arabic, latin  | eastern, western |
| Kurdish | kurmanji  | arabic, latin  | eastern, western |


- `variant`: `kurmanji` or `sorani` (*default*)
- `script`: `arabic` or `latin`
- `numerals`: `western` or `eastern`
- `locale`: currently set by default
- `calendar`: currently set by default to the Gregorian calendar of Kurdish


The scripts for Sorani and Kurmanji are by default `arabic` and `latin`. In addition to the default `\today`, `\ontoday` can be used to take the Izafa structure of Kurdish into account. For instance, the first command produces *15 Gulan 2020* (May 15, 2020) while the latter takes the morphological change into account by producing *15ê Gulanê 2020* (literally meaning, 15 of May of 2020). This option is available for both dialects in the Latin script.

For more information on the configuration of Kurdish in `Polyglossia`, see [this](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/KurdishXeLaTeX/Support/master/docs/Kurdish_XeLaTeX_English.pdf){:target="_blank"}.

## Documenation

You can find simple documentations on XeLaTeX typesetting in various dialects and scripts in the following:

- Sorani dialect in Persian-Arabic script: [XeLaTeX بۆ نووسینی کوردی]({{site.url}}/assets/Kurdish_XeLaTeX_Sorani_Arabic.pdf){:target="_blank"}
- Sorani dialect in Latin script: [XeLaTeX bo Nûsînî Kurdî]({{site.url}}/assets/Kurdish_XeLaTeX_Sorani_Latin.pdf){:target="_blank"}
- Kurmanji dialect in Latin script: [XeLaTeX ji bo nivîsandina Kurdî]({{site.url}}/assets/Kurdish_XeLaTeX_Kurmanji_Latin.pdf){:target="_blank"}
- Kurmanji dialect in Persian-Arabic script: [XeLaTeX ژ بۆ نڤیساندنا کوردی]({{site.url}}/assets/Kurdish_XeLaTeX_Kurmanji_Arabic.pdf){:target="_blank"}

---

## About the project

Our main focus within this project is to create content in Kurdish for the Kurdish scientific communities. You can consult our websites in [Sorani](https://kurdishxelatex.github.io/Sorani) and [Kurmanji](https://kurdishxelatex.github.io/Kurmanji). 


### Contributing

If you are using the XeLaTeX typesetting (or you would like to) and also have an interest in the Kurdish language, please consider joining our group. You can also raise your issues or suggest ideas to improve our content. 

<!-- Read more about becoming a contributor in [our GitHub repo](https://github.com/pmarsceill/just-the-docs#contributing). -->

#### Thank you to the contributors of the Kurdish XeLaTeX Users Group!

<!-- <ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul> -->

