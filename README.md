### Domain Analysis Tool 🌐

This Python script analyzes a list of domains for the presence of specific keywords related to free trials and demos.

### Usage Instructions 📝

1. **Dependencies**:
   - Ensure you have Python installed (`>=3.6`).
   - Install required libraries using `pip`:
     ```bash
     pip install pandas requests beautifulsoup4 selenium seaborn matplotlib
     ```

2. **Setup**:
   - Clone this repository.
   - Navigate to the project directory.

3. **Run**:
   - Execute the script:
     ```bash
     python domain_analysis.py
     ```

### Features ✨

- **Web Scraping**: Utilizes `requests` and `BeautifulSoup` for HTTP requests and HTML parsing.
- **Parallel Execution**: Implements `ThreadPoolExecutor` for concurrent task execution.
- **Headless Browser**: Uses `Selenium` with a headless Chrome browser for dynamic page analysis.
- **Data Visualization**: Generates a pie chart visualizing the breakdown of domain records.

### Code Highlights 🚀

```python
# Check keywords using Selenium for non-standard domains
def check_keywords_in_domain_selenium(domain):
    ...

# Check keywords using requests and BeautifulSoup for standard domains
def check_keywords_in_domain(domain):
    ...

# Pie chart to show distribution of records by keywords
plt.figure(figsize=(10, 7))
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=True, startangle=140, wedgeprops=dict(width=0.3))
plt.title("Breakdown of Records by Free Trials and Demos")
plt.show()
```

### Results 📊

The script reads a list of domains from an Excel file, checks each domain's webpage for the presence of "free trial" and "demo" keywords, and generates insights based on the findings.

For further details and analysis, refer to the displayed DataFrame within the Jupyter notebook.

Enjoy exploring and analyzing your domain records! 🚀
