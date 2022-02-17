Welcome! 

Come join me on my journey of Wes Bos's 30 Day Vanilla JS Code Challenge! Where I build 30 things in 30 days with 30 tuturials~
<br></br>
## Day 7 Challenge of Javascript30

### Array Cardio 2
---- 
In this challenge, I was given some test datasets and utilised other Array Methods using the data provided~

----
### What I learned:

#### .some()
  - method tests whether at least one element in the array passes the test implemented by the provided function
  - example from challenge (is at least one person 19 or older?) :
  ```js
  const isAdult = people.some(person => ((new Date()).
      getFullYear()) - person.year >= 19);
  ```
  returned true since there was a person 19 or older

#### .every()
- method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.
- example from challenge (is everyone 19 or older?):
```js
const allAdults = people.every(person => ((new Date()).getFullYear()) - person.year >= 19);
```
returned false since not everyone was 19 or older in the dataset

#### .find()
- like .filter except this method returns the first element in the provided array that satisfies the provided testing function. If no values satisfy the testing function, undefined is returned.
- example from challenge (find the comment with the ID of 823423):
```js
const comment = comments.find(comment => comment.id === 823423)
```

#### .findIndex()
- method returns the index of the first element in the array that satisfies the provided testing function. Otherwise, it returns -1, indicating that no element passed the test.
- example in challege (Find the comment with ID 823423)
```js
const index = comments.findIndex(comment => comment.id === 823423);
```
return 1 since its in the second position of the dataset array

Starter code from [Javascript 30 Challenge](https://github.com/wesbos/JavaScript30)