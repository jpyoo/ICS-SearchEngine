# Web Crawler for ICS School Pages

121 Search Engine
Kevin Pradjinata, Kashyup Patel, Megan Le, Jay Yoo

## Overview

This project involves the development of a web crawler focused on ICS (Information and Computer Sciences) school webpages. The primary goal is to achieve a remarkable response time of less than 300ms for complex search queries containing multiple words. Various techniques, including indexing index files, database connections, Beautiful Soup library, word stemming, tf-idf vectorizers, and cosine similarity, have been employed to optimize the crawler's performance.

## Key Features

- **Fast Response Time:** Achieved less than 300ms response time for complex search queries.
- **Indexing Index File:** Implemented indexing of index files for speed enhancements during searches.![image](https://github.com/jpyoo/ICS-SearchEngine/assets/58375171/7779b61b-b260-4c19-91f1-da336f23144a)

- **Database Connection:** Established a robust connection to a database to store and retrieve relevant information efficiently.
- **Beautiful Soup Library:** Utilized Beautiful Soup for web scraping, extracting data from HTML and XML files.
- **Stemming Words:** Implemented word stemming to improve search relevance and accuracy.
- **Infinite Loop Avoidance:** Employed tf-idf vectorizers and cosine similarity to prevent infinite loops caused by inappropriate crawler behaviors.
  
### Term Frequency (TF)

$\ \text{TF}(t, d) = \frac{\text{Number of times term } t \text{ appears in document } d}{\text{Total number of terms in document } d} \$

### Inverse Document Frequency (IDF)

$\ \text{IDF}(t, D) = \log\left(\frac{\text{Total number of documents in the corpus } N}{\text{Number of documents containing term } t + 1}\right) \$

### TF-IDF Score

$\ \text{TF-IDF}(t, d, D) = \text{TF}(t, d) \times \text{IDF}(t, D) \$

## Examples

### Query: cristina lopes

- [https://www.ics.uci.edu/~hsajnani/](https://www.ics.uci.edu/~hsajnani/): 40ms
- [https://www.ics.uci.edu/~sjavanma/](https://www.ics.uci.edu/~sjavanma/): 19ms
- [https://www.informatics.uci.edu/close-to-the-trenches/#content](https://www.informatics.uci.edu/close-to-the-trenches/#content): 17ms
- [https://www.informatics.uci.edu/close-to-the-trenches/](https://www.informatics.uci.edu/close-to-the-trenches/): 17ms
- [https://www.ics.uci.edu/community/news/features/view_feature?id=67](https://www.ics.uci.edu/community/news/features/view_feature?id=67): 17ms

### Query: machine learning

- [https://cml.ics.uci.edu/category/aiml/page/2/](https://cml.ics.uci.edu/category/aiml/page/2/): 234ms
- [https://cml.ics.uci.edu/category/aiml/page/2/#content](https://cml.ics.uci.edu/category/aiml/page/2/#content): 234ms
- [https://cml.ics.uci.edu/category/aiml/#content](https://cml.ics.uci.edu/category/aiml/#content): 211ms
- [https://cml.ics.uci.edu/category/aiml/](https://cml.ics.uci.edu/category/aiml/): 211ms
- [https://www.ics.uci.edu/~pazzani/Publications/OldPublications.html#1989](https://www.ics.uci.edu/~pazzani/Publications/OldPublications.html#1989): 192ms

### Query: ACM

- [https://www.ics.uci.edu/~eppstein/bibs/eppstein.html](https://www.ics.uci.edu/~eppstein/bibs/eppstein.html): 114ms
- [https://www.ics.uci.edu/~mjcarey/MJCarey_Publications.html](https://www.ics.uci.edu/~mjcarey/MJCarey_Publications.html): 69ms
- [https://www.ics.uci.edu/~gmark/Home_page/Publications.html](https://www.ics.uci.edu/~gmark/Home_page/Publications.html): 59ms
- [https://www.ics.uci.edu/~kobsa/kobsa-publi.htm](https://www.ics.uci.edu/~kobsa/kobsa-publi.htm): 54ms
- [https://www.ics.uci.edu/~gts/pubs.html](https://www.ics.uci.edu/~gts/pubs.html): 54ms

### Query: master of software engineering

- [https://www.ics.uci.edu/~wscacchi/Papers/Vintage/Software_Productivity.html](https://www.ics.uci.edu/~wscacchi/Papers/Vintage/Software_Productivity.html): 437ms
- [https://www.ics.uci.edu/~taylor/Publications.htm](https://www.ics.uci.edu/~taylor/Publications.htm): 282ms
- [https://www.ics.uci.edu/~wscacchi/publications.html](https://www.ics.uci.edu/~wscacchi/publications.html): 270ms
- [https://www.ics.uci.edu/~andre/publications.html](https://www.ics.uci.edu/~andre/publications.html): 266ms
- [https://redmiles.ics.uci.edu/publication/#content](https://redmiles.ics.uci.edu/publication/#content): 264ms

### Web GUI
<img width="815" alt="search_result" src="https://github.com/jpyoo/ICS-SearchEngine/assets/58375171/6d88d716-67b7-4464-9b08-120b65135b23">

## Responsibilities

As a team member, I contributed to various aspects of the project:

1. **Debugging and Testing:** Conducted thorough testing and debugging of individual functions to ensure robust code.
2. **Infrastructure Construction:** Built the project infrastructure, including database connections for seamless data management.
3. **Web GUI using Flask:** Developed a user-friendly web GUI using Flask for easy interaction with the web crawler.
4. **Indexing Index Files:** Implemented indexing of index files to enhance search speed and efficiency.
5. **Infinite Loop Avoidance Functions:** Designed and integrated functions to avoid infinite loops caused by inappropriate crawler behaviors.

## Deployment

The project is ready for deployment. Follow the steps below to deploy:

1. Clone the repository.
2. Install the required dependencies.
3. Set up the database connection.
4. Run the web crawler using the provided commands.

## Usage

To use the web crawler, follow these steps:

```bash
# Clone the repository
git clone https://github.com/your-username/web-crawler.git

# Navigate to the project directory
cd web-crawler

# Install dependencies
pip install -r requirements.txt

# Set up the database connection
# Update configuration files as needed

# Run the web crawler
python main_crawler.py
