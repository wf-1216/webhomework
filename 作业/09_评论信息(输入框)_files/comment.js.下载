var but = document.querySelector("button")
var textarea = document.querySelector("textarea")
var show = document.querySelector(".show")
but.onclick = function () {
  var val = textarea.value;
  console.log(Boolean(!val));
  if (!val) return;
  var dom = document.createElement("p")
  dom.innerText = val;
  show.appendChild(dom);
  textarea.value = ""
}