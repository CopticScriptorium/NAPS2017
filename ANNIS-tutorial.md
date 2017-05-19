# ANNIS Tutorial
## Introduction to ANNIS
Coptic Scriptorium uses the [ANNIS](http://corpus-tools.org/annis/) search and visualization tool. You can access Coptic Scriptorium's corpora in ANNIS in multiple ways:
* Go directly to [https://corpling.uis.georgetown.edu/annis/scriptorium](https://corpling.uis.georgetown.edu/annis/scriptorium) and run a query
* In the [Coptic online dictionary](https://corpling.uis.georgetown.edu/coptic-dictionary/), search for a word; click on the ANNIS icon to find instances of that lemma in ANNIS
* When browsing documents at [our portal for reading Coptic texts](http://data.copticscriptorium.org), click on the "Search ANNIS" button to search that corpus
This tutorial will introduce you to the ways in which our corpora are annotated, how to search the corpora and annotations, and how to download and cite those queries.

##ANNIS Corpus Browser
When you arrive at [https://corpling.uis.georgetown.edu/annis/scriptorium](https://corpling.uis.georgetown.edu/annis/scriptorium), you will see the list of publicly available corpora on the lower left of your screen.  (On the right, you will see a list of sample queries for our corpora -- more on that in a minute.)
Look at the list of corpora:
1.  To find out more information about any corpus, click the "i" information button for that corpus.  A window will appear with:
  * a dropdown menu at the top listing all the documents in a corpus
  * on the left, _metadata_ (information about the corpus, such as annotators, translators, the date this version of the corpus was released)
  * on the right, all the annotations available for texts in this corpus; for a description of what these annotations are, visit our [Annotation Layer Names documentation page](http://wiki.copticscriptorium.org/doku.php?id=annotation_layer_names); if you're in person at the NAPS workshop, we'll also give you a handout.
2.  To see a list of documents in any corpus, click the document icon (it looks like a page) for that corpus name
  * Click the "i" information button for any document for more information
  * You'll also see a list of visualizations for each document (the same visualizations available at [http://data.copticscriptorium.org](http://data.copticscriptorium.org)
  **Try it:  What happens when you click on a link for a visualization?**
3. You can filter the list of corpora also:
  **Try it:  What happens when you type in "shenoute." (without the quotation marks) in the Filter box above the list of corpora?**
  **What happens when you click the button with the circular arrows?**

##Basic Search
Let's start by using the example queries provided for any given corpus.

**Try it:  Click on the first corpus, apophthegmata.patrum.**
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

**Try it:  Let's create your own simple searches for words.
