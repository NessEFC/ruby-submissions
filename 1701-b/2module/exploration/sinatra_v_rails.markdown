## Sinatra versus Rails Exploration

### Setup:

First, clone down the Rails project:

```terminal
git clone https://github.com/turingschool/job-tracker.git rails_project
```

And then clone down the Sinatra project:

```terminal
git clone https://github.com/turingschool/bike-share.git sinatra_project
```
Now cd into each project, run `bundle` on each project, and you're ready to go. We will only be looking at the code base and not interacting with the app. If you wanted to run the server and interact with the app, you would need to create your database, migrate your migrations, etc.

### Exercise:

Take a look at this stripped down Sinatra app and this stripped down Rails app. How are they different and how are they similar? Identify 5 differences, and for each one describe 1-2 implications. What effect does that difference have for each framework? If you don't know exactly, draw on your knowledge and experience and make some educated guesses/inferences. Also, practice your research skills to look into the differences.

* Rails has these folders in the project root that Sinatra doesn’t: bin, lib, log, public, and vendor. Also the Rails app includes helpers and mailers directories in the app directory. Rails also seems to break out the controllers into separate classes, but perhaps this practice can be implemented in Sinatra too.

Consulting blogs and commentary you find online, identify 3 similarities between Rails and Sinatra.

* Both Rails and Sinatra try to keep the code minimal, and both are web frameworks using ruby. Both use rack and ActiveRecord. Both can implement MVC structure.

Consulting blogs and commentary you find online, identify 3 things that distinguish Rails, advantages.

* Rails runs a lot of its code behind-the-scenes for you, while Sinatra is stripped down and exposed. This can be good for getting apps up and running very quickly or with minimal effort, but sometimes you don’t want certain code to run or certain features to be added without explicitly saying so. Rails also includes a routes class. Sinatra seems to be better with handling APIs. When you want Rails to perform a function for you, it can be overkill at times because it has a lot of boilerplate add-ons to the code. Once your app starts to scale up in size, it’s probably a good idea to switch over from Sinatra to Rails.

In your Rails project, what does the `routes.rb` file inside of the `/config` directory do? What does this correlate to in our Sinatra app?

* The routes file in Rails handles the HTTP routing (verbs and paths). This is the same as the first line of each Sinatra method in the controller file.


We teach Sinatra by adding some structures that Sinatra doesn’t need, but help you make the transition between Sinatra and Rails. What does a stripped down implementation of Sinatra look like, and what are the pieces we’ve added for educational purposes?

* A stripped down Sinatra app only needs the Sinatra gem, the require Sinatra statement at the top of the controller, and the first HTTP routing method for the root page. Then it’s just a matter of running your app file from the terminal. Everything else in the file structure was added for us to make the transition to Rails easier, like the database folder, MVC architecture, spec tests, etc.
