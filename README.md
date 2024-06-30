<!DOCTYPE html>
<html>
<head>
  <title>Click Counter</title>
</head>
<body>

<h1>Click the button to increase the count</h1>
<p>Count: <span id="count">0</span></p>
<button id="clickButton">Click me!</button>

<h2>Options:</h2>
<button id="shopButton">Shop</button>
<button id="friendsButton">Friends</button>

<script>
  let count = 0;
  const countElement = document.getElementById('count');
  const clickButton = document.getElementById('clickButton');
  const shopButton = document.getElementById('shopButton');
  const friendsButton = document.getElementById('friendsButton');

  clickButton.addEventListener('click', function() {
    count++;
    countElement.textContent = count;
  });

  shopButton.addEventListener('click', function() {
    alert('You are entering the shop.');
  });

  friendsButton.addEventListener('click', function() {
    alert('You are checking your friends list.');
  });
</script>

</body>
</html>


