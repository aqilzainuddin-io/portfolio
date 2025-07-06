### Front End Testing
1. https://automationexercise.com/
2. https://todomvc.com/

### Back End Testing
1. https://reqres.in/
2. https://jsonplaceholder.typicode.com/
3. https://openweathermap.org/appid
4. https://docs.github.com/en/rest?apiVersion=2022-11-28

> Not all web services or platforms provide direct support for Python, but the good news is that Python can interact with nearly all web platforms through available libraries and APIs. Here’s a breakdown of how you can use Python to automate testing for different types of websites:


### **1. UI Testing on Websites (e.g., Selenium, Playwright)**
> For **UI Testing**, the website itself doesn’t necessarily need to "support" Python directly. Python can interact with most websites as long as they are accessible through a web browser, because:

> - **Selenium** and **Playwright** (Python bindings) allow you to automate interactions with websites through browser automation. These tools simulate user actions (e.g., clicking buttons, typing into fields) and verify website behavior.

> - **Selenium:** You control a browser (Chrome, Firefox, etc.) through Python, which allows testing on most websites regardless of backend technologies. It's a general-purpose tool for web automation.

> - **Playwright:** Similarly, Playwright allows interaction with Chromium, Firefox, and WebKit browsers in Python, supporting modern web apps with JavaScript-heavy content, which might be tricky for Selenium to handle efficiently.


> ### **2. API Testing (Backend Testing) on Websites**
> For **API Testing**, the website must expose **API endpoints** for Python to interact with. Many websites and services provide APIs for integration, which you can access using the following Python libraries:
 
> - **Requests:** This is a powerful and popular library for sending HTTP requests (GET, POST, PUT, DELETE, etc.) to interact with RESTful APIs.

> - **Postman/Newman:** While Postman is used for manual API testing, it also provides an option to automate collections and export them for use in other tools, including Python.

> - **Pytest + Requests:** This combo is often used for automated backend testing. You write test cases using Pytest, and use `requests` to interact with the APIs.
 
> Some websites (like **ReqRes** and **JSONPlaceholder**) specifically offer APIs for public use and testing. However, most other real-world sites will require you to have an API key or authentication token to interact with their APIs.


> ### **3. Websites Offering Open APIs for Testing** 
> While not every website provides an API by default, here are a few **public APIs** that you can use for testing:

> 1. **JSONPlaceholder** – A free fake API for testing and prototyping.
> 2. [**ReqRes**](https://reqres.in/) – A mock API service for testing CRUD operations and user authentication.
> 3. **OpenWeatherMap** – Provides APIs for weather data (requires API key).
> 4. [**GitHub API**](https://developer.github.com/v3/) – Allows you to test interactions with GitHub's services (e.g., repositories, issues, and pull requests).


> ### **How Python Interacts with Websites Without Direct Support for Python:** 
> Even if a website doesn’t directly “support” Python (since most websites don't need to), you can still automate interactions with the site by leveraging standard web technologies like HTTP, HTML, CSS, and JavaScript.

> 1. **UI Automation:** Python interacts with the frontend by controlling the browser (with **Selenium** or **Playwright**). It doesn't matter what language the website is built with; as long as it is a web app, Python can automate the interaction.

> 2. **Backend/API Automation:** Many websites (whether built with Java, Python, PHP, etc.) expose **REST APIs**. Python can communicate with these APIs using libraries like **requests**, **Pytest**, or **Postman** (for testing APIs). Websites don’t need to support Python specifically; they just need to have publicly accessible API endpoints.


> ### **Conclusion:** 
> - **UI testing (e.g., with Selenium or Playwright)**: Websites don’t need Python support directly. Python can control a browser and interact with any website.
> - **Backend/API testing**: Websites just need to provide accessible APIs (often through RESTful endpoints). Python can easily interact with these APIs using libraries like `requests` or `pytest`.

> If you're using **public APIs** (like those offered by ReqRes, JSONPlaceholder, or OpenWeatherMap), you’re good to go without any extra requirements. For **real-world applications**, most websites will have an API or a way to interact with the backend (but you might need credentials or API keys).

> Would you like me to help with setting up your testing scripts for a specific website or API? Let me know if you'd like further clarification on any of this!
