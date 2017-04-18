# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsibilities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
Models are Ruby classes.  They do the "heavy lifting" - carrying out the business logic of the application and the rules to manipulate data and talk to the database.
```

## Define Controller Responsibilities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer essentially responds to user interactino.  It parses requests made by the user and handles data submissions, cookies, sessions, logins/authorization, errors, and redirection.  A controller can have more than one action.  For example, a controller might have an action to display a list of users, or add/delete a user from a list.
```

## Define Router Responsibilities

In your own words, define what the router does in Rails.

```md
When an HTTP request arrives, it needs to know which controller action shoudl be run. The router takes requests, recognizes URLs, and directs them to the appropriate controller action.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
-The user opens a browser and makes a request for the URL.
-The request makes its way to the router.
-Router maps the request to the correct controller and action.
-Action receives the request, and the model retrieves data from the database
-Model returns a list of data to the controller action.
-Conroller action passes the data to the view.
-View renders the page
-Controller sends the HTML to the browser, where the page loads for the user to see.

```
