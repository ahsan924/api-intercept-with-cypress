# Mocking the API request with Cypress
Let’s start with an example, our web-browser is our Client which sends a bunch of API requests to a certain backend server during the interaction. What Cypress can do is actually it can intercept some of those calls and provide the mock response to your web browser. With this service provided by Cypress, you can create your own service and provide the response which you actually need for your test.

Why is it so? It’s because sometimes you might encounter with some complicated scenarios when you will need to provide certain type of data to be displayed on your web-browser for testing a specific scenario. This may have saved a lot of time with some of the key advantages as:

1. You can simulate complex scenarios.
2. It is very fast and you are not spending time on waiting for the response from the real server i.e. saving the time on the networking as the response from the Cypress server comes back instantly because it’s located on the same machine you are running your test on and at the same time you can specify which API calls you still want to go through to the real API server and which one you want to mock.

Moreover, since Cypress is not just a UI functional testing framework, but in Cypress you can also make an API requests to the server without UI on behalf of the browser you can send the API request, get certain response from the backend server and then use this data as per your requirements.

### Example

#### Summary
* Cypress has built-in-server which can intercept browser API request and provide mock response.
* Cypress can make an API requests and process responses.
* Cy.intercept is very efficient and time-effective solution to deal with some complicated test scenarios.
