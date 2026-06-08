var wrap = document.querySelector(".wrap");
var x = y = 0;
document.documentElement.onkeydown = function (event) {
  switch (event.keyCode) {
    case 37:
      x -= 5;
      wrap.style.backgroundImage = "url(../img/左.png)";
      break
    case 38:
      y -= 5;
      wrap.style.backgroundImage = "url(../img/上.png)";
      break
    case 39:
      x += 5;
      wrap.style.backgroundImage = "url(../img/右.png)";
      break
    case 40:
      y += 5;
      wrap.style.backgroundImage = "url(../img/下.png)";
      break
  }
  wrap.style.transform = `translate(${x}px,${y}px)`;
}