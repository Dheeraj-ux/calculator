<doctype html>
<html>
<head>
<style type="text/css">
body{
background:black;}

.cal{
justify-content:center;
text-align:center;
margin-top:30%;
}
.cal-inner{
background:gray;
height:400px;
width:300px;
margin-left:22px;
border-radius:8px;
padding:10px 2px;
padding-bottom:15px;
}
input{
background:#00cc00;
width:94%;
padding:20px;
border-radius:6px;
pointer-events:none;
outline:none;
border:none;
text-align:right;
direction:ltr;
margin-top:10px;
}
.Int{
font-size:20px;
padding-right:10px;}
.btn{
width:20.6%;
padding:20px 0px;
border-radius:6px;
border:none;
margin:10px 3px 0px 3px;
outline:none;
background:whitesmoke;
font-size:15px;}
.btn-equal{
font-size:15px;
width:90.6%;
padding:20px 0px;
border-radius:6px;
border:none;
margin:10px 3px 0px 3px;
outline:none;
background:#ff8533;
color:white;
}
.btn1{
width:20.6%;
padding:20px 0px;
border-radius:6px;
border:none;
margin:10px 3px 0px 3px;
outline:none;
background:whitesmoke;
font-size:15px;
background:#0040ff;
color:white;}
.btn2{
width:20.6%;
padding:20px 0px;
border-radius:6px;
border:none;
margin:10px 3px 0px 3px;
outline:none;
background:whitesmoke;
font-size:15px;
background: #ff1a1a;
color:white;}

</style>
</head>
<body>
<div class="cal">
<div class="cal-inner">
<input type="text" class="Int" placeholder="0">
<br>
<button class="btn" onclick="press(1)">1</button>
<button class="btn" onclick="press(2)">2</button>
<button class="btn" onclick="press(3)">3</button>
<button class="btn1" onclick="press('+')">+</button>

<button class="btn" onclick="press(4)">4</button>
<button class="btn" onclick="press(5)">5</button>
<button class="btn" onclick="press(6)">6</button>
<button class="btn1" onclick="press('-')">-</button>

<button class="btn" onclick="press(7)">7</button>
<button class="btn" onclick="press(8)">8</button>
<button class="btn" onclick="press(9)">9</button>
<button class="btn1" onclick="press('*')">*</button>

<button class="btn2" onclick="erase()">C</button>
<button class="btn" onclick="press(0)">0</button>
<button class="btn1" onclick="press('.')">.</button>
<button class="btn1" onclick="press('/')">/</button>

<button class="btn-equal" onclick="equal()">=</button>
</div>
</div>
<script type="text/javascript">
let user=document.querySelector(".Int");
let expression="";

function press(num){
expression+=num;
user.value=expression;
}

function equal(){
user.value=eval(expression);
expression="";
}
function erase(){
expression="";
user.value=expression;
}
</script>
<acronym>
</body>
</html>
