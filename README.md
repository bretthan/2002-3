# 2002-3
To do List, Second day of Software Development


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-aec34940fbc1a6e787974dcd360f2c6b63348d4b1f4e06c77743096d55480f33.ico" />
<link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-8f3771b1072e3c38bd662872f6b673a722f4b3ca2421637d5596661b4e2132cc.svg" color="#111" />
<title>CodePen - 2002-3</title>
<style>
  h1{
  color:rgb(280,0,150); 
}

#mainlist{
  font-size: 180%;
  background-color:
}

.odd{
  background-color:rgba(225,225,265,0);
}

.even{
  background-color:rgba(225,225,300,0);
}

.alist{
  color:hotpink;
  font-size:25px;
  background-image:url("http://i48.fastpic.ru/big/2012/1120/33/6dfe090d37297946248ef2e28b452e33.png");
}
</style>
</head>
<body translate="no">
<h1 id="mainlist">To do list</h1>
<ul class="alist">
<li class="odd">Do Math Homework</li>
<li class="even"> Eat din din</li>
</ul>
<button id="add">Add</button>
<input id="item">
<script id="rendered-js">
      console.clear();
console.log("hello world");

const addBtn = document.getElementById("add");

addBtn.addEventListener('click',addItem)

function addItem(e){
  const theItem=document.getElementById("item").value;
  
  console.log('add item');
  var node = document.createElement("li");
  var textnode = document.createTextNode(theItem);
  node.appendChild(textnode);
  document.getElementsById("myList").appendChild(node);
  
  
}
    </script>
</body>
</html>

