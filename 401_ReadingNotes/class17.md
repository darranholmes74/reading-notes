# Class 17 Reading Assignment

1. The key difference between scraping static and dynamic websites is that static websites have all their content loaded into the initial HTML source code, while dynamic websites require additional steps to scrape data since their content may be loaded dynamically using JavaScript.

2. Limit your requests: Sending too many requests to a website in a short period of time can trigger their anti-scraping measures and get you blocked.


Use proxies and rotate user agents: Using the same IP address and user agent for all your requests can make you easily identifiable and get you blocked. 

Follow good scraping etiquette: It's important to be a good web scraping citizen and follow best practices.

3. Playwright is an open-source Node.js library for automating web browsers, including Chromium, Firefox, and WebKit. It provides a high-level API for controlling the browser and allows you to interact with web pages, emulate user interactions, and extract data from web pages.

An example use case where Playwright would be particularly beneficial is scraping data from a website that requires authentication. Many websites require users to log in to access certain pages or data. With Playwright, you can automate the login process, navigate to the pages you need to scrape, and extract the desired data.

4. Xpath is a query language used for selecting elements from an XML or HTML document. 

For example, suppose we want to select the title of a webpage, which is enclosed in an HTML title tag. We can use the following Xpath expression to select the title element:

//title

The double forward slash (//) selects all title elements in the document, regardless of their location within the HTML tree.


### Things I want to know more about