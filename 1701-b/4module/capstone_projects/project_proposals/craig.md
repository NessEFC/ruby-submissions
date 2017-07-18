### Project Template

### [Pardon my French]

### Pitch

I want to build a web app that will help users (myself included) to learn French by displaying a French newspaper article, parsing through the words in the article, then saving those words to flashcards for study purposes.

### Problem

Foreign language learners need an easy way to gather (current, interesting) reading material in their target language, and utilize some sort of system for retaining vocabulary. Modern day flashcard systems typically use an algorithm to help with efficient memory retention, and reserach has shown that adding images to flashcards increases memory associations when learning. It would be nice to tie up all these loose ends into an easily-usable package, along with a way to display dictionary definitions/translations in-app to make learning convenient for the user.

### Solution

I want to pull in an article written in french (either by consuming an API if one exists, or by webscraping) and parse through the words in the article. The words will then be added as flashcards to the database (if they don't already exist) that users can then practice with (and possibly incorporate an SRS learning algorithm to prioritize which cards are shown and on what day). Users are then given relevant images to choose from (maybe from google images) that they can choose to add to each card, which helps to create strong associations with words. Finally, it would be cool if I could add in a French/English dictionary feature that would allow you to look up words in-app so that you don't have to open another tab and look them up.

### Target Audience

Any English speaker who is interested in learning French, and possibly other languages could be supported in the future.

### New Techniques

I want to use React for the front end and Rails on the backend. I'll consume APIs if they exist, but I might also build a webscraper to do that instead which I've wanted to try for a while now. If there was some way to incorporate text-to-speech to help with pronunciation, that would be cool too. Also, if there's time or if I need some new tech to fulfill the requirement, I can incorporate a JS library for data visualization for the user that would showcase their usage stats.

### Workflow

Even though I like Pivotal Tracker, I will probably use a Trello board since I'm the only one working on the project and it's more lightweight.
