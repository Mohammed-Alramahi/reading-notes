# Readings: Express

#### What’s the difference between PUT and PATCH?

##### PUT

overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

##### PATCH

applies a partial update to the resource.

#### Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`

##### Mocky

Mocky is an incredibly simple and super lightweight testing implementation. Mocky is entirely a web app, meaning that everything is generated and managed remotely. This does mean that Mocky grants you significantly less control compared to solutions that focus more on local systems, but this also means the application is simpler and cleaner.

Mocky has great support for a ton of common functionality, but because it is a web app, you have to add this functionality in URL form. For instance, adding ?callback=myfunction enables jsonp; adding ?mocky-delay=100ms allows you to add delays. This sort of functionality still delivers quite a lot of value, but it does point to the relative simplicity of the app – if exceeding granular control is something that is desired, Mocky might not be the first option. For simple interactions, however, Mocky is a great choice.

#### Postman Mock Server

Mock Servers in Postman are tied directly to the Postman app, and for that reason, are a suggestion for a very particular use case. Postman is a great testing solution, and their mocking system is equally great, but the fact that it’s tied to both a Postman account and a defined collection means that using only the Mocking system means that you are buying into an incomplete testing experience. You can create a mock server without an existing collection, but in this case it’s kind of like buying an entire sewing kit for a single needle.

That may not be a deal-breaker, of course – Postman is an excellent testing system and is in relatively common use by many API developers. Still, the fact that the mocking system is but a single aspect of a much larger testing apparatus may deter some users. There’s also the fact that it’s not completely free – Postman allows a limited number of free mock calls, but users engaging in heavy development may quickly find themselves exhausting this limited number.

#### Mockserver

Mockserver is a library that utilizes deride records in order to serve practical deride reactions. It does this by making nearby taunt records that serve substance as on the off chance that they were portion of a genuine API localized on port 9001. Since of the generally clean and fast execution, Mockserver brags that API deriding can be made in “a matter of seconds” – more to the point, since such a framework is super lightweight, it moreover implies that it’s profoundly versatile over a wide range of options. For this reason, Mockserver could be a incredible choice if quick testing is required with relative promptness. Mockserver is wordy, underpins custom headers, incorporates a built-in response delay recreation conspire, and offers a wide run of extra choices to imitate standard testing situations.

#### Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

Popularity: By comparing stats, swagger-ui is more prevalent at that point apidocjs. Consistency: In case we as of now utilizing swagger for our Dotnetcore benefit, at that point actualizing swagger device will comprise more from Information and UI prospective. Implementation complexity: apidocjs and swagger both required documentation substance on executed strategy as customize comment information. In expansion they permit to type in documentation information in partitioned asset record as .js and .json. In case we as of now have swagger.json made by DotnetCore we will reuse more than 80% specification. Support: For apidocjs will got to modify documentation for each influenced method/endpoints in the event that benefit changed. In swagger able to restrain changes. But by actualizing apidocjs we will confine the layer. Other benefits: Since swagger utilize plain .json that may be parsed through programing dialect, hence we will get advantage of different other 3rd parties in arrange to form http client and more. Future: Due to notoriety of swagger, apidocjs give

### swagger

`responses: 200: description: OK 400: description: Bad request. User ID must be an integer and bigger than 0. 401: description: Authorization information is missing or invalid. 404: description: A user with the specified ID was not found.`

### APIDoc.js

`responses: 200: description: OK 400: description: Bad request. User ID must be an integer and bigger than 0. 401: { "isError": true, "errorCode": 401, //--- or 500 depends on error type "errorMessage": "Not authorized" } 404: description: A user with the specified ID was not found.`
