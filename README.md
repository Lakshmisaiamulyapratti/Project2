# Project_Phase - 2:- Construction of Search Engine Index

## IndexBuilder_kr_Custom:
-> "IndexBuilder_kr_Custom" is a search index generator tool designed in Python to help in storing data from a document. It forms forward and inverted index, which facilitate the search by mapping on them where certain terms appear in documents.

## Pre-requisites required:
-> Python 3.x environment
-> NLTK library for text processing (stopwords and stemming)
## Files that are required:
-> stopwordlist.txt: One can create an extra text file with the optionally selected stops words of the actual text where each stop word is separated by a line.
-> Document files: Files should be ft911_ basically their filenames should contain <DOCNO> and <TEXT> tags for document identification and content respectively.

## Setup instructions:
### Custom Stopwords File:
Create a stopwordlist.txt file with one stopword as one line at the file. This list also enriches the standard list of English stop words that are used in the program.

### Directory of the document:
After that, put your documents into the particular directory (for instance, ft911).

-> Ensure that every document consists:
--> <DOCNO> tag: Finds the document ID.
--> <TEXT> tag: Includes the signs and symbols that will be used in the game ,here being the actual text that is to be searched.

### Output files:
The forward_index.txt and the inverted_index.txt files will be created which contain the indices; specify paths for them.

## Usage Workflow:
--> Indexer initialization: Create IndexBuilder_kr_Custom and load stop list data from stopwordlist.txt.
--> Documents of index: Some of the documents in the directory will be used to generate indices as follows. The forward index assigns document numbers to terms and how frequently the terms appear in the documents The inverted index assigns terms to document numbers and how frequently each term occurs in a document.
--> Indices saving: Store the generated indices to output files which might be searched later on.

## Description of output files: 
--> forward_index.txt: Database includes two lists with mappings of document ID to terms identified within each document. In addition, every entry presents the frequency of the terms in the document, so a person understands which terms are more typical.
--> inverted_index.txt: 
These includes mappings of term to the documents in which the terms are used. Each entry includes the frequency of the particular term in each document, allowing for immediate lookups of documents which contain specific terms.

## Usecase for an example:
In order to index the documents, you have to create the file named stopwordlist.txt and the directory, where the documents for the indexing process are stored, and named ft911. This will create forward_index.txt and inverted_index.txt that is used to search for documents by term or applying the term to documents to get the frequency.


### By,
### Name: Reddy Krishna Reddy Yeddula 
### Mail ID: ReddyKrishnaReddyYeddula@my.unt.edu
