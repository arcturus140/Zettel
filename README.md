# Zettel
![](https://github.com/flengyel/Zettel/blob/main/f277683c33c80bdd60626e8c88557aba.png)

---

This repository contains a Zettel template and an abbreviates Zettel template for use with a software implementation of the Zettelkasten Method. The Zettelkasten Method is documented online at [Introduction to the Zettelkasten Method](https://zettelkasten.de/posts/overview/) on the [Zettelkasten.de](https://zettelkasten.de) site and in the [Zettelkasten.de forum](https://forum.zettelkasten.de). The templates are intended to be self-documenting. Further documentation and sample Zettels may be added to the repository in the future.

As of November 18, 2021, the template was developed for Zettlr 2.0.3 + Pandoc 2.16.1 + MikTeX 21.2-x64 + Zotero 5.0.96.3 + BetterBibTex  5.6.8 under Windows 10; it has not been tried with other software. 


This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

---

# 20211119115201 Abbreviated Zettel template v2.4

**CONTEXT** [[20211118010533]] Zettel template v2.4

#replace #these

A Zettel has three parts: a header, a body, and a footer.  The header starts with an optional YAML header and includes a level 1 (H1) header with a timestamp ID and a title; a CONTEXT line that links to a Zettel that this Zettel continues or comments (or raises a question about) on an aspect of that Zettel (if there such a Zettel); and a list of hashtag keywords. This text is part of the body. Footnotes and endnotes become links within the body to other Zettels. That leaves the References section for the footer. The References section below can be omitted, generated with a reference manager such as Zotero and a YAML header [[20211118010533]] Zettel template v2.1; or added by hand, as below. 

-   This Zettel format only applies to Zettlr 2.2.1 + Pandoc 2.16.1 + MikTeX 21.2-x64 + Zotero 5.0.96.3 + BetterBibTex  5.6.8 under Windows 10 and has not been used with other software.  
-   Filenames have the format `timestamp.md` in my implementation.
-   See [From Fleeting Notes to Project Notes - zettelkasten.de](https://zettelkasten.de/posts/concepts-sohnke-ahrens-explained/) for definitions of terms in (Ahrens 2017) 

The following checklist in Markdown is a first attempt (Gawande 2010). 

- [ ] Replace the header timestamp ID with your own ID. 
- [ ] Replace the title with your title.
- [ ] Replace the link after the **CONTEXT** keyword with a link to a Zettel Z such that this Zettel   
    - [ ] continues Z; or
    - [ ] comments on (or raises a question about) an aspect of Zettel Z; otherwise,
    - [ ] if there is no such prior Zettel Z, and this Zettel starts a new topic, link to an index. 
- [ ] Replace the hashtags above with your own #hashtag keywords
- [ ] Replace the body (including this cheklist) with your own text and Markdown in the body. 
- [ ] Are there footnotes or endnotes? 
    - [ ] Footnotes and endnotes become links within the body to other Zettels. 
- [ ] If there are literature citations from a citation manager (Zotero is assumed here) 
    - [ ] Add citations in Pandoc format. 
        - [ ] Verify that the Zotero Citation Database is exported in CSL JSON format and specified in Preferences → Export → Citation Database;
        - [ ] Add a YAML header to beginning of this document (see [[20211118010533]] Zettel template v2.1); or
    - [ ] A references section can be added by hand, as below.
- [ ] Does this Zettel stand on its own?
- [ ] Is there a summary sentence?
- [ ] Is this Zettel limited to at most a screen of text? 

# References

Ahrens, Sönke. 2017. _How to take smart notes: one simple technique to boost writing, learning and thinking: for students, academics and nonfiction book writers_. North Charleston, SC: CreateSpace.

Gawande, Atul. 2010. *The checklist manifesto: how to get things right*. New York, N.Y: Metropolitan Books.

---

# 202202040853 Zettel template v2.4

 #zettel #zettelkasten #ruleofthrees #folgezettel #replace #these 

**CONTEXT** [[20211118010533]] Zettel template v2.1

Revision v2.4 Context and hashtag sections reordered. The context section is now first, since it is important to know where the Zettel fits into the "slip-box."

Revision v2.3 Errors of interpretation of Ahrens corrected. Humiliating, damning errors.

Revision v2.2 after rereading S&ouml;nke Ahrens on the three categories of notes and on consideration of the Three Dicta of (Winebrenner 2022). 

Revision v2.1 following remarks by (Simpson 2021), with additional citations.

-   This Zettel format applies to Zettlr  versions 2.0.3 through 2.2.1 + Pandoc 2.16.1 + MikTeX 21.2-x64 + Zotero 5.0.96.3 + BetterBibTex  5.6.8 under Windows 10.   
-   Filenames have the format `timestamp.md` in my implementation.

## 1. Header: in 3 + 1 parts

-   An optional YAML frontmatter header with commands to Zettlr and Pandoc;
-   a Level 1 (H1) header containing an immutable ID, referred to in this Zettel by `immutableID`, followed by a title, referred to in this Zettel by `title`;
-   the keyword **CONTEXT** followed by a list of IDs of prior Zettels providing the immediate context for `immutableID` (see 1.c.2 below); and,
-   a list of keywords in #hashtag format.


> The meta-variables ‘`immutableID`’ and ‘`title`’ are indexicals in the meta-language. The preceding sentence is in the  meta-meta-language since it quotes meta-linguistic terms. The  header of this Zettel is in the object language. For the utility  of keeping the object language, meta-language and  meta-meta-language separate, see (Chakraborty, Dutta, and SpringerLink (Online service) 2019).

### 1.a YAML frontmatter: optional

\---  
reference-section-title: References    
\---

> If there are Pandoc-style references in the Zettel body, add the preceding YAML frontmatter header to the beginning of `immutableID`. References will appear as the last section of the document in Pandoc output. 

###  1.b. An immutableID and title at heading level 1

\# `immutableID` `title`

\[\[20210424174054\]\] Zettlr title format \#+ImmutableID+Title,

> The value of `immutableID` doesn’t change, although `title` might  change. This syntax relies on enabling the Zettlr  `Preferences → Display` setting “If present, use the first heading  level 1 instead of the filename.” This will display the IDs and  titles of Zettel markdown files in the Zettlr file manager pane.  Without this setting, the file manager will only show the Zettlr  filenames, which in my implementation are IDs.

###   1.c.1. CONTEXT Zettel IDs

The keyword CONTEXT followed by a list of wikilinks of Zettel IDs such that for each `ID` in the list, `immutableID` either:

-   continues `ID`;  
-   comments on (or raises a question about) an aspect of `ID`; 
-   is continued by `ID`; or,
-   begins a new topic and `ID` is the wikilink of an index.
-   No other Zettel ID belongs with CONTEXT.

The keyword CONTEXT applies to Zettel IDs satisfying the above conditions only. Zettels that might provide context for ```immutableID``` in other senses of the term 'context' are excluded. 

> The CONTEXT header section is adaptation of Niklas Luhmann’s Folgezettel ID system to digital Zettelkasten. Folgezettel IDs are  spanning tree coordinates for the graph of Zettels of a Zettelkasten (c.f. [[[20211030133016](https://forum.zettelkasten.de/discussion/comment/13422/#Comment_13422)]]  Folgezettel Formalized). In addition to specifying the location of a Zettel in a distinguished spanning tree, a Folgezettel ID indicates whether that Zettel: continues a  prior Zettel; comments on or raises a question about an aspect of a prior Zettel; or, begins a new topic. If the current Zettel with ID `immutableID` begins a new topic, link to an index with ID [[00000000000000]] (for example). The index Zettel serves as the default context that `immutableID` "continues."


### 1.c.2. Keywords in \#hashtag format

\#keyword \#example

> Paraphrasing Sascha Fast in (Fast 2018), hashtags should be as specific to `immutableID` as possible.

## 2. Body: a self-contained note

-   Some authors recommend limiting the body to a single “unit of thought.”
-   Links \[\[to other Zettels\]\] and external links can go here.
-   Footnotes and endnotes become links \[\[to other Zettels\]\] in the body.
-   In a footnote or endnote Zettel, the ID `immutableID` is added to **RELATED**.

> Ahrens recommends limiting each Zettel to a screenfull of text (a test that this Zettel fails). To my knowledge, there is no standard “unit of thought” maintained at the [National Institute of Standards and Technology](https://www.nist.gov/); the [Bureau international des poids et mesures](https://www.bipm.org/en/home); or elsewhere.  Ahrens identifies three types of notes: _fleeting_, _permanent_ and _project notes_ (Ahrens 2017). Fleeting notes are notes to be rewritten as permanent notes before they are discarded. Permanent notes are either Zettels or citations in a reference manager, such as Zotero. Literature notes in Ahrens are the only permanent notes that Ahrens names explicitly: the most important notes in a Zettelkasten would be described in his terms as permanent non-literature notes -- we call those "Zettels."  Literature notes are citations (possibly with attached notes -- the term 'note' for 'citation' is confusing) in a reference manager; e.g., Zotero. The term "permanent" does not mean "immutable"&mdash;notes and citations can be revised, however revision of a Zettel can obliterate a record of what does not work and can affect every note accessible from it. Ahrens advises Zettel writers to read with pen and paper in hand, to take fleeting notes judiciously, and to reformulate their fleeting notes as Zettels in their own words before committing them as permanent notes to their Zettelkasten (Ahrens 2017).  Since Ahrens omits concrete examples of Zettels, this template attempts to address that omission. Zettels will require rewriting and reorganization prior to their use in long-form articles and projects&mdash;cf. the Three Dicta of (@Winebrenner 2022). Ahrens describes a bottom-up process for drawing upon the Zettelkasten in larger writing projects (Ahrens 2017). Apparently, Niklas Luhmann himself did not follow Ahrens' advice at the writing stage: Hans Georg-Moeller  speculates that Luhmann’s Zettelkasten contributed to an  “unnecessarily convoluted, poorly structured, highly repetitive” writing style lacking a “clear narrative development” (Moeller 2012, chap. 2). For a clear guide to writing style, see *Style: Lessons  in Clarity and Grace* (Williams and Bizup 2017). Avoid *The Elements of Style* (Pullum 2010, 2014). Sascha Fast recommends writing for your future self (Fast 2021). Cory Doctorow maintains that writing and  research are distinct, and recommends writing the placeholder "TK" inline instead of stopping to research (Doctorow 2009). At this  point, Zettel writing could use a checklist (Gawande 2010).


## 3.  Footer: References

\[\[20210803113219\]\] Zotero: citing BetterBibTeX references in Zettlr

> Pandoc style references in the body are resolved under References, provided the `immutableID` contains a Pandoc citation and the YAML header of 1.a.

# References

Ahrens, Sönke. 2017. _How to take smart notes: one simple technique to boost writing, learning and thinking: for students, academics and nonfiction book writers_. North Charleston, SC: CreateSpace.

Chakraborty, Mihir K., and Soma Dutta. 2019. *Theory of graded consequence: a general framework for logics of uncertainty*. Logic in Asia: Studia Logica Library. Singapore: Springer.

Doctorow, Cory. 2009. “Cory Doctorow: Writing in the Age of Distraction.” January 7, 2009. http://www.locusmag.com/Features/2009/01/cory-doctorow-writing-in-age-of.html

Fast, Sascha. 2018. “The Difference Between Good and Bad Tags.” Blog. *Zettelkasten* (blog). September 24, 2018. https://zettelkasten.de/posts/object-tags-vs-topic-tags

Fast, Sascha. 2021. “Write for Your Future Self.” July 29, 2021. https://forum.zettelkasten.de/discussion/comment/12480/#Comment_12480

Gawande, Atul. 2010. *The checklist manifesto: how to get things right*. New York, N.Y: Metropolitan Books.

Moeller, Hans-Georg. 2012. *The radical Luhmann*. New York: Columbia University Press.

Plass, Jan L., Roxana Moreno, and Roland Brünken, eds. 2010. *Cognitive load theory*. 1. publ. Cambridge: Cambridge University Press.

Pullum, Geoffrey K. 2010. “The Land of the Free and *The Elements of Style*.” *English Today* 26 (2): 34–44. https://doi.org/10.1017/S0266078410000076

———. 2014. “Fear and Loathing of the English Passive.” *Language & Communication* 37 (July): 60–74. https://doi.org/10.1016/j.langcom.2013.08.009

Simpson, Will. 2021. “Comment 13603 on Zettel Format.” Blog. *Zettelkasten Forum* (blog). November 15, 2021. https://forum.zettelkasten.de/discussion/comment/13603/#Comment_13603

Williams, Joseph M., and Joseph Bizup. 2017. *Style: lessons in clarity and grace*. Twelfth edition. Always learning. Boston Columbus Indianapolis New York San Francisco Amsterdam Cape Town Dubai London Madrid Milan Munich Paris: Pearson.**

Winebrenner, Caleb. 2022. “Field Report #4: I spent six months using a Zettelkasten to write my thesis. Here’s what I learned.” _Zettelkasten_ (blog). January 28, 2022. https://zettelkasten.de/posts/field-report-4-what-i-learned-writing-thesis-with-zettelkasten/.

