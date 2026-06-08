var wrap = document.querySelectorAll(".wrap input");
var show = document.querySelectorAll(".wrap .show");
var userReg = /^[\w\u4e00-\u9fa5]{2,6}$/;
var passReg = /^[A-Z][\w\.\+\?\(\)\{\}]{7,15}$/;
wrap[0].onchange = function () {
  var value = this.value.trim();
  if (!value) return;
  var bol = userReg.test(value);
  if (!bol) {
    show[0].innerText = "由2至6位数字与字母或中文组成用户名";
    setTimeout(() => {
      show[0].innerText = ""
    }, 3000);
  }
}
wrap[1].onchange = function () {
  var value = this.value.trim();
  if (!value) return;
  var bol = passReg.test(value);
  if (!bol) {
    show[1].innerText = "首字母大写，数字与字母与特殊符号组成8-16";
    setTimeout(() => {
      show[1].innerText = ""
    }, 3000);
  }
}