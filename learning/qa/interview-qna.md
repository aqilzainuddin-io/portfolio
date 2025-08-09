**1. How to create tests in Postman?**
- In Postman, after you send a request, go to the Tests tab. You can write small JavaScript snippets using pm.test() to check things like status codes, response time, or response body. Example:

javascript
pm.test("Status code is 200", () => {
    pm.response.to.have.status(200);
});
*This will pass if the response status is 200 OK.*

**2. What is API schema validation?**
- Schema validation checks if the API response matches the expected data structure — types, fields, etc. It’s like checking if the response “shape” is correct, not just the values.
Example in Postman:

javascript
pm.test("Schema is valid", () => {
    pm.response.to.have.jsonSchema(schema);
});
*Useful to make sure the API doesn’t break when developers change something.*

**3. What are the different API methods?**
- GET → Retrieve data
- POST → Create new data
- PUT → Update entire data
- PATCH → Update part of the data
- DELETE → Remove data

**4. What’s the difference between 400 series and 500 series responses?**
- 400 series → Client errors (wrong request, missing data, unauthorized, not found)
- 500 series → Server errors (problem in the server code, crash, internal bug)
*Think of it like: 400 = you messed up the request, 500 = server messed up processing it.*

**5. What is a framework in QA automation?**
- A framework is a structured way to organize your test code and tools so tests are reusable, maintainable, and easy to run.
Example: In Postman + Newman, your framework is the collection, environment, and report generator working together.

**6. Why use automation for API testing?**
- Faster than manual testing
- Runs 24/7 on CI/CD pipelines
- Less human error
- Easy to repeat across environments

**7. What is Postman used for?**
- Postman is a tool for sending API requests, checking responses, writing automated tests, and generating reports. It makes API testing easier without needing to code everything from scratch.