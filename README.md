
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-aec34940fbc1a6e787974dcd360f2c6b63348d4b1f4e06c77743096d55480f33.ico" />
<link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-8f3771b1072e3c38bd662872f6b673a722f4b3ca2421637d5596661b4e2132cc.svg" color="#111" />
<title>CodePen - 2002-3</title>
<style>
  h1{
  color:rgb(300,88,150);
  background-image:url("http://digitalimagemakerworld.com/images/pink-glitter-wallpaper/38120261-pink-glitter-wallpaper.jpg");
  background-repeat: repeat-y;
  
  
  margin-bottom:-25px
}

#mainList{
    font-size:250%;
}

.odd{
  background-color:rgba(225,225,225,.0)
}

.even{
  background-color:rgba(100,100,100,0);
}

.aList{
  color:#FA8FAA;
  font-size:25px;
  background-image:url("https://media0.giphy.com/media/QmZmvRoZIUNP2/giphy.gif");
  background-repeat: repeat-y;
  
  
   
}

#add{
  background-image: url("http://images2.fanpop.com/images/photos/7500000/Butterflies-butterflies-7572197-396-307.gif"); 
  background-size: 18% 100%;
    background-color: transparent; 
    background-repeat: no-repeat;
    background-position: 0px 0px;
    border: none;
    height: 30px;           
    padding-left: 16px;    
    vertical-align: middle; 
  font-size:20px;
    font-family: "Lucida Console", Times, serif;
  color:transparent;
   font-weight:900px;
}
</style>
</head>
<body translate="no">
<h1 id="mainList">To do list</h1>
<ul class="aList" id="myList">
<li class="odd">Do math homework</li>
<li class="even">Eat dinner</li>
</ul>
<button id="add">Press ME PLEAASEJI</button>
<input id="item">
<script id="rendered-js">
      console.clear();
console.log("hello world");

const addBtn = document.getElementById("add");

addBtn.addEventListener("click", addItem);

function addItem(e) {
  const theItem = document.getElementById("item").value;
  console.log("add item", theItem);
  var node = document.createElement("li");
  var textnode = document.createTextNode(theItem);
  node.appendChild(textnode);
  document.getElementById("myList").appendChild(node);
}
    </script>
</body>
</html>
