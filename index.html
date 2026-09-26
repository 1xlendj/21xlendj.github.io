<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>九一授权系统</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; font-family: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Helvetica Neue", "PingFang SC", sans-serif; -webkit-tap-highlight-color: transparent; }

:root {
  --text: #f5f5f7;
  --dim: rgba(245,245,247,0.55);
  --faint: rgba(245,245,247,0.35);
  --ok: #30d158;
  --bad: #ff453a;
}

html, body { background: #000; }

body {
  color: var(--text);
  min-height: 100vh;
  overflow-x: hidden;
  position: relative;
  -webkit-font-smoothing: antialiased;
}

/* 背景光斑 —— 厚重、缓慢浮动 */
body::before, body::after { content:''; position: fixed; border-radius: 50%; filter: blur(70px); z-index: -2; opacity: .7; }
body::before { width: 46vw; height: 46vw; top: -14vw; left: -12vw;
  background: radial-gradient(circle, rgba(64,92,255,.55), rgba(120,80,200,.3) 55%, transparent 72%);
  animation: fl1 14s ease-in-out infinite; }
body::after { width: 40vw; height: 40vw; bottom: -10vw; right: -8vw;
  background: radial-gradient(circle, rgba(255,45,150,.4), rgba(255,120,60,.25) 55%, transparent 72%);
  animation: fl2 17s ease-in-out infinite; }
@keyframes fl1 { 0%,100%{transform:translate(0,0)} 50%{transform:translate(4vw,3vw) scale(1.06)} }
@keyframes fl2 { 0%,100%{transform:translate(0,0)} 50%{transform:translate(-3vw,-4vw) scale(1.1)} }

/* 第三块光斑 */
.orb3 { position: fixed; width: 34vw; height: 34vw; border-radius: 50%; z-index: -2; opacity: .55;
  background: radial-gradient(circle, rgba(0,200,255,.3), transparent 70%); filter: blur(60px);
  top: 38%; left: 50%; transform: translate(-50%,-50%); animation: fl3 20s ease-in-out infinite; }
@keyframes fl3 { 0%,100%{transform:translate(-50%,-50%) scale(1)} 50%{transform:translate(-50%,-50%) scale(1.14)} }

/* 玻璃块 —— 厚玻璃：深色内底 + 亮边 + 内外阴影 */
.glass {
  background:
    linear-gradient(140deg, rgba(255,255,255,.10), rgba(255,255,255,.02) 45%, rgba(0,0,0,.25)),
    rgba(20,20,28,.42);
  backdrop-filter: blur(34px) saturate(170%);
  -webkit-backdrop-filter: blur(34px) saturate(170%);
  border: .5px solid rgba(255,255,255,.28);
  border-radius: 22px;
  box-shadow:
    inset 0 1px 0 rgba(255,255,255,.32),
    inset 0 -1px 0 rgba(0,0,0,.35),
    0 10px 40px rgba(0,0,0,.45),
    0 1px 3px rgba(0,0,0,.5);
}

/* 布局 */
.wrap { max-width: 460px; margin: 0 auto; padding: 16px; position: relative; z-index: 1; }
.wrap.admin { max-width: 820px; }

/* 头部玻璃块 */
header { text-align: center; padding: 30px 20px; margin-bottom: 18px; }
.logo { font-size: 26px; font-weight: 700; letter-spacing: 1.5px;
  background: linear-gradient(180deg, #fff 30%, rgba(255,255,255,.68) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
.sub { font-size: 12.5px; color: var(--faint); margin-top: 7px; letter-spacing: .5px; }

/* 分段控制器 */
.seg {
  display: flex; gap: 4px; padding: 4px; margin: 0 auto 22px;
  width: fit-content; border-radius: 12px;
  background: rgba(255,255,255,.08); backdrop-filter: blur(20px);
  border: .5px solid rgba(255,255,255,.18);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.15), inset 0 -1px 0 rgba(0,0,0,.3);
}
.seg button {
  border: 0; background: transparent; color: var(--dim); cursor: pointer;
  padding: 8px 22px; border-radius: 9px; font-size: 14px; transition: .25s; font-weight: 500;
}
.seg button.on {
  color: #000; background: rgba(255,255,255,.92);
  box-shadow: 0 2px 8px rgba(0,0,0,.25), inset 0 1px 0 rgba(255,255,255,.9);
}

/* 输入 */
input {
  width: 100%; padding: 16px 18px; border-radius: 16px;
  background: linear-gradient(140deg, rgba(255,255,255,.09), rgba(255,255,255,.02));
  border: .5px solid rgba(255,255,255,.24); color: #fff; font-size: 16px; outline: none;
  backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.18), inset 0 -1px 0 rgba(0,0,0,.25), 0 2px 8px rgba(0,0,0,.15);
  transition: .25s; margin-bottom: 14px; font-family: inherit;
}
input:focus {
  border-color: rgba(255,255,255,.5); background: linear-gradient(140deg, rgba(255,255,255,.13), rgba(255,255,255,.03));
  box-shadow: inset 0 1px 0 rgba(255,255,255,.3), inset 0 -1px 0 rgba(0,0,0,.25), 0 0 0 4px rgba(255,255,255,.06);
}
input::placeholder { color: var(--faint); }

/* 按钮 —— 厚玻璃质感 */
.btn {
  width: 100%; padding: 15px; border-radius: 16px; cursor: pointer;
  border: .5px solid rgba(255,255,255,.26); color: #fff; font-size: 16px; font-weight: 600;
  background: linear-gradient(140deg, rgba(255,255,255,.18), rgba(255,255,255,.05) 50%, rgba(0,0,0,.12));
  backdrop-filter: blur(22px); -webkit-backdrop-filter: blur(22px);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.3), inset 0 -1px 0 rgba(0,0,0,.22), 0 4px 14px rgba(0,0,0,.25);
  margin-bottom: 12px; transition: .15s; letter-spacing: .5px; font-family: inherit;
}
.btn:active { transform: translateY(1px) scale(.99);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.16), inset 0 2px 6px rgba(0,0,0,.3), 0 1px 3px rgba(0,0,0,.25); }
.btn.primary { background: linear-gradient(140deg, rgba(120,180,255,.32), rgba(90,120,255,.22) 55%, rgba(40,50,140,.28)); }
.btn.danger  { background: linear-gradient(140deg, rgba(255,110,100,.26), rgba(255,70,60,.18) 55%, rgba(140,30,30,.25)); }

/* 状态 / 结果 */
.status {
  margin-top: 14px; padding: 15px 18px; border-radius: 16px; font-size: 14px; color: var(--dim);
  background: linear-gradient(140deg, rgba(255,255,255,.08), rgba(255,255,255,.02));
  border: .5px solid rgba(255,255,255,.2);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.18), inset 0 -1px 0 rgba(0,0,0,.2);
}
.result {
  margin-top: 14px; padding: 20px; border-radius: 16px; display: none;
  background: linear-gradient(140deg, rgba(48,209,88,.14), rgba(48,209,88,.04));
  border: .5px solid rgba(48,209,88,.4);
  box-shadow: inset 0 1px 0 rgba(255,255,255,.18), inset 0 -1px 0 rgba(0,0,0,.2), 0 6px 24px rgba(48,209,88,.12);
}
.result.show { display: block; animation: pop .42s cubic-bezier(.2,1.4,.4,1); }
@keyframes pop { from{opacity:0;transform:translateY(10px) scale(.96)} to{opacity:1;transform:none} }
.result .lab { font-size: 12px; color: var(--faint); }
.data {
  font-size: 22px; font-weight: 700; letter-spacing: 1.6px; color: var(--ok); margin: 9px 0 14px;
  font-variant-numeric: tabular-nums;
}
.copy {
  padding: 6px 14px; border-radius: 20px; border: .5px solid rgba(255,255,255,.3);
  background: rgba(255,255,255,.14); color: #fff; font-size: 12.5px; cursor: pointer; font-family: inherit;
  box-shadow: inset 0 1px 0 rgba(255,255,255,.22);
}
.copy:active { transform: scale(.96); }

/* 提示块 */
.tips { padding: 16px 20px; margin-top: 16px; font-size: 12px; line-height: 1.85; color: var(--faint); text-align: center; }

/* 后台 */
.hide { display: none; }
.stats { display: grid; grid-template-columns: repeat(4,1fr); gap: 12px; margin-bottom: 20px; }
.stat { padding: 16px 6px; text-align: center; }
.stat .n { font-size: 24px; font-weight: 700; letter-spacing: .5px; }
.stat .l { font-size: 11px; color: var(--faint); margin-top: 5px; }

.panel { padding: 22px; margin-bottom: 18px; }
.sec { font-size: 14.5px; font-weight: 600; color: rgba(255,255,255,.82); margin: 18px 0 12px; }
.sec:first-child { margin-top: 0; }
.row { display: flex; gap: 10px; margin-bottom: 10px; }
.row input { margin-bottom: 0; flex: 1; min-width: 0; padding: 13px 14px; border-radius: 14px; font-size: 14px; }

table { width: 100%; border-collapse: collapse; font-size: 13px; margin-top: 6px; }
th, td { padding: 11px 8px; text-align: left; border-bottom: .5px solid rgba(255,255,255,.1); }
th { font-size: 11.5px; color: var(--faint); font-weight: 500; }
tr:hover td { background: rgba(255,255,255,.035); }
.mini { padding: 5px 11px; border-radius: 9px; border: .5px solid rgba(255,255,255,.24); cursor: pointer;
  background: linear-gradient(140deg, rgba(255,255,255,.14), rgba(255,255,255,.04));
  color: #fff; font-size: 12px; margin-right: 5px; font-family: inherit; box-shadow: inset 0 1px 0 rgba(255,255,255,.2); }
.mini:active { transform: scale(.95); }
.mini.del { background: linear-gradient(140deg, rgba(255,90,80,.2), rgba(255,60,50,.1)); }
.mini + .mini { margin-left: 2px; }
.sec .mini { float: right; margin-top: -4px; }

/* 密码遮罩 —— 整个遮罩也是厚玻璃 */
.mask {
  position: fixed; inset: 0; z-index: 99; display: none;
  background: rgba(0,0,0,.55); backdrop-filter: blur(28px); -webkit-backdrop-filter: blur(28px);
  align-items: center; justify-content: center; padding: 24px;
}
.mask.show { display: flex; }
.pwd { padding: 34px 30px; width: 100%; max-width: 340px; text-align: center; }
.pwd .t { font-size: 21px; font-weight: 700; letter-spacing: 1px; }
.pwd input { margin: 22px 0 18px; text-align: center; letter-spacing: 4px; font-size: 19px; border-radius: 14px; }
.tip { font-size: 13px; min-height: 20px; color: var(--bad); }

@media (max-width: 600px) {
  .stats { grid-template-columns: repeat(2,1fr); }
  .row { flex-direction: column; gap: 12px; }
  .wrap.admin { padding: 10px; }
  th, td { padding: 9px 4px; font-size: 12px; }
}
</style>
</head>
<body>
<div class="orb3"></div>

<!-- 授权页 -->
<div id="auth-page" class="wrap">
  <header class="glass">
    <div class="logo">九一授权系统</div>
    <div class="sub">QQ交流群 141905528</div>
  </header>

  <div class="seg">
    <button class="on" data-t="auth" onclick="tab(this)">授权页</button>
    <button data-t="admin" onclick="tab(this)">后台管理</button>
  </div>

  <div class="glass" style="padding: 22px;">
    <input type="text" id="code-in" placeholder="在此输入授权码 (JY-XXX-XXX-XXX)">
    <button class="btn primary" onclick="doAuth()">立即授权</button>
    <button class="btn danger" onclick="clearAll()">清除数据</button>
    <div class="status" id="st">授权状态：等待输入…</div>
    <div class="result" id="res">
      <div class="lab">授权成功 · 您的数据号</div>
      <div class="data" id="data-out"></div>
      <button class="copy" onclick="copyData()">复制数据号</button>
    </div>
  </div>

  <div class="glass tips">
    🚀 请使用 https 访问才可使用复制功能<br>
    账号可无限授权，且用且珍惜<br>
    仅限从卡网出售的数据号才能重新授权
  </div>
</div>

<!-- 后台 -->
<div id="admin-page" class="wrap admin hide">
  <header class="glass">
    <div class="logo" style="font-size:22px">九一 · 后台管理</div>
  </header>

  <div class="seg">
    <button data-t="auth" onclick="tab(this)">授权页</button>
    <button class="on" data-t="admin" onclick="tab(this)">后台管理</button>
  </div>

  <div class="stats glass" style="padding:14px">
    <div class="stat"><div class="n" id="n-total">0</div><div class="l">授权码总数</div></div>
    <div class="stat"><div class="n" id="n-used">0</div><div class="l">总授权次数</div></div>
    <div class="stat"><div class="n" id="n-avail">0</div><div class="l">可用码数</div></div>
    <div class="stat"><div class="n" id="n-data">0</div><div class="l">下发数据号</div></div>
  </div>

  <div class="glass panel">
    <div class="sec">生成授权码 · JY-XXX-XXX-XXX</div>
    <div class="row">
      <input type="text" id="c-code" placeholder="留空自动生成">
      <input type="text" id="c-note" placeholder="备注">
    </div>
    <div class="row">
      <input type="number" id="c-times" placeholder="可用次数" value="999">
      <input type="date" id="c-exp">
    </div>
    <button class="btn primary" onclick="genCode()">生成授权码</button>
  </div>

  <div class="glass panel">
    <div class="sec">授权码列表</div>
    <input type="text" id="q" placeholder="搜索授权码 / 备注" oninput="render()">
    <table id="tb-code"></table>
  </div>

  <div class="glass panel">
    <div class="sec">授权记录<button class="mini" onclick="exportCSV()">导出 CSV</button></div>
    <table id="tb-log"></table>
  </div>
</div>

<!-- 密码门 -->
<div class="mask" id="mask">
  <div class="glass pwd">
    <div class="t">后台验证</div>
    <input type="password" id="pwd" placeholder="请输入密码" maxlength="12" autocomplete="off">
    <button class="btn primary" onclick="unlock()">进入</button>
    <div class="tip" id="tip"></div>
  </div>
</div>

<script>
var KEY = "jy_auth_v4";
var ADMIN_PWD = "789113";
var open = false;

var store = { codes:[], logs:[], dataCount:0 };
try { var s = JSON.parse(localStorage.getItem(KEY)); if(s) store = s; } catch(e){}
function save() { try { localStorage.setItem(KEY, JSON.stringify(store)); } catch(e){} }

function tab(btn) {
  var t = btn.dataset.t;
  if (t === "admin" && !open) { document.getElementById("mask").classList.add("show");
    setTimeout(function(){ document.getElementById("pwd").focus(); }, 60); return; }
  document.querySelectorAll(".seg").forEach(function(g){ g.querySelectorAll("button").forEach(function(b){
    b.classList.toggle("on", b.dataset.t === t); }); });
  document.getElementById("auth-page").classList.toggle("hide", t !== "auth");
  document.getElementById("admin-page").classList.toggle("hide", t !== "admin");
  if (t === "admin") render();
}

function unlock() {
  var v = document.getElementById("pwd").value;
  var tip = document.getElementById("tip");
  if (v === ADMIN_PWD) {
    tip.style.color = "var(--ok)"; tip.textContent = "验证通过";
    open = true;
    var m = document.getElementById("mask");
    setTimeout(function(){ m.classList.remove("show"); tip.textContent = ""; document.getElementById("pwd").value = "";
      document.querySelectorAll(".seg").forEach(function(g){ g.querySelectorAll("button").forEach(function(b){
        b.classList.toggle("on", b.dataset.t === "admin"); }); });
      document.getElementById("auth-page").classList.add("hide");
      document.getElementById("admin-page").classList.remove("hide"); render(); }, 380);
  } else {
    tip.textContent = "密码错误，请重试";
    var inp = document.getElementById("pwd"); inp.value = "";
    inp.style.transform = "translateX(7px)"; setTimeout(function(){ inp.style.transform = ""; }, 120);
  }
}
document.getElementById("pwd").addEventListener("keydown", function(e){ if(e.key === "Enter") unlock(); });

function C() { return "ABCDEFGHJKLMNPQRSTUVWXYZ23456789"; }
function seg(n) { var s = ""; for (var i = 0; i < n; i++) s += C()[Math.floor(Math.random()*C().length)]; return s; }
function genCodeStr() { return "JY-" + seg(3) + "-" + seg(3) + "-" + seg(3); }
function genDataStr() { var s = ""; for (var i = 0; i < 4; i++) s += (i ? "-" : "") + seg(4); return s; }

function doAuth() {
  var v = document.getElementById("code-in").value.trim().toUpperCase();
  var st = document.getElementById("st"), res = document.getElementById("res");
  res.classList.remove("show");
  if (!/^JY-[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}$/.test(v)) {
    st.textContent = "授权状态：格式错误，应为 JY-XXX-XXX-XXX"; st.style.color = "var(--bad)"; return;
  }
  var c = store.codes.filter(function(x){ return x.code === v; })[0];
  if (!c) { st.textContent = "授权状态：授权码不存在"; st.style.color = "var(--bad)"; return; }
  if (c.times <= c.used) { st.textContent = "授权状态：授权次数已用完"; st.style.color = "var(--bad)"; return; }
  if (c.exp && new Date(c.exp + "T23:59:59") < new Date()) { st.textContent = "授权状态：授权码已过期"; st.style.color = "var(--bad)"; return; }

  c.used++;
  var d = genDataStr(); c.lastData = d; store.dataCount++;
  store.logs.unshift({ time: new Date().toLocaleString(), code: v, data: d, ok: true });
  save();

  st.textContent = "授权状态：授权成功"; st.style.color = "var(--ok)";
  document.getElementById("data-out").textContent = d; res.classList.add("show");
}
function clearAll() {
  document.getElementById("code-in").value = "";
  var st = document.getElementById("st"); st.textContent = "授权状态：等待输入…"; st.style.color = "var(--dim)";
  document.getElementById("res").classList.remove("show");
}
function copyData() {
  var t = document.getElementById("data-out").textContent;
  if (navigator.clipboard) navigator.clipboard.writeText(t).then(function(){ alert("已复制：" + t); }, function(){ alert(t); });
  else alert(t);
}

function genCode() {
  var code = document.getElementById("c-code").value.trim().toUpperCase();
  if (!code) code = genCodeStr();
  else if (!/^JY-[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}$/.test(code)) { alert("格式错误，应为 JY-XXX-XXX-XXX"); return; }
  if (store.codes.some(function(x){ return x.code === code; })) { alert("该授权码已存在"); return; }
  store.codes.push({ code: code, note: document.getElementById("c-note").value.trim(),
    times: parseInt(document.getElementById("c-times").value, 10) || 999, used: 0,
    exp: document.getElementById("c-exp").value || null, lastData: "" });
  save(); render();
  document.getElementById("c-code").value = ""; document.getElementById("c-note").value = "";
}
function render() {
  document.getElementById("n-total").textContent = store.codes.length;
  document.getElementById("n-used").textContent = store.codes.reduce(function(a,b){ return a + b.used; }, 0);
  document.getElementById("n-avail").textContent = store.codes.filter(function(x){
    return x.times > x.used && (!x.exp || new Date(x.exp + "T23:59:59") >= new Date()); }).length;
  document.getElementById("n-data").textContent = store.dataCount;

  var k = document.getElementById("q").value.trim().toLowerCase();
  var rows = store.codes.filter(function(x){ return (x.code + x.note).toLowerCase().indexOf(k) > -1; });
  var h = '<tr><th>授权码</th><th>备注</th><th>次数</th><th>已用</th><th>数据号</th><th>状态</th><th>操作</th></tr>';
  var html = rows.map(function(x, i) {
    var exp = x.exp && new Date(x.exp + "T23:59:59") < new Date();
    var s = exp ? '<span style="color:var(--bad)">过期</span>' : x.used >= x.times ? '<span style="color:var(--bad)">用完</span>' : '<span style="color:var(--ok)">正常</span>';
    return '<tr><td>' + x.code + '</td><td>' + (x.note || "-") + '</td><td>' + x.times + '</td><td>' + x.used +
      '</td><td style="font-size:11px">' + (x.lastData || "-") + '</td><td>' + s + '</td>' +
      '<td><button class="mini" onclick="cp(\'' + x.code + '\')">复制</button><button class="mini del" onclick="delCode(' + i + ')">删除</button></td></tr>';
  }).join("");
  document.getElementById("tb-code").innerHTML = h + (html || '<tr><td colspan="7" style="text-align:center;color:var(--faint)">暂无数据，先去生成一个吧</td></tr>');

  var lh = '<tr><th>时间</th><th>授权码</th><th>数据号</th><th>结果</th></tr>';
  var lhtml = store.logs.map(function(x) {
    return '<tr><td style="white-space:nowrap">' + x.time + '</td><td>' + x.code + '</td><td style="font-size:11px">' + x.data +
      '</td><td><span style="color:var(--ok)">成功</span></td></tr>';
  }).join("");
  document.getElementById("tb-log").innerHTML = lh + (lhtml || '<tr><td colspan="4" style="text-align:center;color:var(--faint)">暂无授权记录</td></tr>');
}
function cp(t) { if(navigator.clipboard) navigator.clipboard.writeText(t).then(function(){ alert("已复制：" + t); }, function(){ alert(t); }); else alert(t); }
function delCode(i) { if(confirm("确定删除该授权码？")) { store.codes.splice(i,1); save(); render(); } }
function exportCSV() {
  var csv = "时间,授权码,数据号,结果\n" + store.logs.map(function(x){ return '"' + x.time + '","' + x.code + '","' + x.data + '","成功"'; }).join("\n");
  var a = document.createElement("a"); a.href = URL.createObjectURL(new Blob(["\ufeff" + csv], { type: "text/csv" }));
  a.download = "授权记录.csv"; a.click();
}

(function init() {
  if (!store.codes.length) { store.codes.push({ code: "JY-DEM-O01-TST", note: "测试码", times: 999, used: 0, exp: null, lastData: "" }); save(); }
})();
</script>
</body>
</html>
