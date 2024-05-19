### Approach:

1. **Importing Libraries and Setup**:
   - Libraries like `numpy`, `re`, `os`, `pandas`, `nltk`, `urllib`, `BeautifulSoup`, `fake_useragent`, and `requests` are imported to handle data, text processing, web scraping, and HTTP requests.

2. **File Paths and Input Reading**:
   - File paths for stopwords and word lists are defined.
   - Input URLs are read from an Excel file (`Input.xlsx`).

3. **Fetching Article Data**:
   - Functions are defined to fetch article titles and content from URLs using `requests` and `BeautifulSoup`.

4. **Text Processing**:
   - The text is tokenized and stopwords are removed using `nltk.tokenize.RegexpTokenizer`.
   - Positive and negative word counts are calculated using predefined word lists.

5. **Calculating Metrics**:
   - Various metrics such as total word count, average sentence length, complex word count, percentage of complex words, and polarity score are computed.

6. **Data Handling**:
   - Results are organized into a `pandas` DataFrame (`df`) containing article titles and computed metrics.

7. **Saving Output**:
   - The final DataFrame is saved as an Excel file (`Output Data Structure.xlsx`), with the 'corps' column dropped to clean up the data structure.

This approach ensures that article data is fetched, processed, and analyzed efficiently, with results stored in a structured format. 



###Instructions to Run Your Script:

1. Dependencies:
   - This script requires the following Python libraries to be installed:
     - pandas
     - numpy
     - nltk
     - requests
     - beautifulsoup4
     - fake_useragent

   You can install these dependencies using pip:
   $ pip install pandas numpy nltk requests beautifulsoup4 fake_useragent

2. Running the Script:Ensure you have an active internet connection.
   -Modify Input:Place your Input.xlsx file containing the URLs in the same directory as this script.
   -Execute the Script: Run the Python script named 'Assignment.py' using Python3:

3. Output:
   - The script will generate an Excel file named 'Output Data Structure.xlsx' in the same directory.

4. Notes:
   - The script fetches article content from URLs provided in Input.xlsx.
   - The output file will contain the computed variables as specified in 'Output Data Structure.xlsx'.
   - Make sure 'Input.xlsx' is correctly formatted with URLs in the expected column.
   - Ensure that all files (StopWords_Generic.txt, positive-words.txt, negative-words.txt, Input.xlsx, and the script itself) are in the same directory because the script uses direct file names instead of paths.



