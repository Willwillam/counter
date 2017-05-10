# counter
简易计算器
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>confirm</title>
<script type="text/javascript">
function count(){
  var firstone=parseInt(document.getElementById('txt1').value);
  var secondone=parseInt(document.getElementById('txt2').value);
  var selects=document.getElementById('select').value;
  var result;
  switch(selects){
    case "+":
    result=firstone+secondone;
    break;
    case "-":
    result=firstone-secondone;
    break;
    case "*":
    result=firstone*secondone;
    break;
    case "/":
    result=firstone/secondone;
    break;
  }
 document.getElementById('txt3').value=result;
}
</script>
</head>
<body>
  <input type="text" id="txt1">
  <select id="select">
    <option value="+">+</option>
    <option value="-">-</option>
    <option value="*">*</option>
    <option value="">/</option>
  </select>
  <input type="text" id="txt2">
  <input type="button" value="=" onClick="count()">
  <input type="text" id="txt3">
</body>
</html>
