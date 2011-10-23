Eccehomo-cv : LaTeX resume template with multi-language support
===============================================================
Manuel Vonthron - `<manuel DOT vonthron AT acadis DOT org>`
Version 1.0 - 2011


Install
-------
* Copy (or link) the eccehomo-cv folder in your LaTeX distribution directory  
    executing `locate xkeyval.sty` should give you a hint
* Update the TeX index with `texhash`. You may need to be root.


Basic usage
-----------
*  `\usepackage[en]{eccehomo-cv}`
*  `\author{}`
*  `\printmargin{}`
*  `\headline{}`
*  `\lastupdated{}`

*  `section` environment
*  `\subsection`
*  `\place{}`
*  `\position{}`
*  `\item{}`

Multi-language usage
--------------------
This is a work in progress. Only french-english combination is supported at
this time. More info soon.

There are two ways of providing translated content. For now, each command
only accept one of them:
* Optional language argument:  
  `\subsection[en]{This is a subsection}` and `\subsection[fr]{Ceci est une sous-section}`
* Localized content array:
  `\begin{section}{en={This is a section}, fr={Ceci est une section}}`
