# IndexBuilder_kr_Custom
### "IndexBuilder_kr_Custom" is a search index generator tool designed in Python to help in storing data from a document. It forms forward and inverted index, which facilitate the search by mapping on them where certain terms appear in documents.

## Pre-requisites required:
-> Python 3.x environment
-> NLTK library for text processing (stopwords and stemming)
## Files that are required:
-> stopwordlist.txt: A text file containing additional custom stopwords, with each stopword on a new line.
-> Document files: Files should be named with the prefix ft911_ and contain both <DOCNO> and <TEXT> tags for document ID and content.

## Setup Instructions
-> Custom Stopwords File:
Prepare a stopwordlist.txt file with one stopword per line. This list supplements the standard English stopwords used in the program.

-> Directory of the document:
Place your documents in a designated directory (e.g., ft911).

-> Ensure that every document consists:
--> <DOCNO> tag: Identifies the document ID.
--> <TEXT> tag: Contains the text content to be indexed.

-> Output Files:
Specify paths for output files, forward_index.txt and inverted_index.txt, where indices will be saved.

--> Usage Workflow:
Initialize the Indexer: Set up an instance of IndexBuilder_kr_Custom and load custom stopwords from stopwordlist.txt.
Index Documents: Process the documents in the specified directory to generate indices. The forward index maps document IDs to terms and their frequencies, while the inverted index maps terms to document IDs and term frequencies within each document.
Save Indices: Save the generated indices to output files for future retrieval and searching.
Output Files Description
forward_index.txt: Contains mappings of document IDs to terms found within each document. Each entry includes term frequencies for the document, allowing you to see which terms are most prevalent.
inverted_index.txt: Contains mappings of terms to the documents in which they appear. Each entry includes the frequency of the term within each document, enabling quick lookups for documents containing specific terms.
Example Use Case
After setting up stopwordlist.txt and a directory of documents in ft911, you can execute the indexing process. This will produce forward_index.txt and inverted_index.txt, which can be used to search documents by terms or retrieve term frequencies by document.
