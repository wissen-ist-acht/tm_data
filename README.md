# tm data

This repository contains the data used to perform topic modeling on premodern texts; the article that discusses the application and the outcomes can be found here: [LINK WILL BE INSERTED SOON]

There are two folders:
* textual data
* topics explorer 

The folder "textual data" contains the txt-files and the stopword list. 
The txt-files were produced in two different ways: 
For the medieval manuscripts as well as for the two editions of the [chronicle of Jakob Twinger](https://de.wikisource.org/wiki/Die_Chroniken_der_deutschen_St%C3%A4dte#Die_Chroniken_der_oberrheinischen_St%C3%A4dte._Stra%C3%9Fburg) as well as of the [Oberrheinische Chronik](http://dl.ub.uni-freiburg.de/diglit/grieshaber1850a/0017/image?sid=f39b41f27183a69038021538897f5344#current_page), the software [Transkribus](https://readcoop.eu/transkribus/?sc=Transkribus) was used for automatic text recognition. The resulting output was minimally cleaned: During text recognition, words with diacritics were often split into separate strings, e.g. "brů" and "der", so a dissolution of the diacritics was performed, resulting in one string, e.g. "bruoder". Abbreviations were dissolved, e.g. "andˀ" to "ander". Also, information about the digitizing institution that in some cases is shown on the digital copies and therefore recognised as text was deleted completely.  
  
Four different HTR models were used for text recognition:  
[Dresden, UB, Mscr. F 98](https://handschriftencensus.de/18800): Medieval_Scripts_M2 (model ID 35164)  
[Freiburg, UB, Hs. 471](https://handschriftencensus.de/13868): Charter Scripts XIII-XV_M4 (model ID 6091753)  
[Heidelberg, UB, Cpg 116](https://handschriftencensus.de/10347): German_Kurrent_XVI-XVIII_M1 (model ID 19584)  
[Heidelberg, UB, Cpg 475](https://handschriftencensus.de/10406): Thun Missiven M3 (model ID 431)  
[München, BSB, Cgm 568](https://handschriftencensus.de/6173): Charter Scripts XIII-XV_M4 (model ID 6091753)  
[Stuttgart, LB, HB V 22](https://handschriftencensus.de/5897): Thun Missiven M3 (model ID 431)  
[Wolfenbüttel, HAB, Cod. 16.17.](https://handschriftencensus.de/6669): Charter Scripts XIII-XV_M4 (model ID 6091753)  
  
For the edition of the [chronicle of Ulrich Richental](https://edition.mgh.de/001/html/edition.html), the text of the Aulendorfer version was used. The text of the edited [chronicle of Petermann Etterlin](https://www.e-helvetica.nb.admin.ch/view/nbdig-59267!urn%3Anbn%3Ach%3Anbdig-59267%3Anbdig-59267_11.pdf?q=&v=all&urn=nbdig-59267&waybackMode=page&start=0&rows=20&sort=score%20desc%2C%20ehs_urn_id%20asc) could be reused. For the edition of ["Das Leben des Heiligen Ulrich"](https://doi.org/10.1515/9783110816815), I also could reuse already existing full text; unfortunately, the edition is not openly accessible, so I cannot provide the text here.  
The stopword list is an enhanced list of the [Middle High German stopword list](https://docs.cltk.org/en/latest/languages.html#middle-high-german) of the [Classical Language Toolkit](http://cltk.org/).

The folder "topics explorer" contains the output of the topic modeling performed with the software [Dariah Topics Explorer](https://dariah-de.github.io/TopicsExplorer/). The output consists of several csv-files that can be used for visualisations.  
If you want to run the analysis yourself, there is one caveat: Development and maintenance of the Topics Explorer might not be up to date in case of recent updates of your operating system; it should always work if you download the source code and run the programme in a virtual environment. If it does not, you still can try your luck with the provided [notebooks](https://github.com/DARIAH-DE/Topics/tree/master/notebooks). Having a look at the [Topics Explorer issues](https://github.com/DARIAH-DE/TopicsExplorer/issues) or opening a new one might lead to a quick solution.
