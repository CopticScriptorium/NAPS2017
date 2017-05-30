# Digitize and Annotate a Text Using Coptic Scriptorium's GitDox Tool and Natural Language Processing Tools

In this tutorial, you will learn how to digitize and annotate a short Coptic text using our GitDox tool and NLP tools.  For participants in the NAPS workshop, we will provide a text and all the other necessary materials.  Check with the facilitators.  In groups of 2-4 people, you will transcribe a text and provide basic paleographic/manuscript encoding.


For more detailed documentation, visit our [wiki](http://wiki.copticscriptorium.org/doku.php?id=gitdox_workflow); some of this tutorial is taken from that documentation.

If you want to digitize a specific text for inclusion in the Coptic Scriptorium corpora and database, we would like to collaborate with you. Please contact us!

## Login and Orientation to GitDox

GitDox is an online XML and spreadsheet editor which uses [GitHub](github.com/CopticScriptorium/) for data storage and versioning. Coptic Scriptorium currently uses GitDox to transcribe texts and edit them in a spreadsheet.Although you don't need to have a GitHub account to use GitDox, it's helpful.  For the purposes of the NAPS workshop, you don't need one.  If you want to collaborate with us or use GitDox in the future, you can get an account later.

GitDox is located at https://corpling.uis.georgetown.edu/gitdox/ .  Navigate there on your computer, and login using the username and password we provided you at the workshop.

When you log in to GitDox, you see a list of current documents. Use the dropdown menu above the list to display only documents from a certain corpus. You can also use the arrows to the right of each column name to sort by that column.

Documents are assigned to users (as noted in the fifth column). Please only edit documents assigned to you. If you believe a document should be assigned to you but isn't, please contact the person to whom it is currently assigned to confirm that you should be assigned the document before editing it.

Find the text we assigned to you in the workshop.  Click on the "Edit" button for your text.  Assign it to yourself.

## Saving and Committing

The transcription mode of GitDox has two options for saving work: save and commit. The save button saves changes within GitDox but does not commit those changes to GitHub. Your permission levels will not allow you to commit to GitHub; one of the workshop facilitators will complete this step of the process. Because GitDox depends on an internet connection, it's a good idea to save your work frequently while you're working using the save button.

## Adding metadata

Use the button at the bottom of the page to add metadata. We've added some of the important metadata for th etutorial.  You will need to add your own names.  Click the metadata button.  Enter "annotation" in the first window and your group's names separated by commas in the second (e.g., Caroline T. Schroeder, Rebecca S. Krawiec).  After you click submit, the metadata will appear in a chart on the bottom of the page. You can't edit metadata you've already submitted, but you can delete the entry from the list and re-enter the correct field and information.

## Transcribing


Now begin typing in your text.  Use a utf-8 (Unicode) characterset, such as the Antinoou font and keyboard.  Transcribe as you would any manuscript.  Use regular returns to create line breaks

You'll notice two "tags" already in your otherwise empty document.  These are XML tags for annotating text.  If you want to annotate something in your text, you'll wrap the relevant text in "tags".  The first tag (the open tag) is in brackets, such as `<TEI>`; the close tage has brackets and a slash, such as `</TEI>` (If you want, you can read more about [TEI XML](http://www.tei-c.org/index.xml) and the [Epidoc](https://sourceforge.net/p/epidoc/wiki/Home/) subset of XML.)

Start your transcription _inside_ the TEI tags.

You will want to encode for information about pages and columns.  
  * `<pb></pb>` The page break tags will wrap around all the text in a given page.  We use what's called an attribute to encode the page number of the manuscript.
  *  `<cb></cb>` Column break tags will wrap around all the text in a given column.

When you open an angle bracket, GitDox suggests tags that are currently available. GitDox will also suggest attributes for tags. Improperly closed tags and other errors are highlighted in red.

If you need to provide other information, such as if a letter in the manuscript is large or ekthetic (hangs out in the margin), see the cheatsheet provided in the workshop or our longer [Transcription Guidelines](https://github.com/CopticScriptorium/tagger-part-of-speech/blob/master/scriptorium-transcription-guidelines.pdf) for instructions.

Below, see a sample text encoded as an example:

![screenshot of sample text](https://github.com/CopticScriptorium/NAPS2017/raw/master/images/sample-text.png)

Either while you are typing or after you are done transcribing, separate Coptic bound groups with a space or underscore.  For example:

ⲁϥⲥⲱⲧⲙ̄ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ ⇒ ⲁϥⲥⲱⲧⲙ̄_ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_

Be sure to separate the punctuation, as well.  

ⲁϥⲥⲱⲧⲙ̄ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ· ⇒ ⲁϥⲥⲱⲧⲙ̄_ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_·_

Put a separator between all bound groups, even if a bound group ends at the end of a line:

ⲁϥⲥⲱⲧⲙ̄     ⲁϥⲥⲱⲧⲙ̄_
ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ ⇒  ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_·_

If you need to provide other information, such as if a letter in the manuscript is large or ekthetic (hangs out in the margin), see the cheatsheet provided in the workshop or our longer [Transcription Guidelines](https://github.com/CopticScriptorium/tagger-part-of-speech/blob/master/scriptorium-transcription-guidelines.pdf) for instructions.

When you are done typing in your text, be sure to SAVE.

## Tokenizing

Our natural language processing tools will automatically divide bound groups into words.  This process is called tokenization.  Click the NLP button under the transcription box to automatically tokenize your transcribed text. Correct the tokenization in GitDox by adding pipes between the words.

## Processing using the NLP

We expect an automated link between the XML editor, the NLP, and an online spreadsheet editor to be available in summer 2017. However, as of May 2017, the following steps are necessary to move transcribed texts from the XML editor through the natural language processing tools.

After checking tokenization and saving the final text, copy the text from GitDox and paste it into the online NLP pipeline at https://corpling.uis.georgetown.edu/coptic-nlp/. Make sure you select “from pipes in input” under tokenize.
Process the text, copy the resulting SGML, and paste it into a new file (you may use a text editor such as text wrangler or notepad) on your computer. Save the file on your computer.

In your file on GitDox, use the mode drop-down menu to change to the spreadsheet mode. A blank spreadsheet should appear.
Scroll to the bottom of the page and use the upload function to upload the file you saved on your computer. The spreadsheet should be populated with the information from your file.

## Editing the annotations

You should now see annotations in layers, very similar to the grid annotations we saw in the ANNIS database.  

Check the annotations! You probably don't know all our [part of speech abbreviations](http://copticscriptorium.org/download/tools/scriptorium_tagset_documentation.pdf), but you can tell if the NLP tools caught all the loan words, or if they expanded nomina sacra in the normalized layers.


