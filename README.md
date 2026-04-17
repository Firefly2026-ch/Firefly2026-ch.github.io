# Firefly2026-ch.github.io
A surprise webpage
<yb_canvas uuid="571290de-27a0-beef-4cf6-4e73bd772a63" mversion="13" type="code" subtype="single">

<title>给许欣怡的特别惊喜</title>

<filename>index.html</filename>

<yb_code lang="html"><!DOCTYPE html>

<html lang="zh-CN">

<head>

<meta charset="UTF-8">

<title>给许欣怡的特别惊喜</title>

<style>

body {

background: linear-gradient(135deg, #6a11cb, #2575fc);

font-family: "Microsoft YaHei", sans-serif;

color: white;

text-align: center;

padding: 20px;

min-height: 100vh;

}

.box {

background: rgba(255,255,255,0.95);

border-radius: 20px;

padding: 40px;

margin: 20px auto;

max-width: 800px;

color: #333;

}

h1 { color: #6a11cb; margin-bottom: 20px; }

input {

padding: 12px 20px;

font-size: 16px;

border: 2px solid #6a11cb;

border-radius: 10px;

width: 200px;

margin: 20px 10px;

}

button {

padding: 12px 30px;

background: #2575fc;

color: white;

border: none;

border-radius: 10px;

font-size: 16px;

font-weight: bold;

cursor: pointer;

}

.hidden { display: none; }

.message {

text-align: left;

line-height: 1.8;

margin-top: 30px;

}

</style>

</head>

<body>

<div class="box">

给许欣怡的特别惊喜 💫

这是一份只为你准备的小惊喜。请输入密码查看隐藏信息：
<input type="password" id="pwd" placeholder="输入密码...">
<button onclick="checkPwd()">解锁</button>

<div id="msg" class="hidden message">
    <h2>许欣怡，看到这里你是否感到惊讶与疑惑？</h2>
    <p>为什么我要花费一天一夜研究、制作这个网页？因为我有许多许多话想对你说。我一直、一直在试探，我想跟你搞好关系，但是我的表达能力真的很堪忧，正当想说的时候总是说不出口，所以才会用这种方式，敬请见谅！</p>
    <p>在遇到你的前16年里，我才发现我一直在浑浑噩噩地生活，丝毫没有注意生活中的真善美。但遇见你之后，你的一举一动都让我感受到真切的温暖，我也不止一次说过，我真的很感谢你送我的小狗，因为这是我进入高中以来收到的第一份善意，从那时起，你的形象就已经在我心里扎根了。之后我总会不觉间注意你，会因为你的满足而满足，会因为你的悲伤而悲伤。</p>
    <p>还记得那次运动会的跑步比赛上由于意外，让你丢失了更高的名次，那是我第一次见你哭。当时我的心里也很难受，不止是遗憾，还有对你以善待世界，而世界并不总以善待你的不平和心疼。</p>
    <p>你是个心思很细腻的女孩，总是为别人着想，把别人看的比自己更重，这没有什么对错可言。但我也希望你能明白，自己也并非不重要，在芸芸众生中，也一定有人像你一样，会把你看的比自身更重要。</p>
    <p>高中三年，我能与你共同度过，已是我的一大幸事。不知不觉，你也已经成为了一位17岁的妙龄少女了。我衷心祝你生日快乐，天天开心，诸事顺遂！</p>
    <p style="text-align:right;font-style:italic;color:#666;margin-top:30px;">—— 默默一直关注着你的人</p>
</div>
</div>

<script>
// 密码验证函数
function checkPwd() {
    var password = document.getElementById("pwd").value;
    var message = document.getElementById("msg");
    
    if (password === "090823") {
        message.classList.remove("hidden");
        document.querySelector("h1").innerHTML = "🔐 解锁成功！";
        document.querySelector("input").style.display = "none";
        document.querySelector("button").style.display = "none";
        document.querySelector("p:nth-child(2)").innerHTML = "密码正确，请看下面的信息：";
    } else {
        alert("密码不对哦，再试试看？😊");
        document.getElementById("pwd").value = "";
        document.getElementById("pwd").focus();
    }
}

// 回车键支持
document.getElementById("pwd").onkeydown = function(e) {
    if (e.key === "Enter") {
        checkPwd();
    }
};
</script>
</body>

</html>
