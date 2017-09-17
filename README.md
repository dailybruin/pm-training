# Daily Bruin PM Training

## Your Role
As a PM, you are in charge of one of the many Daily Bruin projects! Wow! That’s a very exciting role, but also comes with a lot of responsibility.

## Agile
Agile is a word that carries a lot of connotative weight: people either love or hate the term, and 

The most important thing to know about Agile, Lean, Scrum, Kanban, and other management terms is that they all serve the same purpose: increasing the productivity of a team. If that means that part or all of it isn’t working, __don’t do it__. Each team is different and works differently. Your job as a manager is to know what kind of structure can best complement your team.

With that being said, we’d like to give you some recommendations as a starting point on how we managed our teams.

### Definitions
Firstly, some definitions:

__Agile__: a set of values and principles defined in the [Agile Manifesto](http://agilemanifesto.org). The core ideas it advocates are adaptive planning, continuous delivery, flexible response to change, simplicity, and effective communication.

__Scrum__: the most popular Agile framework[^1]. The main features of Scrum are timeboxed “sprints”, daily “stand-ups”, 3 defined roles, and a “product backlog”. Lyssa Adkins gives a [good overview of Scrum](https://www.youtube.com/watch?v=_BWbaZs1M_8).

__Kanban__: Kanban shares a lot of features with Scrum, including stand-ups, a backlog, and a board. The main difference it that there are no sprints or roles, and tasks are just continuously done. Kanban also imposes limits on tasks that can be in progress, which ensures a team finishes tasks before moving on to the next tasks.

__Lean__: Lean software development is was taken from a methodology of manufacturing called “Lean”. It espouses [7 principles](https://en.wikipedia.org/wiki/Lean_software_development), including eliminating waste and delivering as fast as possible.

Confused about all these terms? This [blog post by Natalie Nedre](https://realtimeboard.com/blog/choose-between-agile-lean-scrum-kanban/) might help you.

__Async__: A set of values and principles declared in the [Async Manifesto](http://asyncmanifesto.org). Where Scrum and Kanban can be strict and unflexible, Async software development favors flexibility, documentation, and asynchronous communication over meetings. Lots of companies have been adopting asynchronous methods of communication as the tools in this category grows, [early GitHub is a good example of this](https://zachholman.com/posts/how-github-works/).

### The Useful Bits
While all of these terms and concepts are interesting, they can’t all be used in our part-time, volunteer-based context (the most obvious example being the daily stand-up).  There are a lot of good ideas you can and should take in your management, though.

#### Continuous and Iterative Delivery of Working Software
This encompasses a couple different Agile concepts into one, but continuous delivery, iterative development, and working software really all lead themselves to the same action.
- Sustainable and Simple Development
- Flexibility to Change
- Support Individuals
- Reflection

## Code Quality
The readability, structure, and testability of your product matter a lot, especially on larger and more sustained projects. UCLA doesn’t do much in the way of teaching what good collaborative practices are, so we detailed a some below. Note that many of these are opinion based, but have reasoning behind them. If you disagree with the reasoning, make a pull request and let us know why! However, just because you disagree with the reason that does not mean you can’t follow them—they are standards so that teams within DB can work easily together and members can switch teams with minimal ramp-up. 

### Files
EditorConfig is a tool to ensure that every text editor uses the same character set, line endings, etc. Every project should have an `.editorconfig` file and every contributor to said project should have an appropriate [EditorConfig plugin](http://editorconfig.org/#download).

### Linting
Make sure your team has all the necessary linters installed for your project and that the linter configuration on your project is enable correctly. When reviewing their pull requests, check for linter errors!

### Structure
Ensure that the structure of your project makes sense. It should follow a well-established software architecture pattern such as [model–view–controller](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller). Folders should be well-name and there should be a description in the readme of the general order of files.

### README
Every project should have a `README.md` file, and  that readme __must__ contain instructions on how to setup and deploy your project, as well as a general description of how the project is structured.

### Documentation
Aside from the readme, documentation is a more up to your discretion. We would highly recommend documenting classes and functions in longer term projects with comments in code, using [JSDoc](https://duckduckgo.com/?q=jsdoc&t=osx&ia=software "jsdoc"), [Docstrings](https://www.python.org/dev/peps/pep-0257/), or a language’s equivalent.

### Git and GitHub
You can read our Git workflow in the training repository. Make sure your team has Git Town installed and understands the workflow!

In addition to Git, GitHub is integral to the DB workflow; make sure everyone on your team knows how to use it, and use it well. You should be using features such as [protected branches](https://help.github.com/articles/working-with-protected-branches/), [code owners](https://help.github.com/articles/about-codeowners/), [issue](https://help.github.com/articles/creating-an-issue-template-for-your-repository/) and [pull request](https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/) templates, [squash merges](https://help.github.com/articles/configuring-commit-squashing-for-pull-requests/), and more.

### Testing
Testing is something that traditionally DB hasn’t done. Not all projects will require tests, but we __highly recommend__ them on any long term project. Use [Travis CI](https://travis-ci.org) for continuous integration.

### Twelve Factor
A couple of developers from Heroku got together a wrote a set of guidelines to make web app deployment as easy as possible. It’s called the [twelve-factor methodology](https://12factor.net). We’d like to see all DB projects be twelve-factored.

## Communication
### Slack
Slack should be your primary form of communication with your team. Make a Slack channel for your project (if there isn’t already one), add your team, add the Online editors, and add anyone else who may be relevant to the project (e.g., design people or the requesting section editor). __Don’t use Facebook messenger__.

### GitHub
GitHub is where all communication about code should go. Make and assign issues for each of your team members. Give through code reviews and talk about bugs in pull requests.

### Meetings
We recommend the following structure for meetings: once a week, for 1 hour with the first 30 minutes being a mandatory check-in with everyone to see how they are doing. The second 30 minutes is optional for team members and should be devoted to helping anyone with specific issues they’ve been having.

### Trello
GitHub has a Kanban board feature with GitHub Projects, so we recommend using GitHub over Trello. Trello should be used only for other sections to request Online content, but further communication with the requestors should be done through Slack. 

### Email
You can send out weekly emails updates to your team, but this is optional.

## Feedback
Actively encourage feedback from your team!

[^1]:	Agile is the idea, while frameworks like Scrum and Kanbans are stricter sets of rules that both follow the ideas of Agile.