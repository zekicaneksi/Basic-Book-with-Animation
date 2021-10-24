# Basic-Book-with-Animation
A very basic, unstyled book.

![book](https://user-images.githubusercontent.com/59491631/138607049-62063a05-859e-4bd3-a9c0-8289cc5b1665.gif)


The book has such a variable;
```
    var bookContents = [
        "<div id=\"project0\" class=\"fill\"><h2>hello from project 0</h2></div>",
        "<div id=\"project1\" class=\"fill\"><h2>hello from project 1</h2></div>",
        "<div id=\"project2\" class=\"fill\"><h2>hello from project 2</h2></div>",
        "<div id=\"project3\" class=\"fill\"><h2>hello from project 3</h2></div>",
        "<div id=\"project4\" class=\"fill\"><h2>hello from project 4</h2></div>",
        "<div id=\"project5\" class=\"fill\"><h2>hello from project 5</h2></div>",
        "<div id=\"project6\" class=\"fill\"><h2>hello from project 6</h2></div>",
    ];
```

You can put whatever HTML in the content you want, and you can style them as well just like i did in my book;

```
#project0{
    background-color: red;
}

#project1{
    background-color: blue;
}

.
.
.

#project6{
    background-color: brown;
}

.fill{
    position: relative;
    width: 100%;
    height: 100%;
}

.fill h2{
    margin:0;
}
```

You can style the book itself as well pretty easily if you check out the code.

And finally, the logic behind the book:<br /><br />
There are 3 main divs; one pinned to the left, one pinned to the right, and one div that turns. The turning div has two divs which are the front and the back side.<br /><br />
When you turn a page, left or right pinned page copies the inner html of your turning div's back or front side, then the turning div just turns. And if you want to turn the page again, lets say you want to turn the right page twice in a row, for the second time, the turning div immediately resets to its original position, then it does the turn again with animation. And that's all there is to it.
