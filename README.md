 <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Jasmine...</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  height: 100vh;
  background: #ffffff;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Tahoma, Arial, sans-serif;
}

input { display: none; }

.window {
  width: 330px;
  background: #c0c0c0;
  border: 2px solid #000;
  box-shadow: 2px 2px 0 #404040;
  display: none;
}

.title {
  background: linear-gradient(to right, #000080, #1084d0);
  color: white;
  padding: 4px 6px;
  font-size: 14px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.close {
  background: #ff0000;
  border: 1px solid #000;
  width: 16px;
  height: 16px;
  text-align: center;
  font-weight: bold;
  font-size: 12px;
  line-height: 14px;
}

.content {
  display: flex;
  gap: 12px;
  padding: 18px;
  font-size: 14px;
}

.icon {
  font-size: 26px;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 10px;
  padding: 0 18px 18px;
}

.btn {
  background: #c0c0c0;
  border: 2px outset #fff;
  padding: 4px 16px;
  cursor: pointer;
  font-size: 13px;
}

.btn:active {
  border: 2px inset #fff;
}

#s1:checked ~ .w1,
#s2:checked ~ .w2,
#s3:checked ~ .w3,
#s4:checked ~ .w4,
#s5:checked ~ .w5,
#s6:checked ~ .w6,
#s7:checked ~ .w7,
#s8:checked ~ .w8,
#s9:checked ~ .w9 {
  display: block;
}
</style>
</head>
<body>

<input type="radio" name="step" id="s1" checked>
<input type="radio" name="step" id="s2">
<input type="radio" name="step" id="s3">
<input type="radio" name="step" id="s4">
<input type="radio" name="step" id="s5">
<input type="radio" name="step" id="s6">
<input type="radio" name="step" id="s7">
<input type="radio" name="step" id="s8">
<input type="radio" name="step" id="s9">

<!-- Intro Windows -->

<div class="window w1">
  <div class="title"><span>Hello Jasmine...</span><div class="close">×</div></div>
  <div class="content"><div class="icon">ℹ️</div><div>I need to ask you something.</div></div>
  <div class="buttons"><label for="s2" class="btn">OK</label></div>
</div>

<div class="window w2">
  <div class="title"><span>Important</span><div class="close">×</div></div>
  <div class="content"><div class="icon">❤️</div><div>Jasmine, will you be my Valentine?</div></div>
  <div class="buttons">
    <label for="s6" class="btn">Yes</label>
    <label for="s3" class="btn">No</label>
  </div>
</div>

<!-- No Path Escalation -->

<div class="window w3">
  <div class="title"><span>Wait...</span><div class="close">×</div></div>
  <div class="content"><div class="icon">🤨</div><div>Really? You're saying no?</div></div>
  <div class="buttons">
    <label for="s4" class="btn">Yes...</label>
  </div>
</div>

<div class="window w4">
  <div class="title"><span>Are you sure?</span><div class="close">×</div></div>
  <div class="content"><div class="icon">😐</div><div>Are you absolutely sure about that?</div></div>
  <div class="buttons">
    <label for="s5" class="btn">I think so...</label>
  </div>
</div>

<div class="window w5">
  <div class="title"><span>Final Check</span><div class="close">×</div></div>
  <div class="content">
    <div class="icon">😏</div>
    <div>
      Last chance.<br><br>
      Think carefully.
    </div>
  </div>
  <div class="buttons">
    <label for="s7" class="btn">Still No</label>
  </div>
</div>

<div class="window w7">
  <div class="title"><span>Error</span><div class="close">×</div></div>
  <div class="content">
    <div class="icon">⚠️</div>
    <div>
      Invalid response detected.<br>
      Redirecting to correct answer...
    </div>
  </div>
  <div class="buttons">
    <label for="s6" class="btn">Continue</label>
  </div>
</div>

<!-- YES Screen -->

<div class="window w6">
  <div class="title"><span>Success</span><div class="close">×</div></div>
  <div class="content">
    <div class="icon"></div>
    <div>
      Yay 💐<br><br>
      I have some flowers for you.<br><br>
      — Elly
    </div>
  </div>
  <div class="buttons">
    <label for="s1" class="btn">Restart</label>
  </div>
</div>

</body>
</html>
