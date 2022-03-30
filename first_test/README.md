## Solutions Engineer's first test
Welcome! Please spend some time answering the questions you can find below

We do not expect reading code here.
## Questions
* Imagine that you have two classes named "Animal" and "Dog" and you want the class "Dog" to have all the properties and methods from the class "Animal", how would you do it? How is this called? What's the benefit?
- *I would make "Dog" as a subclass of "Animal", using ES6 syntax it would go something like: `class Dog extends Animal{...}`*
* A call to the setTimeout() global method can block the event loop in NodeJS. Is this true or false? Why?
- *false, setTimeout is an asynchronous web api that basically queues a function to be called after x time has elapsed. So if you run a function that contains a setTimeout, the callback from said setTimeout will be placed on a different callback queue that will run as soon as the current call stack queue is empty. Therefore it is not blocking the event loop, it is just waiting for the call stack queue to be empty to run the callback function.*
* How can you share information between components on a React application?
- *you either pass them as props from component to component, or with the aid of other state management library like Redux which provides certain hooks to access information stored in the redux store.*
* How would you protect a REST API against potential SQL Injections?
- *the easiest way would be by doing input validation, you can do this by setting certain limitations on what can be inputed on the client side. You could also use an ORM layer so that your backend doesnt do any direct SQL queries.*
* What does the level of coupling measure in software development?
- *It measures how dependent one module is from another. The recommendation is to aim for low coupling when creating software, you want each module to be as independent as possible so that if one fails, they dont all fail as well.*
* What is CI? Have you used one before?
- *continuous integration, it is usually used along with continuous delivery or deployment. It works by having developers merge their changes to a "shared" branch on which their changes will be tested to ensure they dont break the application, this CI process is done regularly to avoid having multiple merge conflicts down the development line.I have worked with it before.*
* How would you deploy a Node application?
- *there are different ways and services that do this, I have only ever deployed using AWS with elastic beanstalk and codepipeline. You basically rent a "computer" on which your server runs the desired application.*
* Why do we do code reviews?
- *for quality assurance. It helps identify problems with the code that may become a problem in the future and therefore prevent them.*
* In which files would you store API tokens, passwords, or similars?
- *.env files.*
* What are the benefits of using Typescript?
- *it is a sort of version of javascript that is less prone to bugs because of its strongly typed nature, it allows you to have more control over the structure, inputs and outputs of your code.*
* Describe with your own words a web socket?
- *web sockets allow you to keep a two way connection open between the client and server so you can pass information instantly without the need of making constant requests every time something changes.*
* Describe with your own words a GraphQL API.
- *an alternative to the more widely used REST api where you create different type definitions, queries and mutations to communicate with the server and get back the data you need in the shape of a previously defined interface. It differs with REST mainly because instead of having different endpoints for different http methods such as `GET`, `POST`, `PUT`, `DELETE`, you can have only one endpoint on which you can send queries, mutations and subscriptions.*
* How do you keep yourself up-to-date in regards the technologies you do use?
- *I like to browse forums dedicated to software development and programming, mainly on reddit, hackernews and softwareengineeringdaily. If I hear about something new and interesting I usually go to youtube to hear a more detailed explanation and maybe try to implement it in a personal project.* 