# Template processor || Template Engine

- A template processor (also known as a template engine or template parser) is software designed to combine templates with a data model to produce result documents.

### In terms of Express

- A template engine enables you to use static template files in your application. At runtime, the template engine replaces variables in a template file with actual values, and transforms the template into an HTML file sent to the client. This approach makes it easier to design an HTML page.

# Template Language

- The language that the templates are written in is known as a template language or templating language.

# Setup in Express

- install Pug:
  - \$ npm install pug --save
- After the view engine is set, you don’t have to specify the engine or load the template engine module in your app
  - app.set('view engine', 'pug')
- Create a pug templete file named index.pug
- create a route to render the index.pug

  - app.get('/', function (req, res) {
    res.render('index', { title: 'Express', message: 'Express Implementation' })
    });

- When you make a request to the home page, the index.pug file will be rendered as HTML.
