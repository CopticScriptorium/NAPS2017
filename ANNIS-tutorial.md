# ANNIS Tutorial
## Introduction to ANNIS
Coptic Scriptorium uses the [ANNIS](http://corpus-tools.org/annis/) search and visualization tool. You can access Coptic Scriptorium's corpora in ANNIS in multiple ways:
* Go directly to [https://corpling.uis.georgetown.edu/annis/scriptorium](https://corpling.uis.georgetown.edu/annis/scriptorium) and run a query
* In the [Coptic online dictionary](https://corpling.uis.georgetown.edu/coptic-dictionary/), search for a word; click on the ANNIS icon to find instances of that lemma in ANNIS
* When browsing documents at [our portal for reading Coptic texts](http://data.copticscriptorium.org), click on the "Search ANNIS" button to query that corpus.

This tutorial will introduce you to the ways in which our corpora are annotated, how to search the corpora and annotations, and how to download and cite those queries.

## ANNIS Corpus Browser
When you arrive at [https://corpling.uis.georgetown.edu/annis/scriptorium](https://corpling.uis.georgetown.edu/annis/scriptorium), you will see the list of publicly available corpora on the lower left of your screen.  (On the right, you will see a list of sample queries for our corpora -- more on that in a minute.)
<a name="docinfo"></a>Look at the list of corpora:
1.  To find out more information about any corpus, click the "i" information button for that corpus.  A window will appear with:
  * a dropdown menu at the top listing all the documents in a corpus
  * on the left, _metadata_ (information about the corpus, such as annotators, translators, the date this version of the corpus was released)
  * on the right, all the annotations available for texts in this corpus; for a description of what these annotations are, visit our [Annotation Layer Names documentation page](http://wiki.copticscriptorium.org/doku.php?id=annotation_layer_names); if you're in person at the NAPS workshop, we'll also give you a handout.
2.  To see a list of documents in any corpus, click the document icon :page_facing_up: for that corpus name
  * Click the "i" information button for any document for more information
  * You'll also see a list of visualizations for each document (the same visualizations available at [http://data.copticscriptorium.org](http://data.copticscriptorium.org)
  **:arrow_right:Try it:  What happens when you click on a link for a visualization?**
3. You can filter the list of corpora also:
  **:arrow_right:Try it:  What happens when you type in "shenoute." (without the quotation marks) in the Filter box above the list of corpora?**
  **:arrow_right:What happens when you click the :arrows_counterclockwise: button ?**

## Basic Search
Let's start by using the example queries provided for any given corpus.

**:arrow_right:Try it:  Click on the first corpus, apophthegmata.patrum.  Then play around with the sample queries or follow the following steps**
  * In the panel on the right, click on the query to search for the word "ⲁⲡⲁ".  Note:  this searches for the *normalized* word, meaning spelling variants have been normalized, diacritics removed, and missing/damaged letters reconstructed. 
  * In the search results on the right, your query term should appear in red (possibly within a Coptic bound group).
  * See the phrase "Base text" at the top of the list of results?  
    * What happens when you change the base text from "norm_group" to "norm"?  How does this change how the results appear on the screen?
    * What happens when you change the base text to "orig"?  (Note:  orig is an abbreviation for "original text" transcription)
  * You should see the same visualizations we've seen before (Analytic, Diplomatic, Normalized views).  Click on the + next to "analytic view".
    * Can you see your search result in red again?
    * This view visualizes three annotations of the textual data:  [part of speech annotations](http://copticscriptorium.org/download/tools/scriptorium_tagset_documentation.pdf), the normalized Coptic text, and an English translation.
    * Check out the other two visualizations.  What information can you glean from these visualizations of the text?
  * What happens when you click the "i" information icon for the first search result?  What information does this give you?
  * To view ALL the annotations for any given query result, click on "annotations (grid)".
    * All annotations for that stretch of text will appear as layers below.
    * What do you think the "orig" annotation layer is?
    * What do you think the "lang" annotation layer is?
    * What do you think the "lemma" annotation layer is?
    
ANNIS uses a multi-layer annotation model, where a base text appears followed by layers of annotations on that base text.  You can have any number of customized annotations.  All our paleographic and manuscript annotations (lacunae, page breaks, column breaks) follow a set of annotation and encoding standards known as the TEI-XML (the Text Encoding Initiative standards for extensible markup language).  Specifically, we use the [Epidoc subset of TEI XML](http://epidoc.sourceforge.net/), the same encoding standards that Papyri.info uses.

**:arrow_right:Try it:  Let's create your own simple searches for words.**
  * Modify the search we just did by typing your own favorite Coptic word where "ⲁⲡⲁ" appears.  Click "Search".  Check out the results.
  * Don't have a Coptic font installed on your computer?  Click on the little keyboard to the right of the search pane!
  * Let's now search for your favorite word in more than one corpus.  Control-click on a Mac/right-click on a PC on another corpus name in the corpus list in the lower left.  Click Search.

**:arrow_right:Try it:  Create simple queries for information other than words.**
  * Search for norm="ⲥⲟⲛ" in your chosen corpora
  * Now search for lemma="ⲥⲟⲛ".  What's the difference in the results?
  * Search for all Greek words in Shenoute's "I See Your Eagerness":  click on [shenoute.eagerness corpus and search for lang="Greek"](https://corpling.uis.georgetown.edu/annis/scriptorium#_q=bGFuZz0iR3JlZWsi&_c=c2hlbm91dGUuZWFnZXJuZXNz&cl=5&cr=5&s=0&l=10&_seg=bm9ybV9ncm91cA)
  * Search for all words with the morpheme "ⲙⲛⲧ" in Shenoute's "Not Because a Fox Barks": click on [shenoute.fox and search for morph="ⲙⲛⲧ"](https://corpling.uis.georgetown.edu/annis/scriptorium#_q=bW9ycGg9IuKymeKym-KypyI&_c=c2hlbm91dGUuZm94&cl=5&cr=5&s=0&l=10&_seg=bm9ybV9ncm91cA)
  * Search for all proper names in Warren Wells' Sahidica edition of the Gospel of Mark: click on [sahidica.mark and search for pos="NPROP"](https://corpling.uis.georgetown.edu/annis/scriptorium#_q=cG9zPSJOUFJPUCI&_c=c2FoaWRpY2EubWFyaw&cl=5&cr=5&s=0&l=10&_seg=bm9ybV9ncm91cA)
  * Play around with some simple searches.
  
**:arrow_right:Try it:  You can click on the History button to see all the previous queries you've run in your current ANNIS session.**

## Complex Searches 

You can also use [regular expressions](http://ryanstutorials.net/regular-expressions-tutorial/) and the Annis Query Language to create complex queries, searches for sequences of characters, queries for two or more annotations, etc.

**:arrow_right:Try it: Select a corpus, like 1 Corinthians, and try the following queries.  (Type or cut-and-paste.) What kind of results do you get?**
  * norm_group=/ⲡⲉⲧ.*/ 
  * norm=/.*ⲟⲥ/ 
  * norm=/ⲥ[ⲟⲱ]ⲧⲙ/ 

Hint:  the .* in the query syntax signals that you want to search for any character(s).

You can also search within a translation, if your corpus has a translation.  (Not all do.)

**:arrow_right:Try it:  Select the 1 Corinthian corpus. Try the following queries.  What's the difference?**
  ```
  translation=/.*brother.*/
  translation=/.*[Bb]rother.*/
```

You can search more than one field at the same time.  

**:arrow_right:Try it: Say you're interested in proper names. Select the corpus for Abraham Our Father. Compare the following queries**
  * `pos="NPROP" _o_ lang="Greek"`
  * `pos="NPROP" _o_ lang="Hebrew"`
  * `pos="NPROP" _o_ lang=/.*/`

Note:  We tag loan words for language of origin based on the oldest possible language.  To find all loan words, use the lang=/.*/ query.  

You can also add metadata to your queries.

**:arrow_right:Try it: Select the Abraham Our Father corpus.  Search for all the appearances of "ϣⲉⲉⲣⲉ" in the codex MONB.YA:  norm="ϣⲉⲉⲣⲉ" & meta::msName="MONB.YA"**
  * Play around with other metadata fields.  To find all words in documents edited by Rebecca S. Krawiec, select your corpora and search: 
```  
norm & meta::annotation=/.*Krawiec.*/
```

There's lots of fun stuff you can do with regular expressions:
  * Find either circumstantial converters or focalizing converters: pos=/CCIRC|CFOC/
  * Find either form of the same verb: norm=/ⲥ[ⲟⲱ]ⲧⲙ/ 
  * Query for things following each other: To search for a copular pron sentence (a copula following a pronoun):  pos="PPERI" . pos="COP" 
  * Query for nearness:  To find "daughter" within 50 tokens after "son": norm="ϣⲏⲣⲉ" ^* norm="ϣⲉⲉⲣⲉ"

*Know your corpus and annotations when doing research.  For example, in our corpus, a compound word containing both Greek and Coptic contains a language tag only for the Greek morph within the compound. (E.g., in ⲣⲭⲣⲉⲓⲁ, only ⲭⲣⲉⲓⲁ receives the Greek tag. Hence, we use syntax for finding overlapping search fields ("o") rather than equivalent fields ("="). `lang="Greek" _=_ pos="V"` ([link](https://corpling.uis.georgetown.edu/annis/?id=dc1b4bdf-6d0e-407e-9c27-80265da4f58a))
finds all verbs that are Greek loanwords; `lang="Greek" _o_ pos="V"` ([link](https://corpling.uis.georgetown.edu/annis/?id=b40a6020-3be6-4f25-bb38-97d64ce6ac79)) finds all verbs that are Greek loanwords or are compound words with Greek loan words as part of the compound.  Compare the results in the links.* 

## Word Frequencies
ANNIS allows you to find word frequency lists for our corpora.

**:arrow_right:Try it: Select the shenoute.eagerness corpus.**
  * type in the following query to find all the words in the corpus:  norm
  * Below the query window, you should see a button for "More."  Click on it and select "Frequency Analysis."  Click "Perform Frequency Analysis"
  * Both a chart and a list of word frequencies will appear.
  * You can see your frequencies on a [linear scale or a log scale](http://www.fool.com/foolfaq/foolfaqcharts.htm)

**:arrow_right:Try it: Download your frequency list by clicking the "Download as CSV" button**

You can also produce frequencies for more refined lists. **_Be sure to close the "Frequency Analysis" pane to clear your data before you start a new analysis._**

**:arrow_right:Try it: Create lists for loan words in our corpus.**

  **Remember: If you have just run a frequency analysis, then close the current "Frequency Analysis" pane first.  Do this (or click "new analysis") between each new frequency analysis.**
  
  1. Find the Greek loan words in the shenoute.eagerness corpus using this query: `lang="Greek" _o_ norm`
    * Enter the query.  (If you've closed the Frequency Analysis pane, click "More" then "Frequency Analysis")
    * Delete all rows EXCEPT "norm" (since you want the frequency of each normalized word)
    * Click "Perform Frequency Analysis"
  2. Can you do the same to find _all_ loan words in the shenoute.eagerness corpus (remember to hit "new analysis" first): `lang=/.*/ _o_ norm`
  3. Can you do the same to find all loan words that are _verbs_ (remember to hit "new analysis" first): `lang=/.*/ _o_ norm _o_ pos="V"`
  
**BONUS question:  What do you do about corpora that contain more than one manuscript witness to the same text?**  I See Your Eagerness is one such corpus.  In some places, we have parallel manuscript witnesses to the same text.  So if you run a straight word frequency list, you'll get duplicate "hits".  For this corpus (and future versions of other corpora) we encode parallel witnesses in the metadata fields.  When you [click on the "i" information button](#docinfo) for a document, you'll see metadata fields for "witness" and "redundant".

  ![Image of metadata-witness](https://https://github.com/CopticScriptorium/NAPS2017/images/metadata-witness.png)

**:arrow_right:Try it: Run a freqency analysis using the following query: `lang=/.*/ _o_ norm _o_ pos="V" & meta::redundant="no"`**
  * Remember to click "new analysis" to clear your old frequency data first!
  * Remember to delete rows for everything except norm when you run the analysis.
  * Are the results _different_ from the results from #3 above?

_Again:  know your corpus so you understand the numbers.  Spend some time looking at the metadata, understanding the annotation layers, and running queries to see how the annotations and textual data work._

## Download Your Results

## Cite and Link to Your Query





