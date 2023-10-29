# javascript-DOM

## Query Selector
```
document.querySelector("ul"); //element
document.querySelector("#title"); //id
document.querySelector(".btn"); // class
document.querySelector("li a"); // Descendant combinator
document.querySelector("#list a"); // Descendant combinator
document.querySelector("#list .item"); // Descendant combinator
document.querySelector("li.item"); // Chaining
```
### Text/HTML
```
document.querySelector("ul").lastElementChild.innerHTML = "3rd";
document.querySelector("h1").innerHTML = "Good Bye";
document.querySelector("h1").innerHTML = "<em>Good Bye</em>";
document.querySelector("h1").textContent = "Good Bye";
```
### CSS
```
document.querySelector("h1").style.fontSize = "10rem"
document.querySelector("h1").style.visibility = "hidden";
document.querySelector(".btn").style.backgroundColor = "Yellow"
```
### Class
```
document.querySelector(".btn").classList.add("invisible");
document.querySelector("h1").classList.add("huge");
document.querySelector(".btn").classList.remove("invisible");
document.querySelector(".btn").classList.toggle("invisible");
```
### Attribute
```
document.querySelector("a").getAttribute("href");
document.querySelector("a").setAttribute("href", "https://www.bing.com");
```
### Select All
```
document.querySelectorAll("#list .item");
document.querySelectorAll("#list .item")[2].style.color = "blue";
```

## Other Selector
```
document.getElementsByTagName("li").length;
document.getElementsByTagName("li")[2].color = "purple";
```
```
document.getElementsByClassName("btn");
```
```
document.getElementById("title").innerHTML = "Good Bye";
```

## Event Listener
```
for (var i = 0; i < document.querySelectorAll("button").length; i++) {
  document.querySelectorAll("button")[i].addEventListener("click", function () {
  document.querySelector("h1").style.color = "purple";
  });
}
```
