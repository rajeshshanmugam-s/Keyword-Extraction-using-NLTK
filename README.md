# Keyword-Extraction-using-NLTK
Extracting keywords From PDF file using PyPDF2 and NLTK

First of all, I'm a newbee in NLTK. I get this assignment as a selection process for an Internship. 
The Internship was to extract keywords from the PDF file they have given. We see PDFs are a proprietary format by Adobe that comes with their own little quirks when it comes to automating the process of extracting information from each file.

Luckily, we have the right language for the job: Python. Now, I’ve made my love for Python clear: It’s easily human-readable, it has a ton of awesome libraries that allow us to do basically anything. It’s the perfect tool in our utility belt. As I’ve mentioned before, it makes me Batman.

Setup:

We require the following python libraries in order to follow this task:

PyPDF2 (To convert simple, text-based PDF files into text readable by Python)
textract (To convert non-trivial, scanned PDF files into text readable by Python)
nltk (To clean and convert phrases into keywords)

In my experience installing textract is the hard part. 

Steps:
1. Import required libraries
2. Load the PDF file
3. Convert the text into keywords
4. create a new list with punctuations that we want to clear. 
5. We initialize the stopwords variable which is a list of words like "The", "I", "and", etc. that don't hold much value as keywords
6. We create a list comprehension which only returns a list of words #that are NOT IN stop_words and NOT IN punctuations.
