# Reading Questions
 ## 1-What are the key differences between scraping static and dynamic websites?
 The difference between static websites and dynamic websites is that static websites appear the same for every user that accesses them
and only change when a developer modifies the source files,whereas dynamic websites can present different information to different visitors.
                                                        
## 2-Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

Respectful Crawling: To avoid overwhelming a website's server and being flagged as a bot, it's crucial to practice respectful crawling. This involves setting a reasonable crawl rate by adding delays between requests and adhering to any rules specified in the website's robots.txt file. By simulating human-like behavior and avoiding excessive requests, you can minimize the risk of being blocked.

User-Agent Rotation: Websites often track user agents to identify automated bots. By rotating the User-Agent header in your requests, you can make your scraping requests appear more like regular user traffic. Using a variety of user agents and occasionally mimicking popular web browsers can help you fly under the radar and avoid detection.

Proxy Rotation: Employing a pool of proxies can help distribute your requests across different IP addresses, making it harder for websites to track and block your scraping activity. By rotating proxies, you can avoid hitting rate limits, prevent IP blocking, and maintain a level of anonymity. It's essential to use reputable proxy providers and ensure that your code is configured correctly to handle proxy rotation seamlessly.

## 3-What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would


 be particularly beneficial.Chromium, Firefox and WebKit with a single API.
Use Case: Scraping data from a Single-Page Application (SPA)

## 4-Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

XPath (XML Path Language) is a powerful query language used in web scraping to navigate and select specific elements within an HTML or XML document. It provides a way to traverse the document's structure and access desired data by using path expressions.
The purpose of using XPath in web scraping is to precisely locate and extract the required information from the webpage. By using XPath expressions, you can target specific elements, such as HTML tags, attributes, or text content, based on their hierarchical relationships within the document.
```
Example: //h1[@class="title"]
In this example, the XPath expression consists of two parts:

//h1: This selects all <h1> elements in the document, regardless of their position or parent elements. The double forward slash (//) indicates that we are searching for <h1> elements anywhere in the document.

[@class="title"]: This is a condition within square brackets that filters the selection based on the class attribute. It selects only those <h1> elements that have a class attribute with the value "title".```