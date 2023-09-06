[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11754498&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length)) //I used https://www.w3schools.com/jsref/jsref_slice_array.asp#:~:text=Description,not%20change%20the%20original%20array. to figure out what slice does
    if(foo > a[0]) return foo;
    else return a[0];
}
```


I believe that the mystery array first checks the array length and if it is 1 it just returns the only element. It then makes a "sub array" using slice then it then checks the elements to see which is the biggest it then returns the biggest and keeps running until it returns the biggest value of the array at the end. 