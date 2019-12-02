### What i Learned Week 12

# All About That Text - this project we worked on the idea that we can put something in the input box AND when we click the button something happens using event listeners and functions for the buttons.


# To DOM - in this project we gave every function its own ``.js`` file and linked them all to the html.

# Componentize - I didnt fully understand this project at first. but then i understood what bootstrap was and we applied it to our html along with applying classes to make the web page look prettier.

# To-do Two - this project we had a to do list. With this to do list we were able to add new items with a time stamp as well as being able to make items complete and remove of the todo list.

# Oops - at first I had a rough time with this exercise. We were to return objects within a function using ``this`` and ``that`` .
 ``` javascript 
    * ex. const Stack = function() {
  return {
    items: [],
      add: function (firstName) {
        this.items.push(firstName)
      },
      remove: function () {
        let removed = this.items.splice(this.items.length-1, 1)[0]
        return removed
      },
      peek: function () {
        return this.items
      },

  }
}
```