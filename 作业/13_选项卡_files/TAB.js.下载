var wrap_img = document.querySelector(".wrap .wrap_img");
var wrap_but = document.querySelectorAll(".wrap .but>div");
var arrows = document.querySelectorAll(".wrap .arrows>div");
var wrap = document.querySelector(".wrap");
var show_index = 0;

wrap_but.forEach(function (item, index, arr) {
  item.onclick = function () {
    wrap_but[show_index].classList.remove("show");
    show_index = index;
    wrap_img.style.transform = `translate(${show_index * -820}px)`;
    this.classList.add("show")
  }
})
arrows[1].onclick = function () { handle(true) }
arrows[0].onclick = function () { handle(false) }
function handle(flag) {
  wrap_but[show_index].classList.remove("show");
  flag ? show_index++ : show_index--
  if (show_index > 4) show_index = 0;
  if (show_index < 0) show_index = 4;
  wrap_img.style.transform = `translate(${show_index * -820}px)`;
  wrap_but[show_index].classList.add("show");
}
var time = setInterval(() => {
  handle(true)
}, 2000);
wrap.onmouseenter = function () {
  clearInterval(time)
}
wrap.onmouseleave = function () {
  time = setInterval(() => {
    handle(true)
  }, 2000);
}
