var add = document.querySelectorAll(".add");
var down = document.querySelectorAll(".down");
var num = document.querySelectorAll(".num");
var total = document.querySelectorAll(".total");
var price = document.querySelectorAll(".price");
var totalNum = document.querySelector(".box .totalNum span");
var totalPrice = document.querySelector(".box .totalPrice span");

for (let i = 0; i < add.length; i++) {
  add[i].onclick = function () { handler(i, true) }
  down[i].onclick = function () { handler(i, false) }
}
function handler(i, bol) {
  var count = num[i].innerText;
  bol ? ++count : --count;
  if (count <= 0) count = 0;
  num[i].innerText = count;
  total[i].innerText = price[i].innerText * count;
  totalNum.innerText = handlerConcat(num)
  totalPrice.innerText = handlerConcat(total)
}
function handlerConcat(dom) {
  let total = 0;
  for (let i = 0; i < dom.length; i++) {
    total += Number(dom[i].innerText);
  }
  return total
}