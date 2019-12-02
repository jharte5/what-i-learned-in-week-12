### What i Learned Week 12

# All About That Text - this project we worked on the idea that we can put something in the input box AND when we click the button something happens using event listeners and functions for the buttons.
    ex
``` javascript
document.querySelector('.biggify').addEventListener('click', function () {
    let val = document.querySelector('#user-input').value;
    const finalValue = biggify(val);
    generateResult(finalValue)
})
```


# To DOM - in this project we gave every function its own ``.js`` file and linked them all to the html.
    ex.
``` javascript
document.querySelector(‘.remove-todo’).addEventListener(‘click’, function(){
    document.querySelector(`.todo-list li:nth-child(${document.querySelector(‘.index-input’).value}`).remove();
})
```

# Componentize - I didnt fully understand this project at first. but then i understood what bootstrap was and we applied it to our html along with applying classes to make the web page look prettier.
    ex.
``` javascript
const addItem = function (str) {
    let hi = 'new item'
    todoList.push(hi);
    console.log(todoList)
}
```

# To-do Two - this project we had a to do list. With this to do list we were able to add new items with a time stamp as well as being able to make items complete and remove of the todo list.
    ex.
``` javascript
document.querySelector('.add-todo').addEventListener('click', function(){
const listArr = [];
if (inputBox.value !== '' && inputBox.value !== ' '){
listArr.push(Object.values(createObject()));
for (const item of listArr){
    document.querySelector('.todo-list').appendChild(document.createElement('li')).innerText = `${item[0]}\n${item.slice(1)}`;
    markLi();
}
inputBox.value = '';
}
});
```


# Oops - at first I had a rough time with this exercise. We were to return objects within a function using ``this`` and ``that`` .
 ``` javascript 
const Stack = function() {
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