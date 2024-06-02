# Web Content Analysis
### Author: Anuroop Arya 
**Introduction:**

This project aims to analyze web content from given URLs to extract insights such as sentiment analysis, complexity metrics, and word counts. By leveraging various Python libraries and techniques, the script fetches article content from URLs, processes the text, and computes relevant metrics. 

**Approach:**

1. **URL Extraction:** URLs are extracted from an Excel file named "Input.xlsx".
2. **Web Scraping:** Using the requests library, the script fetches article content from the provided URLs.
3. **Text Processing:** The fetched text is cleaned, tokenized, and processed to remove stopwords.
4. **Metric Computation:** Various metrics like total word count, percentage of complex words, sentiment scores, etc., are computed.
5. **Output Generation:** The computed metrics are structured into a DataFrame and exported to an Excel file named "Output Data Structure.xlsx".

**Technologies Used:**

- **Python:** The primary programming language used for scripting.
- **Libraries:**
  - **pandas:** For data manipulation and DataFrame creation.
  - **numpy:** For numerical computations.
  - **nltk:** For text tokenization and sentence splitting.
  - **requests:** For making HTTP requests and fetching web content.
  - **beautifulsoup4:** For parsing HTML content during web scraping.
  - **fake_useragent:** For generating fake user agents to avoid detection during web scraping.

**Methodology:**

The script follows a structured approach:
- It begins by extracting URLs from the provided Excel file.
- Then, it fetches article content from each URL using web scraping techniques.
- Next, it processes the text to compute various metrics such as sentiment scores, word counts, and complexity metrics.
- Finally, it structures the computed metrics into a DataFrame and exports it to an Excel file.

**Real-World Applications:**

- **Content Analysis:** This script can be used by content analysts to analyze the sentiment and complexity of articles or blog posts.
- **SEO Optimization:** SEO professionals can utilize the insights generated to optimize content for better search engine rankings.
- **Market Research:** Researchers can analyze web content to understand public opinion or market trends.

**Instructions to Run Your Script:**

**Dependencies:**

This script requires the following Python libraries to be installed:
- pandas
- numpy
- nltk
- requests
- beautifulsoup4
- fake_useragent

You can install these dependencies using pip: 
```
$ pip install pandas numpy nltk requests beautifulsoup4 fake_useragent
```

**Running the Script:**
1. **Ensure you have an active internet connection.**
2. **Modify Input:** Place your "Input.xlsx" file containing the URLs in the same directory as this script.
3. **Execute the Script:** Run the Python script named 'Assignment.py' using Python3.

**Output:**

The script will generate an Excel file named 'Output Data Structure.xlsx' in the same directory.

**Notes:**

- The script fetches article content from URLs provided in Input.xlsx.
- The output file will contain the computed variables as specified in 'Output Data Structure.xlsx'.
- Make sure 'Input.xlsx' is correctly formatted with URLs in the expected column.
- Ensure that all files (StopWords_Generic.txt, positive-words.txt, negative-words.txt, Input.xlsx, and the script itself) are in the same directory because the script uses direct file names instead of paths.
