# DL_for_searching_Russian_Records
This repo is dedicated to building a deep learning system under development that can identify and search through Russian Birth/Marriage/Death records for names of individuals and other translational purposes.

<b>Vision and Background </b>

The vision of this project is to use deep learning and computer vision methods to create a workflow that allows English speakers to search more easily through Russian family history records to find names more easily. After digging through many of these records, it has been difficult for me personally to distiguish handwritten characters, going back and forth between handwritten character guides and spending a lot of time searching through record documents.  I felt like there was a better way to do this more efficiently and quickly to search through more records.

Here is a basic example of some typical Birth/Marriage/Death records along with example title pages and indices that are sometimes included:

[insert pictures here]

<b>Methods</b>

Depending on the records, since there are a vast number, a bounding box table structure is used to separate (generally) any data recorded, and printed text is often used for the titles.  Detecting table regions and title text is an easier first step which can lead to further separation of data for detection of handwritten information.  

Currently (July 2020) detecting handwritten text is a difficult problem still currently being solved in the computer vision/deep learning community, but I still believe that individual characters could still be found using current methods in handwritten text.  I'm trying to start from searching for names using the first (typically capital) letter of the surname based on its placement in the appropriate box (or somewhat near it).

<b>The smaller incremental goals associated with this vision are as follows (in no particular order, although some depend on others): </b>
<ul>
<li> Detecting different regions according to bounding boxes </li>
<li> Using OCR to convert printed title text into Russian words, then into english phrases (direct translations, and adjusted translations) </li>
<li> Detecting Russian handwritten letters (capital vs lowercase) </li>
<li> Using Deep learning to classify between Birth, Marriage, Death, Title, and index pages (or regions) </li>
<li> Detecting words from regions that exit boxes </li>
<li> Detecting Russian handwritten Capital letters inside of a box (from a search, either name or attending, etc.) </li>
<li> Separating different regions of birth/Marriage/Death/title/index parts of pages for analysis? </li>
<li> Building an online javascript system to run this system so that it can be integrated with FamilySearch sites </li>
</ul>

<b>Future work/ideas that may be particularly difficult/time consuming:</b>
<ul>
<li> Handwritten word detection in Russian </li>
<li> Text translation overlay from handwritten text (dependent on above) </li>
<li> Extensions to other languages (other language speakers to search Russian documents, English users to search other language documents) </li>
<li> Using Russian name prediction software (see other Russian family history sites [insert link here]) to generate Russian version of english/polish/other names and then search for it in documentation </li>
</ul>

<b> File Organization </b>
We are currently organizing files by each of the above listed subproject goals, and will create projects that combine many of them in the future.

<b> Running individual projects </b>
See individual .readme files for each project to see how to run them independently.
