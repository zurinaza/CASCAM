# CASCAM
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Course Assessment Summary</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500;600&family=IBM+Plex+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --navy:#0a2342; --navy-2:#13315c; --navy-3:#1b4272;
  --blue:#1d4e89; --blue-2:#2f6fb0; --blue-soft:#dbe8f6; --blue-line:#a9c4e0;
  --ground:#eaf0f7; --surface:#ffffff; --surface-2:#f4f8fd; --surface-3:#e8f0f9;
  --ink:#0c1d33; --ink-2:#3a5570; --ink-3:#6b849c;
  --rule:#c2d3e6; --rule-soft:#dee9f4;
  --yes:#0f6b52; --yes-bg:#daeee7;
  --no:#a8352a; --no-bg:#f8e2df;
  --warn:#8a6206; --warn-bg:#faeed3;
  --action:#1d4e89; --action-bg:#dbe8f6; --action-ink:#ffffff;
  --head:#13315c; --rulemark:#13315c;
  --mast:#0a2342; --mast-ink:#d4e3f4; --mast-ink-2:#8aa8c8; --mast-rule:#1b3c63;
  --focus:#2f6fb0;
  --shadow:0 1px 2px rgba(10,35,66,.10), 0 8px 22px -14px rgba(10,35,66,.35);
  --sans:"IBM Plex Sans",ui-sans-serif,system-ui,-apple-system,"Segoe UI",sans-serif;
  --mono:"IBM Plex Mono",ui-monospace,"SF Mono",Menlo,Consolas,monospace;
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){
    --navy:#050f1d; --navy-2:#0e2540; --navy-3:#17385e;
    --ground:#071320; --surface:#0f2137; --surface-2:#142b45; --surface-3:#1b3552;
    --ink:#dbe8f6; --ink-2:#a6bdd6; --ink-3:#7794b3;
    --rule:#264b73; --rule-soft:#1e3a59;
    --yes:#48b494; --yes-bg:#0d3229; --no:#e08a79; --no-bg:#3a1c17;
    --warn:#d7a53f; --warn-bg:#352a12;
    --action:#7fb2e0; --action-bg:#14304e; --action-ink:#05131f;
    --blue-soft:#14304e; --blue-line:#2c5580; --blue-2:#4b8ec9;
    --head:#dbe8f6; --rulemark:#8fb8dd;
    --head:#dbe8f6; --rulemark:#8fb8dd;
  --mast:#040d18; --mast-ink:#cfe0f2; --mast-ink-2:#7d9ab8; --mast-rule:#1c365a;
    --focus:#6fa8dc;
    --shadow:0 1px 2px rgba(0,0,0,.5), 0 10px 26px -16px rgba(0,0,0,.8);
  }
}
:root[data-theme="dark"]{
  --ground:#071320; --surface:#0f2137; --surface-2:#142b45; --surface-3:#1b3552;
  --ink:#dbe8f6; --ink-2:#a6bdd6; --ink-3:#7794b3;
  --rule:#264b73; --rule-soft:#1e3a59;
  --yes:#48b494; --yes-bg:#0d3229; --no:#e08a79; --no-bg:#3a1c17;
  --warn:#d7a53f; --warn-bg:#352a12;
  --action:#7fb2e0; --action-bg:#14304e; --action-ink:#05131f;
  --blue-soft:#14304e; --blue-line:#2c5580; --blue-2:#4b8ec9;
  --head:#dbe8f6; --rulemark:#8fb8dd;
  --mast:#040d18; --mast-ink:#cfe0f2; --mast-ink-2:#7d9ab8; --mast-rule:#1c365a;
  --focus:#6fa8dc;
  --shadow:0 1px 2px rgba(0,0,0,.5), 0 10px 26px -16px rgba(0,0,0,.8);
}

*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{background:var(--ground); color:var(--ink); font-family:var(--sans); font-size:15px;
  line-height:1.5; -webkit-text-size-adjust:100%; font-feature-settings:"tnum" 1,"lnum" 1}
h1,h2,h3,h4{margin:0; font-weight:600; letter-spacing:-.011em; line-height:1.25}
p{margin:0 0 .7em}
a{color:var(--action)}
button,input,select,textarea{font:inherit; color:inherit}
:focus-visible{outline:2px solid var(--focus); outline-offset:2px; border-radius:2px}
.num{font-family:var(--mono); font-variant-numeric:tabular-nums}

/* ---------- masthead ---------- */
.mast{background:var(--mast); color:var(--mast-ink); border-bottom:3px solid var(--blue-2)}
.mast-in{max-width:1240px; margin:0 auto; padding:0 18px}
.mast-top{display:flex; align-items:center; gap:14px; flex-wrap:wrap; padding:11px 0 10px}
.crest{height:30px; width:auto; display:block; background:#fff; padding:3px 5px; border-radius:3px}
.brand{display:flex; align-items:baseline; gap:9px}
.brand b{font-size:15px; font-weight:700; color:#fff}
.brand span{font-size:11.5px; color:var(--mast-ink-2)}
.picklab{font-size:11.5px; color:var(--mast-ink-2); margin-right:-6px}
.course-pick{background:var(--mast-rule); color:var(--mast-ink); border:1px solid transparent;
  border-radius:5px; padding:6px 30px 6px 10px; max-width:260px; font-size:13.5px; appearance:none;
  background-image:linear-gradient(45deg,transparent 50%,currentColor 50%),linear-gradient(135deg,currentColor 50%,transparent 50%);
  background-position:calc(100% - 15px) 14px, calc(100% - 10px) 14px;
  background-size:5px 5px,5px 5px; background-repeat:no-repeat}
.mast-right{margin-left:auto; display:flex; align-items:center; gap:8px}
.savestate{font-size:11.5px; color:var(--mast-ink-2); font-family:var(--mono); white-space:nowrap}
.savestate.busy{color:#e8c97a} .savestate.err{color:#eda08c}
.ghost{background:transparent; border:1px solid var(--mast-rule); color:var(--mast-ink);
  border-radius:5px; padding:5px 10px; font-size:12.5px; cursor:pointer}
.ghost:hover{background:var(--mast-rule)}
.mast-nav{display:flex; align-items:center; gap:14px}
.mast-nav .tabs{flex:1; min-width:0}
.mast-nav .savestate{flex:none; padding-bottom:2px}
.tabs{display:flex; gap:2px; overflow-x:auto; scrollbar-width:none}
.tabs::-webkit-scrollbar{display:none}
.tab{background:none; border:0; border-bottom:3px solid transparent; color:var(--mast-ink-2);
  padding:9px 13px 7px; cursor:pointer; font-size:13.5px; white-space:nowrap; margin-bottom:-3px}
.tab:hover{color:#fff}
.tab[aria-selected="true"]{color:#fff; border-bottom-color:var(--blue-2)}
.tab .cnt{font-family:var(--mono); font-size:11px; opacity:.7; margin-left:5px}

/* ---------- layout ---------- */
.wrap{max-width:1240px; margin:0 auto; padding:22px 18px 80px}
.panel{background:var(--surface); border:1px solid var(--rule); border-radius:8px;
  box-shadow:var(--shadow); margin-bottom:18px; overflow:hidden}
.panel > header{display:flex; align-items:baseline; gap:12px; flex-wrap:wrap;
  padding:12px 16px; border-bottom:1px solid var(--rule-soft); background:var(--surface-2)}
.panel > header h2{font-size:15px; color:var(--head)}
.panel > header .note{font-size:12.5px; color:var(--ink-3); margin-left:auto}
.body{padding:16px}
.body.flush{padding:0}
.hint{font-size:12.5px; color:var(--ink-3); margin:0 0 12px; max-width:70ch}
.row{display:flex; gap:10px; flex-wrap:wrap; align-items:center}
.spacer{flex:1}
.sectag{display:inline-flex; align-items:center; justify-content:center; width:22px; height:22px;
  border-radius:3px; background:var(--blue-2); color:#fff; font-size:12px; font-weight:600; flex:none}

/* ---------- controls ---------- */
label.f{display:block; font-size:12px; color:var(--ink-3); margin-bottom:4px}
input[type=text],input[type=number],select,textarea{width:100%; background:var(--surface);
  border:1px solid var(--rule); border-radius:5px; padding:7px 9px; font-size:14px}
input[type=number]{font-family:var(--mono)}
textarea{resize:vertical; font-size:13.5px; line-height:1.5}
input:disabled{background:var(--surface-3); color:var(--ink-3)}
.grid2{display:grid; grid-template-columns:repeat(auto-fit,minmax(210px,1fr)); gap:12px}
.btn{background:var(--action); color:var(--action-ink); border:1px solid transparent;
  border-radius:5px; padding:7px 13px; cursor:pointer; font-size:13.5px; font-weight:500}
.btn:hover{filter:brightness(1.14)}
.btn.sec{background:var(--surface); color:var(--head); border-color:var(--rule)}
.btn.sec:hover{background:var(--blue-soft); filter:none}
.btn.danger{background:var(--surface); color:var(--no); border-color:var(--rule)}
.btn.danger:hover{background:var(--no-bg)}
.btn:disabled{opacity:.45; cursor:not-allowed; filter:none}
.btn.sm{padding:4px 9px; font-size:12.5px}
.iconbtn{background:none;border:1px solid var(--rule);border-radius:5px;color:var(--ink-3);
  width:26px;height:26px;line-height:1;cursor:pointer;padding:0;font-size:15px}
.iconbtn:hover{color:var(--no); border-color:var(--no)}

/* ---------- tables ---------- */
.scroll{overflow:auto; max-height:min(70vh,760px)}
table{border-collapse:separate; border-spacing:0; width:100%; font-size:13.5px}
th,td{padding:6px 9px; text-align:left; border-bottom:1px solid var(--rule-soft); white-space:nowrap}
thead th{position:sticky; top:0; z-index:3; background:var(--surface-2); color:var(--head);
  font-weight:600; font-size:12px; border-bottom:1px solid var(--rule); vertical-align:bottom}
thead th .sub{display:block; font-weight:400; font-size:10.5px; color:var(--ink-3); font-family:var(--mono)}
tbody tr:hover td{background:var(--surface-2)}
td.n,th.n{text-align:right; font-family:var(--mono); font-variant-numeric:tabular-nums}
.stick1{position:sticky; left:0; z-index:2; background:var(--surface)}
.stick2{position:sticky; left:44px; z-index:2; background:var(--surface)}
thead .stick1,thead .stick2{z-index:4; background:var(--surface-2)}
tbody tr:hover .stick1,tbody tr:hover .stick2{background:var(--surface-2)}
.divide{border-left:1px solid var(--rule)}
tfoot td{position:sticky; background:var(--surface-2); border-top:1px solid var(--rule);
  border-bottom:0; font-size:12.5px; z-index:2}
tfoot tr:first-child td{bottom:27px}
tfoot tr:last-child td{bottom:0; border-top-color:var(--rule-soft)}
tfoot tr:only-child td{bottom:0; border-top-color:var(--rule)}
.cellin{width:62px; border:1px solid transparent; background:transparent; border-radius:3px;
  padding:3px 5px; text-align:right; font-family:var(--mono); font-size:13px}
.cellin:hover{border-color:var(--rule)}
.cellin:focus{border-color:var(--focus); background:var(--surface); outline:none; box-shadow:0 0 0 2px var(--action-bg)}
.cellin.bad{background:var(--no-bg); color:var(--no); border-color:var(--no)}
.txtin{width:100%; min-width:120px; border:1px solid transparent; background:transparent;
  border-radius:3px; padding:3px 5px; font-size:13px}
.txtin:hover{border-color:var(--rule)}
.txtin:focus{border-color:var(--focus); background:var(--surface); outline:none}

/* ---------- assessment cards ---------- */
.acard{border:1px solid var(--rule); border-left:4px solid var(--blue-2); border-radius:7px;
  padding:11px 13px; margin-bottom:10px; background:var(--surface)}
.acard.bad{border-left-color:var(--no); background:linear-gradient(90deg,var(--no-bg) 0%,var(--surface) 34%)}
.atop{display:flex; gap:9px; align-items:center; flex-wrap:wrap; margin-bottom:9px}
.atop .aname{flex:1 1 200px; min-width:160px; border:1px solid var(--rule); border-radius:5px;
  padding:5px 8px; font-size:14px; font-weight:500; background:var(--surface)}
.atop select{width:auto; min-width:120px; padding:5px 8px; font-size:13px}
.amark{display:flex; align-items:center; gap:6px; font-size:12px; color:var(--ink-3); white-space:nowrap}
.amark input{width:66px; border:1px solid var(--rule); text-align:right}
.arow{display:flex; gap:9px; align-items:flex-start; padding:3px 0}
.alab{width:34px; flex:none; font-size:11px; color:var(--ink-3); font-family:var(--mono); padding-top:4px}
.chips{display:flex; flex-wrap:wrap; gap:5px; flex:1}
.chip{border:1px solid var(--rule); background:var(--surface); color:var(--ink-2); border-radius:999px;
  padding:2px 10px; font-size:11.5px; font-family:var(--mono); cursor:pointer; line-height:1.55}
.chip:hover{border-color:var(--blue-2); color:var(--head)}
.chip[aria-pressed="true"]{background:var(--action); border-color:var(--action); color:var(--action-ink); font-weight:500}
.chipnote{font-size:11.5px; color:var(--no); padding-top:4px}
.chipnote.mute{color:var(--ink-3)}

/* ---------- mapping chain ---------- */
.cblock{border:1px solid var(--rule); border-left:4px solid var(--blue-2); border-radius:7px;
  padding:11px 13px; margin-bottom:10px; background:var(--surface)}
.cblock.bad{border-left-color:var(--no)}
.chead{display:flex; gap:10px; align-items:baseline; flex-wrap:wrap;
  padding-bottom:7px; border-bottom:1px solid var(--rule-soft)}
.chead b{font-size:14px; color:var(--head)}
.chead .cdesc{font-size:12.5px; color:var(--ink-2); flex:1 1 200px; min-width:0}
.chead .cnum{font-family:var(--mono); font-size:11.5px; color:var(--ink-3); white-space:nowrap}
.clink{list-style:none; margin:6px 0 0; padding:0}
.clink li{display:flex; gap:10px; align-items:center; flex-wrap:wrap; padding:4px 0; font-size:13px}
.clink .anm{font-weight:500; min-width:130px}
.clink .adel{font-size:11.5px; color:var(--ink-3)}
.clink .apc{font-family:var(--mono); font-size:12px; color:var(--ink-3); min-width:42px; text-align:right}
.clink .arrow{color:var(--ink-3); font-size:14px}
.pill{display:inline-block; background:var(--action-bg); color:var(--head); border-radius:999px;
  padding:1px 9px; font-size:11px; font-family:var(--mono); margin-right:4px}
.pill.miss{background:var(--no-bg); color:var(--no); font-family:var(--sans)}
.cfoot{margin-top:7px; padding-top:7px; border-top:1px solid var(--rule-soft);
  font-size:12px; color:var(--ink-3)}

/* ---------- mapping matrix ---------- */
.map th.rot{height:74px; vertical-align:bottom; padding-bottom:8px; width:42px; white-space:nowrap}
.map th.rot > div{writing-mode:vertical-rl; transform:rotate(180deg); font-size:12px; font-weight:600;
  text-align:left; line-height:1.1}
.map td.chk{text-align:center; width:42px}
.map input[type=checkbox]{width:16px;height:16px;accent-color:var(--action);cursor:pointer}
.map tbody tr td:first-child{font-weight:500}
.tot-cell{font-family:var(--mono); font-size:12px; color:var(--ink-3)}
tr.off td{opacity:.42}

/* ---------- attainment strip ---------- */
.gauge{position:relative; padding:6px 0 2px}
.gline{position:absolute; top:0; bottom:22px; width:0; border-left:2px dashed var(--rulemark);
  z-index:2; pointer-events:none; left:calc(78px + (100% - 216px) * var(--t,.6))}
.gline b{position:absolute; top:-3px; left:6px; font-size:11px; font-family:var(--mono);
  color:var(--rulemark); background:var(--surface); padding:0 4px; white-space:nowrap; font-weight:500}
.grow{display:grid; grid-template-columns:68px 1fr 128px; align-items:center; gap:10px; padding:5px 0}
.gname{font-size:13px; font-weight:600}
.gname small{display:block; font-weight:400; font-size:10.5px; color:var(--ink-3); font-family:var(--mono)}
.gtrack{height:22px; background:var(--surface-3); border-radius:2px; position:relative; overflow:hidden}
.gfill{position:absolute; inset:0 auto 0 0; border-radius:2px 0 0 2px}
.gfill.ok{background:var(--yes)} .gfill.bad{background:var(--no)}
.gmark{position:absolute; top:-2px; bottom:-2px; width:2px; background:var(--rulemark); opacity:.8}
.gval{font-family:var(--mono); font-size:13px; text-align:right; white-space:nowrap}
.gval .tag{display:inline-block; min-width:62px; text-align:center; margin-left:8px; border-radius:3px;
  padding:1px 6px; font-size:11.5px; font-weight:600; font-family:var(--sans)}
.tag.ok{background:var(--yes-bg); color:var(--yes)}
.tag.bad{background:var(--no-bg); color:var(--no)}
.gscale{display:flex; justify-content:space-between; font-size:10.5px; color:var(--ink-3);
  font-family:var(--mono); margin-left:78px; margin-right:138px; padding-top:2px}

/* ---------- stats / issues ---------- */
.stats{display:grid; grid-template-columns:repeat(auto-fit,minmax(130px,1fr)); gap:1px;
  background:var(--rule-soft); border-top:1px solid var(--rule-soft)}
.stat{background:var(--surface); padding:12px 14px}
.stat b{display:block; font-family:var(--mono); font-size:21px; font-weight:500; letter-spacing:-.02em}
.stat span{font-size:11.5px; color:var(--ink-3)}
.issues{list-style:none; margin:0; padding:0; font-size:13px}
.issues li{display:flex; gap:9px; padding:8px 16px; border-bottom:1px solid var(--rule-soft); align-items:baseline}
.issues li:last-child{border-bottom:0}
.issues .dot{width:7px;height:7px;border-radius:50%;flex:none;transform:translateY(-1px)}
.issues .err .dot{background:var(--no)} .issues .warn .dot{background:var(--warn)}
.issues .ok{color:var(--ink-3)} .issues .ok .dot{background:var(--yes)}
.issues .where{margin-left:auto; color:var(--ink-3); font-size:11.5px; font-family:var(--mono); white-space:nowrap}
.gradebar{display:flex; height:26px; border-radius:3px; overflow:hidden; border:1px solid var(--rule)}
.gradebar div{display:flex;align-items:center;justify-content:center;font-size:10.5px;
  font-family:var(--mono); color:#fff; min-width:0; overflow:hidden}
.gradekey{display:flex;flex-wrap:wrap;gap:10px;font-size:11.5px;color:var(--ink-3);margin-top:7px;font-family:var(--mono)}
.gradekey i{width:9px;height:9px;border-radius:2px;display:inline-block;margin-right:4px}

/* ---------- home ---------- */
.hero{background:linear-gradient(160deg,var(--navy) 0%,var(--navy-2) 58%,var(--navy-3) 100%);
  color:#eaf2fb; border-radius:10px; padding:34px 32px; margin-bottom:20px; position:relative; overflow:hidden}
.hero::after{content:""; position:absolute; right:-70px; top:-70px; width:280px; height:280px;
  border-radius:50%; border:1px solid rgba(255,255,255,.08); box-shadow:0 0 0 34px rgba(255,255,255,.03)}
.hero-crest{background:#fff; padding:8px 12px; border-radius:5px; display:inline-block; margin-bottom:20px}
.hero-crest img{height:42px; display:block}
.hero h1{font-size:clamp(25px,4.2vw,38px); font-weight:700; letter-spacing:-.02em; color:#fff; max-width:17ch}
.hero .kicker{font-size:12.5px; color:#9dbcdd; margin-bottom:9px; font-family:var(--mono)}
.hero p.lede{margin:14px 0 0; max-width:56ch; color:#c5daf0; font-size:14.5px}
.credit{display:flex; align-items:center; gap:16px; margin-top:26px; padding:16px 18px;
  border-top:2px solid var(--blue-2); background:var(--surface); border-radius:0 0 8px 8px;
  border:1px solid var(--rule); border-top-width:2px; border-radius:8px; box-shadow:var(--shadow)}
.credit img{height:40px; width:auto; background:#fff; padding:4px 7px; border-radius:4px; flex:none}
.credit div{display:flex; flex-direction:column; min-width:0}
.credit b{font-size:14px; color:var(--head); font-weight:600}
.credit span{font-size:12.5px; color:var(--ink-3)}
.clist{display:grid; grid-template-columns:repeat(auto-fill,minmax(250px,1fr)); gap:12px}
.ccard{position:relative; display:block; width:100%; text-align:left; background:var(--surface);
  border:1px solid var(--rule); border-left:4px solid var(--blue-2); border-radius:7px;
  padding:13px 38px 13px 15px; cursor:pointer}
.ccdel{position:absolute; top:9px; right:9px; width:24px; height:24px; padding:0; line-height:1;
  border:1px solid transparent; border-radius:5px; background:none; color:var(--ink-3);
  cursor:pointer; font-size:15px; opacity:0}
.ccard:hover .ccdel, .ccard:focus-within .ccdel{opacity:1}
.ccdel:hover{color:var(--no); border-color:var(--no); background:var(--no-bg)}
.ccard:hover{border-color:var(--blue-2); background:var(--surface-2)}
.ccard b{display:block; font-size:14.5px; color:var(--head)}
.ccard span{display:block; font-size:12px; color:var(--ink-3); margin-top:3px}
.ccard .st{display:flex; gap:12px; margin-top:9px; font-size:11.5px; font-family:var(--mono); color:var(--ink-2)}
.empty{text-align:center; padding:52px 20px; max-width:52ch; margin:0 auto}
.empty h2{font-size:19px; margin-bottom:8px}
.empty p{color:var(--ink-2); font-size:14px}

/* ---------- printable documents ---------- */
.paper{background:#fff; color:#000; border:1px solid var(--rule); border-radius:6px;
  box-shadow:var(--shadow); margin:0 auto 20px; padding:14mm 12mm; max-width:208mm;
  font-size:10.5px; line-height:1.38; font-family:var(--sans)}
.paper *{border-color:#000}
.paper h3{font-size:11px; margin:0 0 5px}
.paper table{border-collapse:collapse; width:100%; font-size:9.6px; margin:0 0 9px}
.paper th,.paper td{border:1px solid #000; padding:3px 5px; vertical-align:top;
  white-space:normal; text-align:left; background:none; position:static; color:#000}
.paper thead th{position:static; background:#eef2f7; color:#000; font-size:9.6px; border-bottom:1px solid #000}
.paper tbody tr:hover td{background:none}
.paper .n{text-align:right; font-family:var(--mono)}
.paper .c{text-align:center}
.ph{display:flex; border:1px solid #000; margin-bottom:10px}
.ph .logo{width:130px; flex:none; border-right:1px solid #000; display:flex; align-items:center; justify-content:center; padding:6px}
.ph .logo img{width:100%; height:auto}
.ph .txt{flex:1; display:flex; flex-direction:column}
.ph .t1{border-bottom:1px solid #000; padding:6px 8px; text-align:center; font-size:10px; font-weight:700; line-height:1.35}
.ph .t1 .doc{display:block; font-weight:400; font-size:9.4px; margin-top:2px}
.ph .t2{padding:8px; text-align:center; font-weight:700; font-size:11.5px}
.ph .t2 i{display:block; font-weight:400}
.pf{margin-top:14px; font-size:9px; font-family:var(--mono); color:#000; border-top:1px solid #000; padding-top:5px}
.pf span{display:inline-block; min-width:170px}
.hl{background:#fff8a8}
.shade-b,.shade-o,.shade-g{color:#0c1d33}
.shade-b{background:#dbe8f6} .shade-o{background:#f7e0cf} .shade-g{background:#d9ecd6}
.cas-sec{display:flex; border:1px solid #000; border-bottom:0}
.cas-sec:last-of-type{border-bottom:1px solid #000}
.cas-sec > .lt{width:26px; flex:none; border-right:1px solid #000; text-align:center;
  font-weight:700; padding:6px 0; font-size:10.5px}
.cas-sec > .ct{flex:1; padding:7px 9px; min-width:0}
.cas-sec p{margin:0 0 5px}
.cas-sec p:last-child{margin-bottom:0}
.sign{display:grid; grid-template-columns:1fr 1fr; gap:40px; margin-top:26px; font-size:10px}
.sign .line{border-bottom:1px dotted #000; height:40px; margin-bottom:4px}
.runner{border-collapse:collapse; width:100%; margin:0; font-size:inherit}
.runner > thead > tr > th, .runner > tbody > tr > td{border:0; padding:0; background:none; white-space:normal}
.runner > thead > tr > th{font-weight:400; text-align:left; position:static}
.runner > thead{display:table-header-group}
.docbar{position:sticky; top:0; z-index:5; background:var(--ground); padding:10px 0 12px; margin-bottom:4px}

@media (max-width:700px){ .savestate{display:none} }
@media (max-width:860px){ .picklab{display:none} }
@media (max-width:640px){
  .wrap{padding:14px 10px 70px}
  .body{padding:13px}
  .hero{padding:24px 18px}
  .grow{grid-template-columns:56px 1fr; gap:8px}
  .gval{grid-column:2; text-align:left}
  .gscale{margin:0 0 0 64px}
  .gline{left:calc(64px + (100% - 64px) * var(--t,.6))}
  .paper{padding:10px; font-size:10px}
  .sign{grid-template-columns:1fr; gap:20px}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important; animation:none!important}}

/* ---------- dialog / toast ---------- */
dialog{border:1px solid var(--rule); border-radius:9px; background:var(--surface); color:var(--ink);
  padding:0; max-width:600px; width:calc(100% - 32px); box-shadow:0 20px 50px -20px rgba(10,35,66,.6)}
dialog::backdrop{background:rgba(10,35,66,.5)}
dialog header{padding:13px 16px; border-bottom:1px solid var(--rule-soft); font-weight:600; background:var(--surface-2)}
dialog .body{padding:16px}
dialog footer{padding:12px 16px; border-top:1px solid var(--rule-soft); display:flex; gap:8px;
  justify-content:flex-end; background:var(--surface-2)}
.opts{display:flex; flex-direction:column; gap:2px; margin:0 0 4px}
.opt{display:flex; gap:10px; align-items:flex-start; padding:9px 11px; border:1px solid var(--rule);
  border-radius:6px; cursor:pointer; background:var(--surface)}
.opt:hover{border-color:var(--blue-2); background:var(--surface-2)}
.opt input{margin:3px 0 0; accent-color:var(--action); flex:none}
.opt b{display:block; font-size:13.5px; font-weight:600}
.opt span{display:block; font-size:12px; color:var(--ink-3); margin-top:1px}
.opt.warn{border-color:var(--no)}
.opt.warn b{color:var(--no)}
#toast{position:fixed; left:50%; bottom:22px; transform:translateX(-50%) translateY(10px);
  background:var(--navy); color:#e4eefa; padding:9px 16px; border-radius:6px; font-size:13px;
  opacity:0; pointer-events:none; transition:opacity .16s, transform .16s; z-index:99; max-width:90vw}
#toast.on{opacity:1; transform:translateX(-50%) translateY(0)}

@media print{
  @page{size:A4; margin:11mm}
  .mast,.noprint,.docbar{display:none!important}
  body{background:#fff}
  .wrap{padding:0; max-width:none}
  .paper{border:0; box-shadow:none; padding:0; max-width:none; margin:0; font-size:9.6px}
  .paper table{page-break-inside:auto}
  tr{page-break-inside:avoid}
  .pagebreak{page-break-before:always}
  .paper .ph{position:running(hdr)}
}
</style>
</head>
<body>
<header class="mast noprint">
  <div class="mast-in">
    <div class="mast-top">
      <img class="crest" id="crestImg" alt="Universiti Putra Malaysia">
      <span class="brand"><b>Course Assessment Summary</b><span>CLO &amp; EAC attainment</span></span>
      <span class="picklab" id="pickLab">Editing</span>
      <select id="coursePick" class="course-pick" aria-label="Course being edited"></select>
      <button class="ghost" id="newCourse">New course</button>
      <button class="ghost" id="resetTop">Reset&hellip;</button>
      <span class="mast-right">
        <button class="ghost" id="themeBtn" aria-label="Switch colour theme">Theme</button>
      </span>
    </div>
    <div class="mast-nav">
    <nav class="tabs" role="tablist" id="tabs">
      <button class="tab" role="tab" data-view="home">Home</button>
      <button class="tab" role="tab" data-view="setup">Setup</button>
      <button class="tab" role="tab" data-view="marks">Marks<span class="cnt" id="tabCount"></span></button>
      <button class="tab" role="tab" data-view="analysis">Attainment</button>
      <button class="tab" role="tab" data-view="cas">CAS form</button>
      <button class="tab" role="tab" data-view="print">Print</button>
      <button class="tab" role="tab" data-view="data">Data</button>
    </nav>
      <span class="savestate" id="saveState">&nbsp;</span>
    </div>
  </div>
</header>

<main class="wrap" id="app"></main>
<div id="toast" role="status" aria-live="polite"></div>

<dialog id="dlg">
  <header id="dlgTitle">Dialog</header>
  <div class="body" id="dlgBody"></div>
  <footer id="dlgFoot"></footer>
</dialog>
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<script>
/* ============================================================
   Course Assessment Summary — Faculty of Engineering, UPM
   Calculation engine, EAC catalogue and storage.

   Attainment, per the CAM method:
     outcome full mark  = SUM(full marks of the assessments mapped to it)
     student outcome %  = ROUND(SUM(mapped marks) / outcome full mark * 100, 2)
     Y                  = students reaching the student threshold
     Z                  = ROUND(Y / students counted * 100, 2)
     status             = Y when Z reaches that outcome's required minimum for this semester
   ============================================================ */
"use strict";

const $  = (s, r) => (r || document).querySelector(s);
const $$ = (s, r) => Array.from((r || document).querySelectorAll(s));
const uid = p => (p || "id") + "_" + Math.random().toString(36).slice(2, 9);
const esc = v => String(v == null ? "" : v).replace(/[&<>"']/g, c =>
  ({ "&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;", "'": "&#39;" }[c]));
const nl2br = v => esc(v).replace(/\n/g, "<br>");
const r2 = n => Math.round((n + Number.EPSILON) * 100) / 100;
const fmt = (n, d) => (n == null || !isFinite(n)) ? "—" : n.toFixed(d == null ? 2 : d);
const clamp = (n, lo, hi) => Math.min(hi, Math.max(lo, n));

function toast(msg) {
  const t = $("#toast");
  t.textContent = msg; t.classList.add("on");
  clearTimeout(toast._t); toast._t = setTimeout(() => t.classList.remove("on"), 2600);
}

/* ---------------- the 11 EAC programme outcomes, 2021–2025 curriculum ---------------- */

const EAC_CATALOGUE = [
  ["EAC1", "C", "Engineering Knowledge", "WK1 to WK4", "Apply knowledge of mathematics, science, engineering fundamentals and an engineering specialization to develop solutions of complex engineering problems;"],
  ["EAC2", "C", "Problem Analysis", "WK1 to WK4", "Identify, formulate, research literature and analyse complex engineering problems reaching substantiated conclusions using first principles of mathematics, natural sciences and engineering sciences with holistic considerations for sustainable development;"],
  ["EAC3", "C", "Design/Development of Solution", "WK5", "Design creative solutions for complex engineering problems and design systems, components or processes to meet identified needs with appropriate consideration for public health and safety, whole-life cost, net zero carbon as well as resource, cultural, societal, and environmental considerations;"],
  ["EAC4", "C", "Investigation", "WK8", "Conduct investigation of complex problems using research-based methods including research-based knowledge, including design of experiments, analysis and interpretation of data, and synthesis of information to provide valid conclusions;"],
  ["EAC5", "P", "Tool Usage", "WK2 and WK6", "Create, select and apply, and recognize limitation of appropriate techniques, resources, and modern engineering and IT tools, including prediction and modelling, to complex engineering problems;"],
  ["EAC6", "C", "The Engineer and the World", "WK1, WK5 and WK7", "Analyze and evaluate sustainable development impacts to: society, the economy, sustainability, health and safety, legal frameworks, and the environment, in solving complex engineering problems;"],
  ["EAC7", "C", "Ethics", "WK9", "Apply ethical principles and commit to professional ethics and norms of engineering practice and adhere to relevant national and international laws. Demonstrate an understanding of the need for diversity and inclusion;"],
  ["EAC8", "C", "Individual and Team Work", "WK9", "Function effectively as an individual, and as a member or leader in diverse and inclusive teams and in multidisciplinary, face-to-face, remote and distributed settings;"],
  ["EAC9", "A", "Communication", "", "Communicate effectively and inclusively on complex engineering activities with the engineering community and with society at large, such as being able to comprehend and write effective reports and design documentation, make effective presentations, taking into account cultural, language, and learning differences;"],
  ["EAC10", "C", "Project Management and Finance", "", "Apply knowledge and understanding of engineering management principles and economic decision-making and apply these to one\u2019s own work, as a member and leader in a team, and to manage projects in multidisciplinary environments;"],
  ["EAC11", "A", "Life Long Learning", "WK8", "Recognise the need for, and have the preparation and ability for i) independent and life-long learning ii) adaptability to new and emerging technologies and iii) critical thinking in the broadest context of technological change."]
].map(([code, taxonomy, name, wk, desc]) => ({ code, taxonomy, name, wk, desc }));

const newEacSet = (target) => EAC_CATALOGUE.map(e =>
  ({ id: e.code, code: e.code, taxonomy: e.taxonomy, name: e.name, wk: e.wk, desc: e.desc,
     selected: false, target: target == null ? 60 : target, studentThreshold: null }));

const DEVELOPER  = "Prof. Dr. Zurina Zainal Abidin";
const FACULTY    = "Faculty of Engineering";
const UNIVERSITY = "Universiti Putra Malaysia";

const DELIVERY = ["Lecture", "SCL", "Lecture | SCL", "Laboratory", "Tutorial", "Project"];

/* ---------------- model ---------------- */

const GRADE_SCALE = [
  { min: 79.5, grade: "A" }, { min: 74.5, grade: "A-" }, { min: 69.5, grade: "B+" },
  { min: 64.5, grade: "B" }, { min: 59.5, grade: "B-" }, { min: 54.5, grade: "C+" },
  { min: 49.5, grade: "C" }, { min: 46.5, grade: "C-" }, { min: 43.5, grade: "D+" },
  { min: 39.5, grade: "D" }
];
const PASS_GRADE_MIN = 49.5;

/** An untouched course record — nothing typed, nothing mapped, no students. */
function isPristine(c) {
  if (!c) return false;
  const bare = !["courseCode", "courseName", "semester", "lecturer", "group", "programme", "department"]
    .some(k => (c[k] || "").trim() && c[k] !== "Untitled course");
  const noStudents = !(c.students || []).length;
  const noWork = (c.assessments || []).every(a => !(a.clos || []).length && !(a.eacs || []).length);
  return bare && noStudents && noWork;
}

function blankCourse(name) {
  return {
    id: uid("c"), v: 2,
    programme: "", department: "", courseName: name || "Untitled course", courseCode: "",
    semester: "", lecturer: "", group: "", curriculum: "2021-2025",
    studentThreshold: 50, defaultTarget: 60,
    gradeScale: GRADE_SCALE.map(g => ({ ...g })),
    clos: [{ id: uid("o"), code: "CO1", desc: "", taxonomy: "", target: 60, studentThreshold: null }],
    eacs: newEacSet(60),
    assessments: [{ id: uid("a"), name: "Test 1", fullMark: 100, delivery: "Lecture", clos: [], eacs: [] }],
    students: [],
    cas: { prevReview: "", teachingPlan: "", eacComments: {}, cloComments: {},
           reflection: "", recommendation: "" },
    updated: Date.now()
  };
}

/** The ECC3014 spreadsheet, rebuilt — for checking the figures against the old workbook. */
function templateCourse() {
  const c = blankCourse("Engineering Statistics");
  c.semester = "Semester 1, 2020/2021";
  c.courseCode = "ECC3014";
  c.lecturer = "Dr. XYZ";
  c.group = "1";
  c.programme = "Bachelor of Mechanical Engineering with Honours";
  c.department = "Mechanical and Manufacturing Engineering";
  const clo = [
    ["CO1", "Analyse engineering data using descriptive and inferential statistics (WK, C4)"],
    ["CO2", "Apply probability distributions to engineering problems (WK, C3)"],
    ["CO3", "Design and report a statistical study of an engineering process (WK, A3)"]
  ].map(([code, desc]) => ({ id: uid("o"), code, desc, taxonomy: "", target: 60, studentThreshold: null }));
  c.clos = clo;
  ["EAC1", "EAC2", "EAC6", "EAC11"].forEach(k => {
    const e = c.eacs.find(x => x.id === k); if (e) e.selected = true;
  });
  const A = (name, fullMark, delivery, cl, ec) =>
    ({ id: uid("a"), name, fullMark, delivery, clos: cl.map(i => clo[i].id), eacs: ec });
  c.assessments = [
    A("Test 1", 15, "Lecture", [0], ["EAC1"]),
    A("Test 2", 15, "Lecture", [1], ["EAC2"]),
    A("Assignment 1", 10, "SCL", [2], ["EAC11"]),
    A("Assignment 2", 10, "SCL", [1], ["EAC6"]),
    A("Quiz", 10, "Lecture", [1], ["EAC2"]),
    A("Final exam", 40, "Lecture", [0], ["EAC2"])
  ];
  const raw = [[15,15,8,10,9,35],[11,5.5,8,10,7,16.5],[15,8,7.5,9.5,8,34],[6,13,8,10,9,8],
    [14,10,9,8.5,8,35],[10.5,13,8,10,9,10],[7,11,8,10,8,18.5],[4.5,6,9.5,9.5,8,23],
    [7,15,8,8,8,8.5],[9,9,8,9,7,23],[6,14,9,9,9,10],[5,9,9,9,8,30.5],[15,12,9.5,9.5,8,28.5],
    [5,7,8,10,9,21],[12,5,7.5,9.5,9,22.5],[12,13,7.5,8.5,8,20],[6.5,8,8,8,7,7.5],
    [7.5,10,9,6,8,28.5],[11.5,10,8,9.5,8,19.5],[5.5,8,8,10,8,29.5],[12,8,8,9,8,11],
    [13,8.5,7.5,9,7,12],[10,7,9,8,5,22.5],[7.5,12.5,8,8,8,7.5],[14,10,7.5,8,8,30.5],
    [5.5,10,9.5,10,9,7.5],[6,10,8,9,5,3],[10,11.5,8,8,8,26.5],[11,10,8,9,7,27.5],
    [8,15,9,9.5,8,31],[5,4,9,9,9,14.5],[10,5.5,8,9,8,16.5],[13,7.5,9.5,8,8,18.5],
    [10,14,8,10,3,17],[6,12,9.5,8,8,8.5],[5,8,7.5,10,8,28.5],[11,13,8,8.5,6,28],
    [7,4,8,8,9,20],[10.5,9.5,8.5,7.5,8,29],[16,14,8,9,7,20],[9,12,8,8.5,8,29],
    [11.5,10.5,8.5,7.5,7,9.5],[12,12,8,8,8,31.5],[7,14,9,10,7,11.5],[9.5,13,9,8,8,7.5],
    [5,9,9.5,8.5,8,31.5],[5,7,9.5,10,8,36.5],[4,10.5,9,10,9,16],[14,8,8,9.5,8,11.5],
    [6,10,8,7,8,29],[6.5,9,9.5,10,9,13],[5,14,8.5,8,8,8],[9,15,8,9,6,11.5],
    [13.5,10,9.5,9,7,17],[14,10,8,8.5,8,23],[6,13,8.5,8.5,7,11],[5,1,9.5,0,7,6]];
  c.students = raw.map((row, i) => {
    const marks = {};
    c.assessments.forEach((a, j) => { marks[a.id] = row[j]; });
    return { id: uid("s"), matric: String(190000 + i * 7), name: "Student " + (i + 1), marks, excluded: false };
  });
  return c;
}

/** Older records predate the EAC catalogue and per-outcome minimums. */
function migrate(c) {
  if (!c) return c;
  if (!Array.isArray(c.eacs) || !c.eacs.length) {
    c.eacs = newEacSet(c.cohortThreshold || 60);
    if (Array.isArray(c.plos)) {
      // carry an old PLO mapping over where the code matches PLOn -> EACn
      c.plos.forEach(old => {
        const n = String(old.code || "").match(/(\d+)/);
        const hit = n && c.eacs.find(e => e.id === "EAC" + n[1]);
        if (hit) {
          hit.selected = true;
          (c.assessments || []).forEach(a => {
            if ((a.plos || []).includes(old.id)) a.eacs = [...new Set([...(a.eacs || []), hit.id])];
          });
        }
      });
    }
  }
  delete c.plos;
  (c.eacs || []).forEach(e => {                       // keep the wording current
    const ref = EAC_CATALOGUE.find(x => x.code === e.id);
    if (ref) { e.code = ref.code; e.name = ref.name; e.taxonomy = ref.taxonomy; e.wk = ref.wk; e.desc = ref.desc; }
  });
  if (c.defaultTarget == null) c.defaultTarget = c.cohortThreshold || 60;
  (c.clos || []).forEach(o => {
    if (o.target == null) o.target = c.defaultTarget;
    if (o.studentThreshold === undefined) o.studentThreshold = null;
    if (o.taxonomy === undefined) o.taxonomy = "";
  });
  (c.assessments || []).forEach(a => { if (!a.delivery) a.delivery = "Lecture"; if (!a.eacs) a.eacs = []; });
  if (!c.cas) c.cas = { prevReview: "", teachingPlan: "", eacComments: {}, cloComments: {}, reflection: "", recommendation: "" };
  if (!c.curriculum) c.curriculum = "2021-2025";
  c.v = 2;
  return c;
}

/* ---------------- calculation engine ---------------- */

function calc(course) {
  const A = course.assessments || [];
  const usedEac = new Set();
  A.forEach(a => (a.eacs || []).forEach(id => usedEac.add(id)));
  const outcomes = [
    ...(course.clos || []).map(o => ({ ...o, kind: "CLO", key: "clos" })),
    ...(course.eacs || []).filter(o => usedEac.has(o.id)).map(o => ({ ...o, kind: "EAC", key: "eacs" }))
  ];
  const active = (course.students || []).filter(s => !s.excluded);
  const n = active.length;
  const baseT = Number(course.studentThreshold) || 50;
  const gradeScale = (course.gradeScale || GRADE_SCALE).slice().sort((a, b) => Number(b.min) - Number(a.min));
  const fullTotal = A.reduce((t, a) => t + (Number(a.fullMark) || 0), 0);

  outcomes.forEach(o => {
    o.members = A.filter(a => (a[o.key] || []).includes(o.id));
    o.fullMark = o.members.reduce((t, a) => t + (Number(a.fullMark) || 0), 0);
    o.stuT = o.studentThreshold == null || o.studentThreshold === "" ? baseT : Number(o.studentThreshold);
    o.tgt = o.target == null || o.target === "" ? (Number(course.defaultTarget) || 60) : Number(o.target);
  });

  const rows = active.map(s => {
    const marks = s.marks || {};
    let total = 0, missing = 0;
    A.forEach(a => {
      const v = marks[a.id];
      if (v === null || v === undefined || v === "") missing++;
      total += Number(v) || 0;
    });
    const totalPct = fullTotal > 0 ? r2(total / fullTotal * 100) : null;
    let grade = "F";
    for (const g of gradeScale) { if (totalPct != null && totalPct >= Number(g.min)) { grade = g.grade; break; } }
    const oPct = {};
    outcomes.forEach(o => {
      if (o.fullMark > 0) {
        const got = o.members.reduce((t, a) => t + (Number(marks[a.id]) || 0), 0);
        oPct[o.kind + ":" + o.id] = r2(got / o.fullMark * 100);
      } else oPct[o.kind + ":" + o.id] = null;
    });
    return { s, total: r2(total), totalPct, grade, oPct, missing };
  });

  const cols = A.map(a => {
    const fm = Number(a.fullMark) || 0;
    const cut = fm * baseT / 100;
    const vals = rows.map(r => Number(r.s.marks?.[a.id]) || 0);
    const y = fm > 0 ? vals.filter(v => v >= cut).length : 0;
    const z = n > 0 ? r2(y / n * 100) : null;
    const mean = n > 0 && fm > 0 ? r2(vals.reduce((t, v) => t + v, 0) / n / fm * 100) : null;
    const weight = fullTotal > 0 ? r2(fm / fullTotal * 100) : 0;
    return { a, cut: r2(cut), y, z, meanPct: mean, weight, verdict: z != null && z >= (Number(course.defaultTarget) || 60) };
  });

  const outs = outcomes.map(o => {
    const k = o.kind + ":" + o.id;
    const vals = rows.map(r => r.oPct[k]).filter(v => v != null);
    const y = vals.filter(v => v >= o.stuT).length;
    const z = n > 0 && o.fullMark > 0 ? r2(y / n * 100) : null;
    const mean = vals.length ? r2(vals.reduce((t, v) => t + v, 0) / vals.length) : null;
    return { o, key: k, y, z, meanPct: mean, verdict: z != null && z >= o.tgt };
  });

  const passY = rows.filter(r => r.totalPct != null && r.totalPct >= PASS_GRADE_MIN).length;
  const overall = {
    n, fullTotal,
    meanPct: n ? r2(rows.reduce((t, r) => t + (r.totalPct || 0), 0) / n) : null,
    minPct: n ? r2(Math.min(...rows.map(r => r.totalPct || 0))) : null,
    maxPct: n ? r2(Math.max(...rows.map(r => r.totalPct || 0))) : null,
    passY, passZ: n ? r2(passY / n * 100) : null,
    excluded: (course.students || []).length - n
  };
  const gradeCount = {};
  rows.forEach(r => { gradeCount[r.grade] = (gradeCount[r.grade] || 0) + 1; });

  const clos = outs.filter(x => x.o.kind === "CLO");
  const eacs = outs.filter(x => x.o.kind === "EAC");

  /* the CAS section D grid: one cell per CLO × EAC, naming the assessments that
     serve both, grouped by how they were delivered */
  const grid = {};
  eacs.forEach(e => clos.forEach(cl => {
    const hits = A.filter(a => (a.eacs || []).includes(e.o.id) && (a.clos || []).includes(cl.o.id));
    if (!hits.length) { grid[e.o.id + "|" + cl.o.id] = ""; return; }
    const byDelivery = {};
    hits.forEach(a => {
      const d = a.delivery || "Lecture";
      (byDelivery[d] = byDelivery[d] || []).push(
        `${a.name} (${fmt(fullTotal > 0 ? a.fullMark / fullTotal * 100 : 0, 0)}%)`);
    });
    grid[e.o.id + "|" + cl.o.id] = Object.entries(byDelivery)
      .map(([d, list]) => `${d} | ${list.join(", ")}`).join("; ");
  }));

  return { rows, cols, outs, clos, eacs, outcomes, overall, gradeCount, baseT, fullTotal, gradeScale, grid };
}

/* ---------------- validation ---------------- */

function validate(course, res) {
  const out = [];
  const add = (level, msg, where) => out.push({ level, msg, where });
  const A = course.assessments || [];

  if (!course.courseCode?.trim() || !course.courseName?.trim())
    add("warn", "Course code and name are blank. They head the CAS form.", "Setup");
  if (!course.semester?.trim()) add("warn", "No semester or session recorded.", "Setup");
  if (!course.programme?.trim()) add("warn", "No programme recorded.", "Setup");
  if (!A.length) add("err", "No assessments defined yet.", "Setup");

  const ft = res.fullTotal;
  if (A.length && Math.abs(ft - 100) > 0.001)
    add(ft > 100 ? "err" : "warn",
        `Assessment marks add up to ${fmt(ft)}, not 100. The CAS form requires a total of 100%.`, "Setup");

  A.forEach(a => {
    if (!(Number(a.fullMark) > 0)) add("err", `“${a.name}” has no full mark.`, "Setup");
    if (!(a.clos || []).length) add("err", `“${a.name}” is not assigned to a CLO.`, "Assessments");
    if (!(a.eacs || []).length) add("err", `“${a.name}” is not assigned to an EAC.`, "Assessments");
  });
  if (!res.eacs.length) add("err", "No assessment has been assigned to an EAC yet.", "Assessments");
  res.outcomes.forEach(o => {
    if (!o.members.length) add("err", `${o.code} has no assessment assigned to it, so it cannot be measured.`, "Assessments");   // CLOs only; an EAC without an assessment is simply not carried
  });
  if (!(course.students || []).length) add("err", "No students in the roster.", "Marks");

  let over = 0, neg = 0, blanks = 0;
  const seen = new Map(); const dups = new Set();
  (course.students || []).forEach(s => {
    A.forEach(a => {
      const v = s.marks?.[a.id];
      if (v === null || v === undefined || v === "") { if (!s.excluded) blanks++; return; }
      const num = Number(v);
      if (!isFinite(num)) { over++; return; }
      if (num > Number(a.fullMark) + 1e-9) over++;
      if (num < 0) neg++;
    });
    const m = (s.matric || "").trim();
    if (m) { if (seen.has(m)) dups.add(m); else seen.set(m, 1); }
  });
  if (over) add("err", `${over} mark${over > 1 ? "s exceed" : " exceeds"} the full mark for its assessment.`, "Marks");
  if (neg) add("err", `${neg} negative mark${neg > 1 ? "s" : ""} entered.`, "Marks");
  if (blanks) add("warn", `${blanks} mark${blanks > 1 ? "s are" : " is"} blank and counted as zero.`, "Marks");
  if (dups.size) add("err", `Duplicate matric number${dups.size > 1 ? "s" : ""}: ${[...dups].join(", ")}.`, "Marks");
  if (res.overall.excluded) add("warn", `${res.overall.excluded} student${res.overall.excluded > 1 ? "s are" : " is"} excluded from the analysis.`, "Marks");

  const cas = course.cas || {};
  const missingNarrative = [];
  res.eacs.forEach(x => { if (!(cas.eacComments || {})[x.o.id]?.trim()) missingNarrative.push(x.o.code); });
  res.clos.forEach(x => { if (!(cas.cloComments || {})[x.o.id]?.trim()) missingNarrative.push(x.o.code); });
  if (missingNarrative.length)
    add("warn", `Section E/F comments still empty for ${missingNarrative.join(", ")}.`, "CAS form");
  if (!cas.reflection?.trim()) add("warn", "Section G, the teaching and learning reflection, is empty.", "CAS form");
  if (!cas.recommendation?.trim()) add("warn", "Section H, the overall recommendation, is empty.", "CAS form");

  if (!out.length) add("ok", "Everything checks out. The CAS is ready to sign off.", "");
  return out;
}

/* ---------------- storage ---------------- */

const Store = {
  db: null, mode: "local", ready: false,
  async init() {
    try {
      if (window.claude && typeof window.claude.use === "function") {
        const db = await Promise.race([
          window.claude.use("db"),
          new Promise(r => setTimeout(() => r(null), 11000))
        ]);
        if (db) { this.db = db; this.mode = "db"; }
      }
    } catch (e) { /* fall through to local */ }
    this.ready = true;
    return this.mode;
  },
  async list() {
    if (this.mode === "db") {
      const snap = await this.db.collection("courses").limit(200).get();
      return snap.docs.map(d => d.data()).filter(Boolean);
    }
    try {
      const cur = JSON.parse(localStorage.getItem("cas.courses") || "[]");
      if (cur.length) return cur;
      const old = JSON.parse(localStorage.getItem("cam.courses") || "[]");   // records from the earlier version
      return old;
    } catch (e) { return []; }
  },
  async save(course) {
    course.updated = Date.now();
    if (this.mode === "db") {
      await this.db.doc("courses/" + course.id).set(JSON.parse(JSON.stringify(course)));
      return;
    }
    const all = await this.list();
    const i = all.findIndex(c => c.id === course.id);
    if (i >= 0) all[i] = course; else all.push(course);
    localStorage.setItem("cas.courses", JSON.stringify(all));
  },
  async remove(id) {
    if (this.mode === "db") { await this.db.doc("courses/" + id).delete(); return; }
    const all = (await this.list()).filter(c => c.id !== id);
    localStorage.setItem("cas.courses", JSON.stringify(all));
  },
  async getSettings() {
    if (this.mode === "db") {
      try { const d = await this.db.doc("settings/app").get(); return d.exists ? d.data() : {}; }
      catch (e) { return {}; }
    }
    try { return JSON.parse(localStorage.getItem("cas.settings") || "{}"); } catch (e) { return {}; }
  },
  async setSettings(obj) {
    if (this.mode === "db") { await this.db.doc("settings/app").set(obj); return; }
    localStorage.setItem("cas.settings", JSON.stringify(obj));
  }
};

/* ---------------- app state + save queue ---------------- */

const S = { courses: [], activeId: null, view: "home", saving: false, pending: false,
            doc: "cas" };
const course = () => S.courses.find(c => c.id === S.activeId) || null;

let saveTimer = null;
function markDirty(redraw) {
  const c = course(); if (!c) return;
  c.updated = Date.now();
  setSaveState("Saving…", "busy");
  clearTimeout(saveTimer);
  saveTimer = setTimeout(flush, 700);
  if (redraw !== false) renderChrome();
}
async function flush() {
  const c = course(); if (!c) return;
  if (S.saving) { S.pending = true; return; }
  S.saving = true;
  try {
    await Store.save(c);
    setSaveState("Saved " + new Date().toLocaleTimeString([], { hour: "2-digit", minute: "2-digit" }), "");
  } catch (e) {
    setSaveState(e && e.code === "invalid_argument" ? "Read-only — not saved" : "Not saved", "err");
  } finally {
    S.saving = false;
    if (S.pending) { S.pending = false; flush(); }
  }
}
function setSaveState(text, cls) {
  const el = $("#saveState");
  el.textContent = text;
  el.className = "savestate " + (cls || "");
}

/* ============================================================
   Views: chrome, home, setup
   ============================================================ */

const CREST = "data:image/png;base64,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";

function renderChrome() {
  const sel = $("#coursePick");
  sel.innerHTML = S.courses.slice().sort((a, b) => (b.updated || 0) - (a.updated || 0))
    .map(c => `<option value="${esc(c.id)}"${c.id === S.activeId ? " selected" : ""}>${
      esc([c.courseCode, c.courseName].filter(Boolean).join(" · ") || "Untitled course")}${
      c.group ? esc(" — group " + c.group) : ""}</option>`).join("");
  sel.style.display = S.courses.length ? "" : "none";
  $$("#tabs .tab").forEach(b => b.setAttribute("aria-selected", String(b.dataset.view === S.view)));
  const c = course();
  $("#tabCount").textContent = c ? (c.students || []).length : "";
}

function render() {
  renderChrome();
  const app = $("#app");
  const c = course();
  if (S.view === "home" || !c) { app.innerHTML = viewHome(c); return; }
  const res = calc(c);
  const views = { setup: viewSetup, marks: viewMarks, analysis: viewAnalysis,
                  cas: viewCas, print: viewPrint, data: viewData };
  app.innerHTML = (views[S.view] || viewSetup)(c, res);
  app.scrollTop = 0;
}

/* ---------------- home ---------------- */

function viewHome(active) {
  const cards = S.courses.slice().sort((a, b) => (b.updated || 0) - (a.updated || 0)).map(c => {
    let st = { n: 0, short: 0, measured: 0 };
    try {
      const r = calc(c);
      st = { n: r.overall.n, short: r.outs.filter(x => !x.verdict && x.o.fullMark > 0).length,
             measured: r.outs.filter(x => x.o.fullMark > 0).length };
    } catch (e) {}
    const title = [c.courseCode, c.courseName].filter(x => (x || "").trim()).join(" · ");
    const ready = st.measured > 0 && st.n > 0;
    const status = !ready ? "Not set up yet"
      : st.short ? st.short + (st.short === 1 ? " outcome" : " outcomes") + " below the minimum"
      : "All outcomes attained";
    return `<div class="ccard" data-open="${esc(c.id)}" role="button" tabindex="0">
      <button class="ccdel" data-cdel="${esc(c.id)}" aria-label="Delete this course">&times;</button>
      <b>${title ? esc(title) : "Untitled course"}</b>
      <span>${esc(c.semester || "No semester recorded")}${c.group ? esc(" · group " + c.group) : ""}</span>
      <span class="st"><span>${st.n} student${st.n === 1 ? "" : "s"}</span>
        <span style="color:${!ready ? "var(--ink-3)" : st.short ? "var(--no)" : "var(--yes)"}">${status}</span></span>
    </div>`;
  }).join("");

  return `
  <section class="hero">
    <div class="hero-crest"><img src="${CREST}" alt="Universiti Putra Malaysia"></div>
    <div class="kicker">PU/PS/FK/CAS · Borang Ringkasan Penilaian Kursus</div>
    <h1>Course Assessment Summary</h1>
    <p class="lede">Enter marks once. The system computes CLO and EAC attainment by the CAM method
      and prints the signed summary your department files each semester.</p>
  </section>

  <section class="panel">
    <header><h2>Courses</h2><span class="note">${S.courses.length} record${S.courses.length === 1 ? "" : "s"}</span></header>
    <div class="body">
      ${S.courses.length ? `<div class="clist">${cards}</div>`
        : `<p class="hint" style="margin:0 0 14px">Nothing recorded yet. Create a course, or load the worked
             example to see the whole flow end to end.</p>`}
      <div class="row" style="margin-top:${S.courses.length ? "16px" : "0"}">
        <button class="btn" id="mkBlank">Create a course</button>
        <button class="btn sec" id="mkDemo">Load the worked example</button>
        ${active ? `<span class="spacer"></span><button class="btn sec" data-go="setup">Continue with ${esc(active.courseCode || "the open course")}</button>` : ""}
      </div>
    </div>
  </section>

  <section class="panel">
    <header><h2>How a semester runs</h2></header>
    <div class="body">
      <ol style="margin:0; padding-left:20px; font-size:13.5px; color:var(--ink-2); line-height:1.75">
        <li><b>Setup</b> — record the course, write the CLOs, then list each assessment with its
          percentage and assign it to the CLOs and EACs it measures. Set the minimum attainment each
          outcome must reach this semester.</li>
        <li><b>Marks</b> — type or paste the raw marks. Totals, grades and every outcome percentage follow.</li>
        <li><b>Attainment</b> — read Y, Z and the attained status against each minimum, and see where the cohort fell short.</li>
        <li><b>CAS form</b> — write sections B, E, F, G and H. The alignment grid fills itself from the mapping.</li>
        <li><b>Print</b> — the CAS form and the CAM sheet, both ready to sign.</li>
      </ol>
    </div>
  </section>

  <footer class="credit">
    <img src="${CREST}" alt="Universiti Putra Malaysia">
    <div>
      <b>Developed by ${esc(DEVELOPER)}</b>
      <span>${esc(FACULTY)}</span>
      <span>${esc(UNIVERSITY)}</span>
    </div>
  </footer>`;
}

/* ---------------- setup ---------------- */

function viewSetup(c, res) {
  const f = (label, key, ph, type) => `<div><label class="f" for="fld_${key}">${label}</label>
    <input id="fld_${key}" type="${type || "text"}" data-fld="${key}" value="${esc(c[key] ?? "")}" placeholder="${esc(ph || "")}"></div>`;

  const cloRow = o => `<tr data-oid="${o.id}" data-kind="clos">
      <td style="width:84px"><input class="txtin" style="min-width:66px" data-ocode value="${esc(o.code)}" aria-label="CLO code"></td>
      <td><input class="txtin" data-odesc value="${esc(o.desc || "")}" placeholder="Analyse … (WK, C4)" aria-label="CLO statement"></td>
      <td class="n" style="width:94px"><input class="cellin" data-otarget type="number" min="0" max="100" step="1" value="${esc(o.target)}" aria-label="Minimum attainment for ${esc(o.code)}"></td>
      <td style="width:38px"><button class="iconbtn" data-odel aria-label="Remove ${esc(o.code)}">×</button></td>
    </tr>`;

  const chip = (a, kind, o) => `<button class="chip" data-chip="${kind}" data-oid="${esc(o.id)}"
      title="${esc(o.name || o.desc || o.code)}"
      aria-pressed="${(a[kind] || []).includes(o.id)}">${esc(o.code)}</button>`;
  const liveEacs = c.eacs;
  const aCard = a => {
    const noClo = !(a.clos || []).length, noEac = !(a.eacs || []).length;
    const share = res.fullTotal ? fmt(a.fullMark / res.fullTotal * 100, 1) + "% of course marks" : "";
    return `<div class="acard${noClo || noEac || !(Number(a.fullMark) > 0) ? " bad" : ""}" data-aid="${a.id}">
      <div class="atop">
        <input class="aname" data-aname value="${esc(a.name)}" aria-label="Assessment name" placeholder="Test 1">
        <select data-adeliv aria-label="Teaching delivery for ${esc(a.name)}">
          ${DELIVERY.concat(DELIVERY.includes(a.delivery) ? [] : [a.delivery])
            .map(d => `<option${d === a.delivery ? " selected" : ""}>${esc(d)}</option>`).join("")}</select>
        <label class="amark"><span>Marks</span>
          <input class="cellin" data-afull type="number" step="0.5" min="0" value="${esc(a.fullMark)}"
            aria-label="Marks for ${esc(a.name)}">%</label>
        <span class="tot-cell">${share}</span>
        <button class="iconbtn" data-adel aria-label="Remove ${esc(a.name)}">×</button>
      </div>
      <div class="arow"><span class="alab">CLO</span>
        ${c.clos.length ? `<div class="chips">${c.clos.map(o => chip(a, "clos", o)).join("")}</div>`
          : `<span class="chipnote mute">Write the course outcomes above, then assign them here.</span>`}
        ${c.clos.length && noClo ? `<span class="chipnote">assign at least one</span>` : ""}</div>
      <div class="arow"><span class="alab">EAC</span>
        <div class="chips">${liveEacs.map(o => chip(a, "eacs", o)).join("")}</div>
        ${liveEacs.length && noEac ? `<span class="chipnote">assign at least one</span>` : ""}</div>
    </div>`;
  };

  const mapTable = kind => {
    const list = kind === "clos" ? c.clos : c.eacs.filter(e => e.selected);
    if (!list.length || !c.assessments.length)
      return `<p class="hint">${kind === "clos" ? "Add CLOs" : "Tick the EACs this course carries"} and list the assessments first.</p>`;
    const head = list.map(o => `<th class="rot"><div>${esc(o.code)}</div></th>`).join("");
    const body = c.assessments.map(a => `<tr data-aid="${a.id}">
        <td>${esc(a.name)}</td><td class="n tot-cell">${esc(a.fullMark)}</td>
        ${list.map(o => `<td class="chk"><input type="checkbox" data-map="${kind}" data-oid="${o.id}"
          ${(a[kind] || []).includes(o.id) ? "checked" : ""}
          aria-label="${esc(a.name)} measures ${esc(o.code)}"></td>`).join("")}
      </tr>`).join("");
    const foot = list.map(o => {
      const oo = res.outcomes.find(x => x.kind === (kind === "clos" ? "CLO" : "EAC") && x.id === o.id);
      return `<td class="n">${oo && oo.fullMark ? fmt(oo.fullMark, 0) : "<span style='color:var(--no)'>0</span>"}</td>`;
    }).join("");
    return `<div class="scroll"><table class="map">
      <thead><tr><th>Assessment</th><th class="n">Marks</th>${head}</tr></thead>
      <tbody>${body}</tbody>
      <tfoot><tr><td colspan="2">Marks measuring each outcome</td>${foot}</tr></tfoot>
    </table></div>`;
  };

  const gradeRows = res.gradeScale.map((g, i) => `<tr data-gi="${i}">
      <td style="width:90px"><input class="txtin" style="min-width:56px" data-gname value="${esc(g.grade)}" aria-label="Grade letter"></td>
      <td class="n"><input class="cellin" data-gmin type="number" step="0.5" value="${esc(g.min)}" aria-label="Minimum percentage for ${esc(g.grade)}"></td>
      <td style="width:38px"><button class="iconbtn" data-gdel aria-label="Remove grade ${esc(g.grade)}">×</button></td>
    </tr>`).join("");

  return `
  <section class="panel">
    <header><h2>Course</h2><span class="note">Heads the CAS form</span></header>
    <div class="body"><div class="grid2">
      ${f("Programme", "programme", "Bachelor of Mechanical Engineering with Honours")}
      ${f("Department", "department", "Mechanical and Manufacturing Engineering")}
      ${f("Course name", "courseName", "Dynamics")}
      ${f("Course code", "courseCode", "EMM3118")}
      ${f("Semester / session", "semester", "Semester 1, 2025/2026")}
      ${f("Lecturer", "lecturer", "Dr. …")}
      ${f("Group", "group", "1")}
      <div><label class="f" for="fld_curr">Curriculum</label>
        <select id="fld_curr" data-fld="curriculum">
          <option value="2021-2025"${c.curriculum === "2021-2025" ? " selected" : ""}>2021 – 2025 (11 EACs)</option>
          <option value="2016-2020"${c.curriculum === "2016-2020" ? " selected" : ""}>2016 – 2020 (14 POs)</option>
        </select></div>
    </div></div>
  </section>

  <section class="panel">
    <header><h2>Course learning outcomes</h2>
      <span class="note">The minimum each outcome must reach this semester</span></header>
    <div class="body flush"><table>
      <thead><tr><th>Code</th><th>Statement, with taxonomy level</th><th class="n" style="width:112px">Min. attainment (%)</th><th></th></tr></thead>
      <tbody id="cloBody">${c.clos.map(cloRow).join("")}</tbody></table></div>
    <div class="body" style="border-top:1px solid var(--rule-soft)"><button class="btn sec sm" id="addCLO">Add CLO</button></div>
  </section>

  <section class="panel">
    <header><h2>Assessments</h2>
      <span class="note" style="color:${Math.abs(res.fullTotal - 100) < .001 ? "var(--yes)" : "var(--no)"}">
        ${fmt(res.fullTotal, 1)}% of 100 allocated</span></header>
    <div class="body">
      <p class="hint">Every assessment carries a percentage of the course total and must be assigned to at least
        one CLO and at least one EAC. Those assignments drive the attainment figures and write section D of the
        CAS form, so an unassigned assessment is flagged until you deal with it.</p>
      ${c.assessments.map(aCard).join("")}
      <div class="row" style="margin-top:12px">
        <button class="btn sec sm" id="addA">Add assessment</button>
        <span class="spacer"></span>
        <span class="hint" style="margin:0">Total allocated
          <b class="num" style="color:${Math.abs(res.fullTotal - 100) < .001 ? "var(--yes)" : "var(--no)"}">${fmt(res.fullTotal, 1)}%</b></span>
      </div>
    </div>
  </section>

  <section class="panel">
    <header><h2>Programme outcomes in use</h2>
      <span class="note">${res.eacs.length} of 11 carried by this course</span></header>
    <div class="body" style="padding-bottom:4px">
      <p class="hint" style="margin:0">An EAC appears here as soon as an assessment above is assigned to it,
        and it is ticked in section C(b) of the CAS form. Each minimum is recorded per semester, so a course
        may require 60% on EAC2 one semester and 70% the next.</p>
    </div>
    ${res.eacs.length ? `<div class="scroll" style="max-height:none"><table>
      <thead><tr><th style="width:210px">Outcome</th><th>Description</th><th class="n" style="width:112px">Min. attainment (%)</th></tr></thead>
      <tbody>${res.eacs.map(x => `<tr data-oid="${esc(x.o.id)}" data-kind="eacs">
        <td><b>${esc(x.o.code)} (${esc(x.o.taxonomy)})</b><br>
          <span style="font-size:11.5px;color:var(--ink-3)">${esc(x.o.name)}</span></td>
        <td style="white-space:normal;font-size:12px;color:var(--ink-2);line-height:1.4">${esc(x.o.desc)}</td>
        <td class="n"><input class="cellin" data-otarget type="number" min="0" max="100" step="1"
          value="${esc(x.o.target)}" aria-label="Minimum attainment for ${esc(x.o.code)}"></td></tr>`).join("")}</tbody>
    </table></div>` : `<div class="body" style="padding-top:0"><p class="hint" style="color:var(--no);margin:0">
      No assessment has been assigned to an EAC yet. Use the EAC buttons on each assessment above.</p></div>`}
    <details class="body" style="border-top:1px solid var(--rule-soft)">
      <summary style="cursor:pointer;font-size:13px;color:var(--head)">All eleven EAC programme outcomes</summary>
      <table style="margin-top:10px"><tbody>${c.eacs.map(o => `<tr>
        <td style="width:200px;vertical-align:top"><b>${esc(o.code)} (${esc(o.taxonomy)})</b><br>
          <span style="font-size:11.5px;color:var(--ink-3)">${esc(o.name)}</span></td>
        <td style="white-space:normal;font-size:12px;color:var(--ink-2);line-height:1.45">${esc(o.desc)}${
          o.wk ? ` <b style="color:var(--ink-3)">(${esc(o.wk)})</b>` : ""}</td></tr>`).join("")}</tbody></table>
    </details>
  </section>

  <section class="panel">
    <header><h2>Mapping check</h2><span class="note">Read back from the assignments above</span></header>
    <div class="body">
      <p class="hint">Each course outcome, the assessments that measure it, and the programme outcomes those
        assessments carry. Read down a chain to confirm the mapping is what you intended.</p>
      ${c.clos.length ? c.clos.map(cl => {
        const oo = res.outcomes.find(x => x.kind === "CLO" && x.id === cl.id) || { members: [], fullMark: 0, tgt: c.defaultTarget };
        const reached = [];
        oo.members.forEach(a => (a.eacs || []).forEach(e => { if (!reached.includes(e)) reached.push(e); }));
        const nameOf = id => (c.eacs.find(e => e.id === id) || {}).code || id;
        const gaps = oo.members.some(a => !(a.eacs || []).length);
        return `<div class="cblock${oo.members.length && !gaps ? "" : " bad"}">
          <div class="chead">
            <b>${esc(cl.code)}</b>
            <span class="cdesc">${esc(cl.desc || "No statement written yet")}</span>
            <span class="cnum">${fmt(oo.fullMark, 0)} marks · ${res.fullTotal ? fmt(oo.fullMark / res.fullTotal * 100, 1) : "0"}% of the course</span>
            <span class="cnum">needs ${oo.tgt}%</span>
          </div>
          ${oo.members.length ? `<ul class="clink">${oo.members.map(a => `<li>
            <span class="anm">${esc(a.name)}</span>
            <span class="adel">${esc(a.delivery || "")}</span>
            <span class="apc">${fmt(res.fullTotal ? a.fullMark / res.fullTotal * 100 : 0, 1)}%</span>
            <span class="arrow">&rarr;</span>
            <span>${(a.eacs || []).length ? (a.eacs || []).map(e => `<span class="pill">${esc(nameOf(e))}</span>`).join("")
              : `<span class="pill miss">no EAC assigned</span>`}</span></li>`).join("")}</ul>`
            : `<p style="margin:8px 0 0;font-size:13px;color:var(--no)">No assessment measures ${esc(cl.code)} yet.</p>`}
          ${reached.length ? `<div class="cfoot">Programme outcomes reached through ${esc(cl.code)}:
            ${reached.map(e => esc(nameOf(e))).join(", ")}</div>` : ""}
        </div>`;
      }).join("") : `<p class="hint" style="color:var(--no);margin:0">No course outcomes written yet.</p>`}
    </div>
    ${res.eacs.length ? `<div class="body" style="border-top:1px solid var(--rule-soft);padding-bottom:6px">
      <h3 style="font-size:13px;margin-bottom:4px">The same mapping, seen from the programme outcomes</h3>
      <p class="hint" style="margin-bottom:0">Use this to check nothing is over- or under-weighted.</p>
    </div>
    <div class="scroll" style="max-height:none"><table>
      <thead><tr><th>Programme outcome</th><th>Reached through</th><th>Assessed by</th>
        <th class="n">Marks</th><th class="n">% of course marks</th><th class="n">Min. attainment</th></tr></thead>
      <tbody>${res.eacs.map(x => {
        const via = c.clos.filter(cl => x.o.members.some(a => (a.clos || []).includes(cl.id))).map(cl => cl.code);
        return `<tr>
          <td><b>${esc(x.o.code)}</b> <span style="color:var(--ink-3);font-size:11.5px">${esc(x.o.name)}</span></td>
          <td style="${via.length ? "" : "color:var(--no)"}">${via.length ? via.join(", ") : "no CLO"}</td>
          <td style="white-space:normal">${x.o.members.map(m => esc(m.name)).join(", ")}</td>
          <td class="n">${fmt(x.o.fullMark, 0)}</td>
          <td class="n">${res.fullTotal ? fmt(x.o.fullMark / res.fullTotal * 100, 1) + "%" : "—"}</td>
          <td class="n">${x.o.tgt}%</td></tr>`;
      }).join("")}</tbody>
    </table></div>` : ""}
  </section>

  <section class="panel">
    <header><h2>Thresholds and grades</h2></header>
    <div class="body">
      <div class="grid2" style="margin-bottom:16px">
        <div><label class="f" for="stuT">A student attains an outcome at</label>
          <input id="stuT" type="number" min="1" max="100" step="1" data-fld="studentThreshold" value="${esc(c.studentThreshold)}">
          <p class="hint" style="margin:6px 0 0">Percent of the marks measuring that outcome. The CAM method uses 50.</p></div>
        <div><label class="f" for="defT">Default minimum for a new outcome</label>
          <input id="defT" type="number" min="1" max="100" step="1" data-fld="defaultTarget" value="${esc(c.defaultTarget)}">
          <p class="hint" style="margin:6px 0 0">The EAC form states an outcome is attained at 60% or above.</p></div>
      </div>
      <h3 style="font-size:13px;margin-bottom:8px">Grade boundaries</h3>
      <table style="max-width:340px"><thead><tr><th>Grade</th><th class="n">From (%)</th><th></th></tr></thead>
        <tbody id="gBody">${gradeRows}</tbody></table>
      <button class="btn sec sm" id="addG" style="margin-top:10px">Add grade</button>
    </div>
  </section>`;
}

/* ============================================================
   Views: marks, attainment
   ============================================================ */

function viewMarks(c, res) {
  const A = c.assessments;
  if (!A.length) return `<div class="empty"><h2>List the assessments first</h2>
    <p>The marks columns come from the assessments you define in Setup.</p>
    <button class="btn" style="margin-top:14px" data-go="setup">Go to setup</button></div>`;

  const head = A.map(a => `<th class="n">${esc(a.name)}<span class="sub">/ ${esc(a.fullMark)}</span></th>`).join("");
  const rows = (c.students || []).map((s, i) => {
    const r = res.rows.find(x => x.s.id === s.id);
    const cells = A.map((a, j) => {
      const v = s.marks?.[a.id];
      const num = Number(v);
      const bad = v !== "" && v != null && (!isFinite(num) || num < 0 || num > Number(a.fullMark) + 1e-9);
      return `<td class="n"><input class="cellin${bad ? " bad" : ""}" inputmode="decimal"
        data-si="${i}" data-aj="${j}" data-aid="${a.id}" value="${v == null ? "" : esc(v)}"
        aria-label="${esc(a.name)} mark for row ${i + 1}"></td>`;
    }).join("");
    return `<tr data-sid="${s.id}"${s.excluded ? ' style="opacity:.45"' : ""}>
      <td class="stick1 n" style="width:44px;color:var(--ink-3)">${i + 1}</td>
      <td class="stick2"><input class="txtin" style="min-width:104px" data-matric value="${esc(s.matric || "")}" aria-label="Matric number"></td>
      <td><input class="txtin" data-name value="${esc(s.name || "")}" aria-label="Student name"></td>
      ${cells}
      <td class="n divide js-total">${r ? fmt(r.total) : "—"}</td>
      <td class="n js-pct">${r ? fmt(r.totalPct) : "—"}</td>
      <td class="n js-grade" style="font-weight:600">${r ? esc(r.grade) : "—"}</td>
      <td style="width:46px;text-align:center"><input type="checkbox" data-sinc ${s.excluded ? "" : "checked"}
        style="accent-color:var(--action);cursor:pointer" aria-label="Count row ${i + 1} in the analysis"></td>
      <td style="width:38px"><button class="iconbtn" data-sdel aria-label="Remove row ${i + 1}">×</button></td>
    </tr>`;
  }).join("");

  return `
  <section class="panel">
    <header><h2>Marks</h2>
      <span class="note">${res.overall.n} counted${res.overall.excluded ? ` · ${res.overall.excluded} excluded` : ""}</span></header>
    <div class="body" style="padding-bottom:12px">
      <p class="hint">Type marks as awarded, out of each assessment's full mark. Paste a block straight from
        Excel into any cell and it fills across and down. Enter moves down, Tab moves across.</p>
      <div class="row">
        <button class="btn sec sm" id="addS">Add row</button>
        <button class="btn sec sm" id="add10">Add 10 rows</button>
        <button class="btn sec sm" id="impRoster">Paste roster</button>
        <button class="btn sec sm" id="impCsv">Import CSV</button>
        <span class="spacer"></span>
        <button class="btn sec sm" id="sortName">Sort by name</button>
        <button class="btn sec sm" id="sortMatric">Sort by matric</button>
        <button class="btn sec sm" id="resetBtn2">Reset…</button>
      </div>
    </div>
    <div class="scroll"><table>
      <thead><tr>
        <th class="stick1 n">#</th><th class="stick2">Matric</th><th>Name</th>${head}
        <th class="n divide">Total<span class="sub">/ ${fmt(res.fullTotal, 0)}</span></th>
        <th class="n">%</th><th class="n">Grade</th>
        <th style="text-align:center">Counts<span class="sub">in analysis</span></th><th></th>
      </tr></thead>
      <tbody id="mBody">${rows || `<tr><td colspan="${A.length + 8}" style="padding:26px;text-align:center;color:var(--ink-3)">No students yet. Add a row or paste a roster.</td></tr>`}</tbody>
      <tfoot id="mFoot">${rows ? marksFoot(res) : ""}</tfoot>
    </table></div>
  </section>

  <section class="panel" id="outPanel">
    <header><h2>Per outcome, per student</h2><span class="note">Derived — nothing to type here</span></header>
    <div class="scroll" id="outPanelBody" style="max-height:460px">${outTable(res)}</div>
  </section>`;
}

function marksFoot(res) {
  return `<tr>
      <td class="stick1"></td><td class="stick2">Reached ${res.baseT}% of the marks</td><td></td>
      ${res.cols.map(col => `<td class="n">${col.y}</td>`).join("")}
      <td class="n divide">${res.overall.passY}</td><td class="n"></td><td></td><td></td><td></td></tr>
    <tr><td class="stick1"></td><td class="stick2">Attainment Z (%)</td><td></td>
      ${res.cols.map(col => `<td class="n" style="color:${col.verdict ? "var(--yes)" : "var(--no)"}">${fmt(col.z)}</td>`).join("")}
      <td class="n divide">${fmt(res.overall.passZ)}</td><td class="n"></td><td></td><td></td><td></td></tr>`;
}

function outTable(res) {
  const os = res.outs.filter(x => x.o.fullMark > 0);
  if (!os.length) return `<p class="hint" style="padding:16px">No outcome has marks mapped to it yet.</p>`;
  return `<table>
    <thead><tr><th class="stick1 n">#</th><th class="stick2">Matric</th>
      ${os.map((x, i) => `<th class="n${i === 0 ? " divide" : ""}">${esc(x.o.code)}<span class="sub">/ ${fmt(x.o.fullMark, 0)}</span></th>`).join("")}
    </tr></thead>
    <tbody>${res.rows.map((r, i) => `<tr>
      <td class="stick1 n" style="color:var(--ink-3)">${i + 1}</td>
      <td class="stick2">${esc(r.s.matric || r.s.name || "")}</td>
      ${os.map((x, j) => {
        const v = r.oPct[x.key];
        const ok = v != null && v >= x.o.stuT;
        return `<td class="n${j === 0 ? " divide" : ""}" style="color:${v == null ? "var(--ink-3)" : ok ? "inherit" : "var(--no)"}">${fmt(v)}</td>`;
      }).join("")}</tr>`).join("")}</tbody>
    <tfoot><tr><td class="stick1"></td><td class="stick2">Y — students at or above the student threshold</td>
      ${os.map((x, j) => `<td class="n${j === 0 ? " divide" : ""}">${x.y}</td>`).join("")}</tr>
      <tr><td class="stick1"></td><td class="stick2">Z — attainment (%) against the minimum</td>
      ${os.map((x, j) => `<td class="n${j === 0 ? " divide" : ""}" style="color:${x.verdict ? "var(--yes)" : "var(--no)"};font-weight:600">${fmt(x.z)}<span style="color:var(--ink-3);font-weight:400"> / ${x.o.tgt}</span></td>`).join("")}</tr>
    </tfoot></table>`;
}

/* ---------------- attainment ---------------- */

const GRADE_COLORS = ["#0f6b52","#2b7f63","#4a9269","#6ea36b","#93ad6c","#b7ae64","#c89b4d","#cc8141","#c8673a","#bd4e34","#a8352a"];

function gaugeStrip(items) {
  if (!items.length) return `<p class="hint">Nothing mapped yet.</p>`;
  const tgt = items[0].o.tgt;
  const uniform = items.every(x => x.o.tgt === tgt);
  const rows = items.map(x => {
    const pct = clamp(x.z || 0, 0, 100);
    return `<div class="grow">
      <div class="gname">${esc(x.o.code)}<small>${x.y}/${x.n}</small></div>
      <div class="gtrack" role="img" aria-label="${esc(x.o.code)} attainment ${fmt(x.z)} percent against a required minimum of ${x.o.tgt} percent">
        <div class="gfill ${x.verdict ? "ok" : "bad"}" style="width:${pct}%"></div>
        ${uniform ? "" : `<div class="gmark" style="left:${clamp(x.o.tgt, 0, 100)}%"></div>`}
      </div>
      <div class="gval">${fmt(x.z)}%<span class="tag ${x.verdict ? "ok" : "bad"}">${x.verdict ? "attained" : "shortfall"}</span></div>
    </div>`;
  }).join("");
  return `<div class="gauge" style="--t:${tgt / 100}">
    ${uniform ? `<div class="gline"><b>${tgt}% needed</b></div>` : ""}
    ${rows}
    <div class="gscale"><span>0</span><span>50</span><span>100%</span></div>
    ${uniform ? "" : `<p class="hint" style="margin:8px 0 0">The required minimum differs between outcomes
      this semester, so each bar carries its own marker.</p>`}
  </div>`;
}

function viewAnalysis(c, res) {
  const n = res.overall.n;
  const withN = list => list.map(x => ({ ...x, n }));
  const issues = validate(c, res);
  const shortfalls = res.outs.filter(x => !x.verdict && x.o.fullMark > 0);

  const gradeOrder = res.gradeScale.map(g => g.grade).concat("F");
  const total = Object.values(res.gradeCount).reduce((a, b) => a + b, 0) || 1;
  const bar = gradeOrder.map((g, i) => {
    const k = res.gradeCount[g] || 0;
    if (!k) return "";
    return `<div style="width:${k / total * 100}%;background:${GRADE_COLORS[Math.min(i, GRADE_COLORS.length - 1)]}" title="${esc(g)}: ${k}">${k / total > .045 ? esc(g) : ""}</div>`;
  }).join("");
  const key = gradeOrder.map((g, i) => {
    const k = res.gradeCount[g] || 0; if (!k) return "";
    return `<span><i style="background:${GRADE_COLORS[Math.min(i, GRADE_COLORS.length - 1)]}"></i>${esc(g)} ${k}</span>`;
  }).join("");

  return `
  <section class="panel">
    <header><h2>Outcome attainment</h2>
      <span class="note">${esc(c.semester || "semester not recorded")} · ${n} student${n === 1 ? "" : "s"} · a student attains at ${res.baseT}%</span></header>
    <div class="body">
      <h3 style="font-size:13px;margin-bottom:4px">Course learning outcomes</h3>
      ${gaugeStrip(withN(res.clos))}
      <h3 style="font-size:13px;margin:22px 0 4px">Programme outcomes (EAC)</h3>
      ${gaugeStrip(withN(res.eacs))}
    </div>
    <div class="stats">
      <div class="stat"><b>${n}</b><span>students counted</span></div>
      <div class="stat"><b>${fmt(res.overall.meanPct, 1)}</b><span>mean total (%)</span></div>
      <div class="stat"><b>${fmt(res.overall.passZ, 1)}</b><span>passing the course (%)</span></div>
      <div class="stat"><b style="color:${shortfalls.length ? "var(--no)" : "var(--yes)"}">${shortfalls.length}</b><span>outcomes below the minimum</span></div>
    </div>
  </section>

  ${shortfalls.length ? `<section class="panel">
    <header><h2>Where the cohort fell short</h2><span class="note">Each needs a written action in section E or F</span></header>
    <div class="body">
      ${shortfalls.map(x => {
        const weak = res.cols.filter(col => x.o.members.some(m => m.id === col.a.id))
          .sort((a, b) => (a.z || 0) - (b.z || 0));
        return `<div style="padding:10px 0;border-bottom:1px solid var(--rule-soft)">
          <div class="row" style="gap:8px"><b>${esc(x.o.code)}</b>
            <span class="num" style="color:var(--no)">${fmt(x.z)}%</span>
            <span style="color:var(--ink-3);font-size:12.5px">against a required ${x.o.tgt}% · ${x.y} of ${n} students reached it</span></div>
          <p class="hint" style="margin:6px 0 0">Weakest contributing assessment:
            <b>${esc(weak[0] ? weak[0].a.name : "—")}</b>${weak[0] ? ` at ${fmt(weak[0].z)}% cohort attainment and a ${fmt(weak[0].meanPct, 1)}% mean` : ""}.</p>
        </div>`;
      }).join("")}
    </div>
  </section>` : ""}

  <section class="panel">
    <header><h2>Assessment by assessment</h2></header>
    <div class="scroll" style="max-height:none"><table>
      <thead><tr><th>Assessment</th><th>Delivery</th><th class="n">Marks</th><th class="n">Pass mark</th>
        <th class="n">Mean (%)</th><th class="n">Y</th><th class="n">Z (%)</th></tr></thead>
      <tbody>${res.cols.map(col => `<tr>
        <td>${esc(col.a.name)}</td><td style="color:var(--ink-3)">${esc(col.a.delivery || "")}</td>
        <td class="n">${esc(col.a.fullMark)}</td><td class="n">${fmt(col.cut)}</td>
        <td class="n">${fmt(col.meanPct)}</td><td class="n">${col.y}</td>
        <td class="n" style="font-weight:600">${fmt(col.z)}</td></tr>`).join("")}</tbody>
    </table></div>
  </section>

  <section class="panel">
    <header><h2>Grade spread</h2><span class="note">Total percentage against the grade boundaries</span></header>
    <div class="body">
      <div class="gradebar">${bar || `<div style="background:var(--surface-3);width:100%"></div>`}</div>
      <div class="gradekey">${key}</div>
    </div>
  </section>

  <section class="panel">
    <header><h2>Checks</h2><span class="note">Run on every change</span></header>
    <ul class="issues">${issues.map(i => `<li class="${i.level}">
      <span class="dot"></span><span>${esc(i.msg)}</span>${i.where ? `<span class="where">${esc(i.where)}</span>` : ""}</li>`).join("")}</ul>
  </section>`;
}

/* ============================================================
   The CAS form — narrative input and the printable documents
   ============================================================ */

function viewCas(c, res) {
  const cas = c.cas;
  const ta = (label, key, rows, ph) => `<div style="margin-bottom:14px">
    <label class="f" for="cas_${key}">${label}</label>
    <textarea id="cas_${key}" rows="${rows}" data-cas="${key}" placeholder="${esc(ph || "")}">${esc(cas[key] || "")}</textarea></div>`;

  const perOutcome = (list, bag, label) => list.length ? `<table><thead><tr>
      <th style="width:90px">${label}</th><th>Comments / recommendation</th></tr></thead>
    <tbody>${list.map(x => `<tr>
      <td style="vertical-align:top;padding-top:10px"><b>${esc(x.o.code)}</b><br>
        <span class="num" style="font-size:11px;color:${x.verdict ? "var(--yes)" : "var(--no)"}">${fmt(x.z)}%</span></td>
      <td><textarea rows="3" data-casmap="${bag}" data-oid="${esc(x.o.id)}"
        placeholder="${esc(x.verdict ? "What went well, and what to keep" : "Why the cohort fell short, and what will change")}"
        >${esc((c.cas[bag] || {})[x.o.id] || "")}</textarea></td></tr>`).join("")}</tbody></table>`
    : `<p class="hint">Nothing mapped yet.</p>`;

  return `
  <section class="panel">
    <header><span class="sectag">A</span><h2>Teaching plan</h2><span class="note">Section A</span></header>
    <div class="body">${ta("Note on the teaching plan attached to this summary", "teachingPlan", 2,
      "e.g. Teaching plan for Semester 1, 2025/2026 attached separately")}</div>
  </section>

  <section class="panel">
    <header><span class="sectag">B</span><h2>Review of the previous year's assessment</h2><span class="note">Section B</span></header>
    <div class="body">
      <p class="hint">Have the recommendations from the previous CAS been considered? If not, why not, and are
        they still valid?</p>
      ${ta("Comments", "prevReview", 5,
        "Based on the previous CAS, it was recommended that …  This recommendation has been considered this semester by …")}
    </div>
  </section>

  <section class="panel">
    <header><span class="sectag">D</span><h2>Alignment grid</h2><span class="note">Filled from the mapping</span></header>
    <div class="body">
      <p class="hint">Section D writes itself from the assessments, their delivery method and the CLO/EAC mapping.
        Change any of those in Setup and this changes with it.</p>
      ${casGridTable(c, res, false)}
    </div>
  </section>

  <section class="panel">
    <header><span class="sectag">E</span><h2>Comments on EAC attainment</h2><span class="note">Section E</span></header>
    <div class="body flush" style="padding:16px">${perOutcome(res.eacs, "eacComments", "EAC")}</div>
  </section>

  <section class="panel">
    <header><span class="sectag">F</span><h2>Comments on CLO attainment</h2><span class="note">Section F</span></header>
    <div class="body flush" style="padding:16px">${perOutcome(res.clos, "cloComments", "CLO")}</div>
  </section>

  <section class="panel">
    <header><span class="sectag">G</span><h2>Reflect on your teaching and learning</h2><span class="note">Section G</span></header>
    <div class="body">${ta("", "reflection", 5,
      "Students were exposed to … through discussion in class, mini project and the technical visit. Most students did well in …")}</div>
  </section>

  <section class="panel">
    <header><span class="sectag">H</span><h2>Overall recommendation</h2><span class="note">Section H</span></header>
    <div class="body">
      <p class="hint">Be specific enough that the recommendation can actually be carried out next semester.</p>
      ${ta("", "recommendation", 5,
        "It is suggested to continue or enhance the delivery methods such as …, to give more understanding to the students.")}
    </div>
  </section>

  <div class="row" style="margin-bottom:30px">
    <button class="btn" data-go="print">See the printable form</button>
    <button class="btn sec" data-go="analysis">Back to attainment</button>
  </div>`;
}

/* ---------------- section D grid ---------------- */

function casGridTable(c, res, paper) {
  const clos = res.clos, eacs = res.eacs;
  if (!clos.length || !eacs.length)
    return `<p class="hint">Add CLOs and tick the EACs this course carries to build the grid.</p>`;
  const cls = paper ? "" : ' class="paper" style="border:0;box-shadow:none;padding:0;background:transparent"';
  const cellStyle = paper ? "" : "";
  const body = eacs.map(e => `<tr>
      <th style="width:70px;text-align:center;vertical-align:middle">${esc(e.o.code)}</th>
      ${clos.map(cl => {
        const t = res.grid[e.o.id + "|" + cl.o.id];
        return `<td style="text-align:center;font-style:${t ? "italic" : "normal"};vertical-align:middle">${t ? esc(t) : ""}</td>`;
      }).join("")}
      <td class="c shade-b" style="vertical-align:middle;font-weight:600">${fmt(e.z)}%<br>${e.verdict ? "Y" : "N"}
        <div style="font-weight:400;font-size:8.6px;color:#444">min. ${e.o.tgt}%</div></td>
    </tr>`).join("");
  const foot = `<tr>
      <th class="c shade-o" style="vertical-align:middle">CO<br>Attainment</th>
      ${clos.map(cl => `<td class="c shade-o" style="vertical-align:middle;font-weight:600">${fmt(cl.z)}%<br>${cl.verdict ? "Y" : "N"}
        <div style="font-weight:400;font-size:8.6px;color:#444">min. ${cl.o.tgt}%</div></td>`).join("")}
      <td class="shade-o"></td></tr>`;
  const tbl = `<table${paper ? "" : ' style="font-size:12px"'}>
    <thead><tr><th></th>${clos.map(cl => `<th class="c">${esc(cl.o.code)}</th>`).join("")}
      <th class="c shade-b">PO Attainment</th></tr></thead>
    <tbody>${body}${foot}</tbody></table>`;
  return paper ? tbl : `<div class="scroll" style="max-height:none">${tbl.replace("<table", '<table class="paper-in"')}</div>`;
}

/* ---------------- the printable CAS form ---------------- */

function paperHead(runner) {
  return `<div class="ph ${runner ? "runhead" : "dup"}">
    <div class="logo"><img src="${CREST}" alt="Universiti Putra Malaysia"></div>
    <div class="txt">
      <div class="t1">PERKHIDMATAN UTAMA PRASISWAZAH<br>FAKULTI KEJURUTERAAN
        <span class="doc">Kod Dokumen: PU/PS/FK/CAS</span></div>
      <div class="t2">BORANG RINGKASAN PENILAIAN KURSUS<i>(COURSE ASSESSMENT SUMMARY)</i></div>
    </div></div>`;
}
function paperFoot(runner) {
  return `<div class="pf ${runner ? "runfoot" : "dup"}"><span>NO. SEMAKAN&nbsp;&nbsp;:&nbsp;&nbsp;02</span><br>
    <span>NO. ISU&nbsp;&nbsp;:&nbsp;&nbsp;01</span><br>
    <span>TARIKH KUATKUASA&nbsp;&nbsp;:&nbsp;&nbsp;16/07/2025</span></div>`;
}

function casDoc(c, res) {
  const cas = c.cas || {};
  const tick = v => v ? "√" : "&nbsp;&nbsp;";
  const c21 = c.curriculum !== "2016-2020";

  const meta = `<table>
    <tr><td style="width:120px"><b>Programme&nbsp;:</b></td><td colspan="3"><b>${esc(c.programme)}</b></td></tr>
    <tr><td><b>Department:</b></td><td colspan="3"><b>${esc(c.department)}</b></td></tr>
    <tr><td>Course Name:</td><td style="width:33%">${esc(c.courseName)}</td>
        <td style="width:16%">Semester/Session:</td><td>${esc(c.semester)}</td></tr>
    <tr><td>Course Code:</td><td>${esc(c.courseCode)}</td><td>Lecturer:</td><td>${esc(c.lecturer)}</td></tr>
    <tr><td>Group :</td><td colspan="3">${esc(c.group)}</td></tr>
    <tr><td>Curriculum <b>(Tick)</b></td><td colspan="3">2016 – 2020 (&nbsp;${tick(!c21)}&nbsp;)
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2021 – 2025 (&nbsp;${tick(c21)}&nbsp;)</td></tr>
  </table>`;

  const closList = `<table>${c.clos.map(o => `<tr>
      <td style="width:60px;text-align:center;vertical-align:middle"><b>${esc(o.code)}</b></td>
      <td>${esc(o.desc || "—")}${o.taxonomy ? " (" + esc(o.taxonomy) + ")" : ""}</td></tr>`).join("")}</table>`;

  const eacTick = `<table>
    <tr><th class="c shade-g" style="width:56px">*EAC</th>
      ${c.eacs.map(e => `<th class="c shade-g">${esc(e.code)}<br>(${esc(e.taxonomy)})</th>`).join("")}</tr>
    <tr><td class="c">Tick<br>( √ )</td>
      ${c.eacs.map(e => `<td class="c" style="height:22px;font-size:12px">${
        c.assessments.some(a => (a.eacs || []).includes(e.id)) ? "√" : ""}</td>`).join("")}</tr>
  </table>
  <p style="font-size:9px;margin:-4px 0 8px">*Note: EACxx is the code for Programme Outcomes in 2021 – 2025 Curriculum</p>`;

  const deliveryLines = res.clos.map(cl => {
    const eacCodes = res.eacs.filter(e => res.grid[e.o.id + "|" + cl.o.id]).map(e => e.o.code);
    const items = c.assessments.filter(a => (a.clos || []).includes(cl.o.id));
    if (!items.length) return "";
    const byDelivery = {};
    items.forEach(a => {
      const d = a.delivery || "Lecture";
      (byDelivery[d] = byDelivery[d] || []).push(
        `${a.name} (${fmt(res.fullTotal > 0 ? a.fullMark / res.fullTotal * 100 : 0, 0)}%)`);
    });
    return Object.entries(byDelivery).map(([d, list]) =>
      `${d} | ${list.join(", ")}`).join("; ") +
      ` &nbsp;for ${esc(cl.o.code)}${eacCodes.length ? "-" + eacCodes.join("/") : ""}`;
  }).filter(Boolean);

  const commentTable = (list, bag, label) => `<table>
    <tr><th style="width:74px">${label}</th><th>Comments/ Recommendation</th></tr>
    ${list.map(x => `<tr><td style="vertical-align:top">${esc(x.o.code)}</td>
      <td>${nl2br((cas[bag] || {})[x.o.id] || "")}</td></tr>`).join("")}</table>`;

  const eacDesc = `<h3>Description of Programme Outcomes :</h3>
    <table>
      <tr><th class="c shade-g" style="width:130px">EAC</th>
        <th class="c shade-g">CURRICULUM 2021 – 2025<br>(DESCRIPTION OF 11 POs)</th></tr>
      ${c.eacs.map(e => `<tr>
        <td class="c"><b>${esc(e.code)} (${esc(e.taxonomy)})</b><br><i>${esc(e.name)}</i></td>
        <td style="text-align:justify">${esc(e.desc)}${e.wk ? ` <b>(${esc(e.wk)})</b>` : ""}</td></tr>`).join("")}
    </table>`;

  return `<article class="paper" id="casPaper">
    <table class="runner"><thead><tr><th>${paperHead(true)}</th></tr></thead><tbody><tr><td>
    ${meta}
    <div class="cas-sec"><div class="lt">A</div><div class="ct">
      <p>Attach Teaching Plan</p>${cas.teachingPlan ? `<p><i>${nl2br(cas.teachingPlan)}</i></p>` : ""}</div></div>
    <div class="cas-sec"><div class="lt">B</div><div class="ct">
      <p>Review of previous year's assessment (Review comments in the previous year's CAS). Have the recommended
        changes been considered? If not, why not? Are the recommended changes still valid?</p>
      <table><tr><td style="width:84px">Comments:</td>
        <td class="hl">${nl2br(cas.prevReview || "")}</td></tr></table></div></div>
    <div class="cas-sec"><div class="lt">C</div><div class="ct">
      <p><i>a) List the specified Course Outcomes (with taxonomy levels).</i></p>
      ${closList}
      <p><i>b) Tick the assigned Programme Outcomes.</i></p>
      <p><i>Curriculum 2021 – 2025 (11 POs)</i></p>
      ${eacTick}</div></div>
    <div class="cas-sec"><div class="lt">D</div><div class="ct">
      <p>Alignment between Teaching Delivery, Assessment Method and Outcomes, and Programs &amp; Course Outcomes Attainment</p>
      <p style="margin-left:14px"><i>a) &nbsp;Fill in <span class="hl">Teaching Delivery | Assessment Method (Marks (%))</span> for each assigned CO-PO mapping.</i></p>
      <div style="margin-left:34px;font-style:italic">${deliveryLines.map(l => `<div>${l}</div>`).join("")}</div>
      <p style="margin-left:34px" class="hl"><i>NOTE: Total Marks of All Assessments must be 100%
        — currently ${fmt(res.fullTotal, 1)}%</i></p>
      <p style="margin-left:14px"><i>b) &nbsp;Fill in PO attainment percentage (in %) and its status (either Y (Yes) or N (No)) based on CAM.</i></p>
      <p style="margin-left:34px" class="hl"><i>Note: PO attainment status is "Y" if its attainment equals or is greater than the required minimum</i></p>
      <p style="margin-left:14px"><i>c) &nbsp;Fill in CO attainment percentage (in %) and its status (either Y (Yes) or N (No)) based on CAM.</i></p>
      <p style="margin-left:34px" class="hl"><i>Note: CO attainment status is "Y" if its attainment equals or is greater than the required minimum</i></p>
      ${casGridTable(c, res, true)}</div></div>
    <div class="cas-sec"><div class="lt">E</div><div class="ct">
      <p><i>Give comments and recommendation based on POs attainments and Results in CAM.</i></p>
      ${commentTable(res.eacs, "eacComments", "PO")}</div></div>
    <div class="cas-sec"><div class="lt">F</div><div class="ct">
      <p><i>Give comments and recommendation based on COs attainments</i></p>
      ${commentTable(res.clos, "cloComments", "CO")}</div></div>
    <div class="cas-sec"><div class="lt">G</div><div class="ct">
      <p class="hl"><i>Reflect on your Teaching and Learning:</i></p>
      <p>${nl2br(cas.reflection || "")}</p></div></div>
    <div class="cas-sec"><div class="lt">H</div><div class="ct">
      <p class="hl"><i>State Overall Recommendation (be specific in the recommendation so that it can be executed):</i></p>
      <p>${nl2br(cas.recommendation || "")}</p></div></div>

    <div class="sign">
      <div><div>Prepared by:</div><div>(Lecturer's signature &amp; stamp)</div>
        <div class="line"></div><div>Date: ____________________</div></div>
      <div><div>Approved by:</div><div>(Head of Department's signature &amp; stamp)</div>
        <div class="line"></div><div>Date: ____________________</div></div>
    </div>
    ${paperFoot(true)}
    </td></tr></tbody></table>
    <div class="pagebreak" style="padding-top:2px">
      <table class="runner"><thead><tr><th>${paperHead(true)}</th></tr></thead><tbody><tr><td>
      ${eacDesc}${paperFoot(true)}</td></tr></tbody></table></div>
  </article>`;
}

/* ---------------- the printable CAM sheet ---------------- */

function camDoc(c, res) {
  const A = c.assessments;
  const os = res.outs.filter(x => x.o.fullMark > 0);
  const marks = `<table>
    <thead><tr><th class="n">No</th><th>Matric</th><th>Name</th>
      ${A.map(a => `<th class="n">${esc(a.name)}<br><span style="font-weight:400">/${esc(a.fullMark)}</span></th>`).join("")}
      <th class="n">Total</th><th class="n">%</th><th class="c">Grade</th>
      ${os.map(x => `<th class="n">${esc(x.o.code)}</th>`).join("")}</tr></thead>
    <tbody>${res.rows.map((r, i) => `<tr><td class="n">${i + 1}</td><td>${esc(r.s.matric || "")}</td>
      <td>${esc(r.s.name || "")}</td>
      ${A.map(a => `<td class="n">${r.s.marks?.[a.id] == null || r.s.marks[a.id] === "" ? "" : fmt(Number(r.s.marks[a.id]), 1)}</td>`).join("")}
      <td class="n">${fmt(r.total, 1)}</td><td class="n">${fmt(r.totalPct, 1)}</td><td class="c">${esc(r.grade)}</td>
      ${os.map(x => `<td class="n">${fmt(r.oPct[x.key], 1)}</td>`).join("")}</tr>`).join("")}</tbody>
    <tfoot><tr><td colspan="3"><b>Y</b> — students reaching ${res.baseT}% of the marks</td>
      ${res.cols.map(col => `<td class="n">${col.y}</td>`).join("")}
      <td class="n">${res.overall.passY}</td><td class="n"></td><td></td>
      ${os.map(x => `<td class="n">${x.y}</td>`).join("")}</tr>
    <tr><td colspan="3"><b>Z</b> — attainment (%), Y / ${res.overall.n} × 100</td>
      ${res.cols.map(col => `<td class="n">${fmt(col.z, 1)}</td>`).join("")}
      <td class="n">${fmt(res.overall.passZ, 1)}</td><td class="n"></td><td></td>
      ${os.map(x => `<td class="n">${fmt(x.z, 1)}</td>`).join("")}</tr>
    <tr><td colspan="3">Attained (Z ≥ the minimum)</td>
      ${res.cols.map(() => `<td></td>`).join("")}<td></td><td></td><td></td>
      ${os.map(x => `<td class="c" style="font-weight:700">${x.verdict ? "Y" : "N"}</td>`).join("")}</tr>
    </tfoot></table>`;

  return `<article class="paper" id="camPaper">
    <table class="runner"><thead><tr><th>${paperHead(true)}</th></tr></thead><tbody><tr><td>
    <h3 style="text-align:center;font-size:12px;margin-bottom:8px">COURSE ASSESSMENT MATRIX (CAM)</h3>
    <table>
      <tr><td style="width:110px">Semester/Session:</td><td>${esc(c.semester)}</td>
          <td style="width:90px">Course Code:</td><td>${esc(c.courseCode)}</td></tr>
      <tr><td>Course Name:</td><td>${esc(c.courseName)}</td><td>Lecturer:</td><td>${esc(c.lecturer)}</td></tr>
      <tr><td>Group:</td><td>${esc(c.group)}</td><td>No. of students:</td><td>${res.overall.n}</td></tr>
    </table>
    <table>
      <thead><tr><th>Outcome</th><th>Measured by</th><th class="n">Marks</th>
        <th class="n">Y</th><th class="n">Z (%)</th><th class="n">Minimum</th><th class="c">Attained</th></tr></thead>
      <tbody>${os.map(x => `<tr><td><b>${esc(x.o.code)}</b></td>
        <td>${x.o.members.map(m => esc(m.name)).join(", ")}</td>
        <td class="n">${fmt(x.o.fullMark, 0)}</td><td class="n">${x.y}</td>
        <td class="n"><b>${fmt(x.z)}</b></td><td class="n">${x.o.tgt}</td>
        <td class="c" style="font-weight:700">${x.verdict ? "Y" : "N"}</td></tr>`).join("")}</tbody>
    </table>
    <h3 style="margin-top:10px">Marks and individual attainment</h3>
    ${marks}
    <div class="sign">
      <div><div>Prepared by:</div><div>(Lecturer's signature &amp; stamp)</div>
        <div class="line"></div><div>Date: ____________________</div></div>
      <div><div>Approved by:</div><div>(Head of Department's signature &amp; stamp)</div>
        <div class="line"></div><div>Date: ____________________</div></div>
    </div>
    ${paperFoot(true)}
    </td></tr></tbody></table>
  </article>`;
}

/* ---------------- print view ---------------- */

function viewPrint(c, res) {
  const errs = validate(c, res).filter(i => i.level === "err");
  const which = S.doc === "cam" ? camDoc(c, res) : casDoc(c, res);
  return `
  ${errs.length ? `<section class="panel noprint" style="border-color:var(--no)">
    <header style="background:var(--no-bg)"><h2 style="color:var(--no)">Fix before signing</h2></header>
    <ul class="issues">${errs.map(i => `<li class="err"><span class="dot"></span><span>${esc(i.msg)}</span>
      <span class="where">${esc(i.where)}</span></li>`).join("")}</ul>
  </section>` : ""}
  <div class="docbar noprint">
    <div class="row">
      <button class="btn${S.doc === "cas" ? "" : " sec"}" data-doc="cas">CAS form</button>
      <button class="btn${S.doc === "cam" ? "" : " sec"}" data-doc="cam">CAM sheet</button>
      <span style="width:12px"></span>
      <button class="btn sec" id="printBtn">Print</button>
      <button class="btn sec" id="dlDoc">Download (.html)</button>
      <span class="spacer"></span>
      <span style="font-size:12px;color:var(--ink-3)">A4 · ${new Date().toLocaleDateString()}</span>
    </div>
  </div>
  ${which}`;
}

/* ============================================================
   Data management, interaction and startup
   ============================================================ */

function viewData(c, res) {
  const size = new Blob([JSON.stringify(c)]).size;
  const noXl = typeof XLSX === "undefined";
  return `
  <section class="panel">
    <header><h2>Export</h2><span class="note">Marks and analysis leave in open formats</span></header>
    <div class="body">
      <p class="hint">The workbook rebuilds the familiar CAM sheet with live Excel formulas, so every figure
        stays checkable after it leaves here.</p>
      <div class="row">
        <button class="btn" id="exXlsx"${noXl ? " disabled" : ""}>Workbook (.xlsx)</button>
        <button class="btn sec" id="exMarks">Marks (.csv)</button>
        <button class="btn sec" id="exAnalysis">Analysis (.csv)</button>
        <button class="btn sec" id="exJson">Backup this course (.json)</button>
      </div>
      ${noXl ? `<p class="hint" style="margin:10px 0 0;color:var(--warn)">The workbook library did not load in
        this view, so the .xlsx export is unavailable. The CSV exports carry the same figures.</p>` : ""}
    </div>
  </section>

  <section class="panel">
    <header><h2>Import</h2></header>
    <div class="body">
      <p class="hint">A CSV needs a matric column and a name column; the remaining columns are matched to
        assessment names, or taken left to right when the headers don't match.</p>
      <div class="row">
        <button class="btn sec" id="impCsv2">Import marks from CSV</button>
        <button class="btn sec" id="impJson">Restore a backup (.json)</button>
      </div>
    </div>
  </section>

  <section class="panel">
    <header><h2>Next semester</h2><span class="note">Set up once, run every semester</span></header>
    <div class="body">
      <p class="hint">Duplicating keeps the assessments, outcomes, mapping and minimums and clears the roster,
        so the next semester starts from a structure that has already been checked. The minimums stay editable,
        because each semester sets its own.</p>
      <div class="row">
        <button class="btn sec" id="dupEmpty">Duplicate without students</button>
        <button class="btn sec" id="dupFull">Duplicate with students</button>
      </div>
    </div>
  </section>

  <section class="panel">
    <header><h2>Reset</h2><span class="note">Start a section over</span></header>
    <div class="body">
      <p class="hint">Clear last semester's figures without rebuilding the course. Useful when the same course
        runs again and only the roster and marks change.</p>
      <div class="row">
        <button class="btn sec" id="resetBtn">Clear data…</button>
      </div>
    </div>
  </section>

  <section class="panel">
    <header><h2>This course</h2></header>
    <div class="body">
      <dl style="display:grid;grid-template-columns:auto 1fr;gap:5px 14px;font-size:13px;margin:0 0 16px">
        <dt style="color:var(--ink-3)">Stored in</dt><dd style="margin:0">${Store.mode === "db" ? "Shared storage for this app" : "This browser only"}</dd>
        <dt style="color:var(--ink-3)">Last change</dt><dd style="margin:0">${c.updated ? new Date(c.updated).toLocaleString() : "—"}</dd>
        <dt style="color:var(--ink-3)">Record size</dt><dd style="margin:0" class="num">${(size / 1024).toFixed(1)} KB</dd>
        <dt style="color:var(--ink-3)">Rows</dt><dd style="margin:0" class="num">${(c.students || []).length}</dd>
      </dl>
      ${Store.mode !== "db" ? `<p class="hint" style="color:var(--warn)">Shared storage is unavailable in this
        view, so courses are kept in this browser only. Download a backup before clearing browsing data.</p>` : ""}
      <button class="btn danger" id="delCourse">Delete this course</button>
    </div>
  </section>`;
}

/* ---------------- targeted refresh so typing never loses focus ---------------- */
function softRefresh() {
  const c = course(); if (!c || S.view !== "marks") return;
  const res = calc(c);
  $$("#mBody tr[data-sid]").forEach(tr => {
    const r = res.rows.find(x => x.s.id === tr.dataset.sid);
    const t = $(".js-total", tr), p = $(".js-pct", tr), g = $(".js-grade", tr);
    if (t) t.textContent = r ? fmt(r.total) : "—";
    if (p) p.textContent = r ? fmt(r.totalPct) : "—";
    if (g) g.textContent = r ? r.grade : "—";
  });
  const foot = $("#mFoot"); if (foot) foot.innerHTML = marksFoot(res);
  const op = $("#outPanelBody"); if (op) op.innerHTML = outTable(res);
}

function newCourse() {
  const spare = S.courses.find(isPristine);          // don't stack up blank records
  if (spare) {
    S.activeId = spare.id; S.view = "setup"; render();
    toast("Opened the empty course you already had");
    return;
  }
  const c = blankCourse();
  S.courses.push(c); S.activeId = c.id; S.view = "setup";
  Store.save(c).catch(() => {}); render();
}

function setView(v) {
  S.view = v;
  try { localStorage.setItem("cas.view", v); } catch (e) {}
  render();
}

/* ---------------- dialogs ---------------- */
function dialog(title, bodyHTML, buttons) {
  const d = $("#dlg");
  $("#dlgTitle").textContent = title;
  $("#dlgBody").innerHTML = bodyHTML;
  $("#dlgFoot").innerHTML = "";
  (buttons || [{ label: "Close" }]).forEach(b => {
    const el = document.createElement("button");
    el.className = "btn" + (b.primary ? "" : " sec");
    el.textContent = b.label;
    el.onclick = () => { const keep = b.onClick && b.onClick(d); if (!keep) d.close(); };
    $("#dlgFoot").appendChild(el);
  });
  d.showModal();
  const first = $("#dlgBody input, #dlgBody textarea");
  if (first) first.focus();
  return d;
}
function openReset(c) {
  const n = (c.students || []).length;
  const marked = (c.students || []).reduce((t, s2) =>
    t + Object.values(s2.marks || {}).filter(v => v !== null && v !== undefined && v !== "").length, 0);
  const cas = c.cas || {};
  const written = ["prevReview", "teachingPlan", "reflection", "recommendation"].filter(k => (cas[k] || "").trim()).length
    + Object.values(cas.eacComments || {}).filter(v => (v || "").trim()).length
    + Object.values(cas.cloComments || {}).filter(v => (v || "").trim()).length;
  const opt = (v, label, desc, warn) => `<label class="opt${warn ? " warn" : ""}">
    <input type="radio" name="resetWhat" value="${v}"${v === "marks" ? " checked" : ""}>
    <span style="min-width:0"><b>${label}</b><span>${desc}</span></span></label>`;

  dialog("Reset data", `
    <p class="hint">Clearing cannot be undone. Download a backup from the Data tab first if you might want
      these figures again.</p>
    <div class="opts">
      ${opt("marks", "Marks only", `Blanks ${marked} mark${marked === 1 ? "" : "s"} and keeps the ${n} student row${n === 1 ? "" : "s"}, the assessments, the outcomes and the CAS narrative.`)}
      ${opt("roster", "Roster and marks", `Removes all ${n} student row${n === 1 ? "" : "s"}. The course structure stays, ready for the next intake.`)}
      ${opt("cas", "CAS narrative", `Clears the ${written} written section${written === 1 ? "" : "s"} — A, B, E, F, G and H. Marks and attainment are untouched.`)}
      ${opt("structure", "Assessments and outcomes", "Removes the assessments, the CLOs and every EAC assignment, along with the marks that depended on them. Course details and the roster stay.")}
      ${opt("all", "Everything in this course", "Back to an empty form. Only the course record itself survives.", true)}
    </div>`,
    [{ label: "Cancel" },
     { label: "Clear", primary: true, onClick: d => {
        const pick = $('input[name="resetWhat"]:checked', d);
        doReset(c, pick ? pick.value : "marks");
      } }]);
}

function doReset(c, what) {
  if (what === "marks") {
    (c.students || []).forEach(s2 => { s2.marks = {}; });
    toast("Marks cleared");
  } else if (what === "roster") {
    c.students = [];
    toast("Roster cleared");
  } else if (what === "cas") {
    c.cas = { prevReview: "", teachingPlan: "", eacComments: {}, cloComments: {}, reflection: "", recommendation: "" };
    toast("CAS narrative cleared");
  } else if (what === "structure") {
    c.assessments = [{ id: uid("a"), name: "Test 1", fullMark: 100, delivery: "Lecture", clos: [], eacs: [] }];
    c.clos = [{ id: uid("o"), code: "CO1", desc: "", taxonomy: "", target: c.defaultTarget, studentThreshold: null }];
    c.eacs = newEacSet(c.defaultTarget);
    (c.students || []).forEach(s2 => { s2.marks = {}; });
    c.cas.eacComments = {}; c.cas.cloComments = {};
    S.view = "setup";
    toast("Assessments and outcomes cleared");
  } else if (what === "all") {
    const fresh = blankCourse();
    fresh.id = c.id;
    const i = S.courses.findIndex(x => x.id === c.id);
    if (i >= 0) S.courses[i] = fresh;
    S.view = "setup";
    toast("Course reset");
  }
  markDirty(); flush(); render();
}

function confirmDo(title, body, fn) {
  dialog(title, `<p class="hint" style="margin:0">${esc(body)}</p>`,
    [{ label: "Cancel" }, { label: "Delete", primary: true, onClick: () => fn() }]);
}

/* ---------------- file out ---------------- */
let _dl;
async function saveFile(filename, data, mime) {
  if (_dl === undefined) {
    try { _dl = (window.claude && window.claude.use) ? await window.claude.use("downloads") : null; }
    catch (e) { _dl = null; }
  }
  if (_dl) {
    try { await _dl.save({ filename, data }); toast("Saved " + filename); return; }
    catch (e) {
      if (e && e.code === "declined") return;
      if (e && (e.code === "rejected_extension" || e.code === "bad_request")) { toast("Could not save " + filename); return; }
    }
  }
  try {
    const blob = data instanceof Blob ? data : new Blob([data], { type: mime || "text/plain;charset=utf-8" });
    const url = URL.createObjectURL(blob);
    const a = document.createElement("a");
    a.href = url; a.download = filename; document.body.appendChild(a); a.click();
    setTimeout(() => { URL.revokeObjectURL(url); a.remove(); }, 1500);
    toast("Saved " + filename); return;
  } catch (e) {}
  if (typeof data === "string") {
    dialog("Copy " + filename, `<p class="hint">Downloads are unavailable here. Select everything below and copy it into a file.</p>
      <textarea rows="12" spellcheck="false">${esc(data)}</textarea>`,
      [{ label: "Copy", primary: true, onClick: d => { const t = $("textarea", d); t.select(); document.execCommand("copy"); toast("Copied"); return true; } },
       { label: "Close" }]);
  } else toast("Downloads are unavailable in this view.");
}

const fileStem = c => (c.courseCode || "course").replace(/[^\w.-]+/g, "_") +
  (c.group ? "-G" + String(c.group).replace(/[^\w.-]+/g, "") : "");

function standaloneDoc(c, res, which) {
  const css = Array.from(document.styleSheets).filter(s => !s.href)
    .map(s => { try { return Array.from(s.cssRules).map(r => r.cssText).join("\n"); } catch (e) { return ""; } }).join("\n");
  const inner = which === "cam" ? camDoc(c, res) : casDoc(c, res);
  return `<!doctype html><html lang="en"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>${esc(c.courseCode || "")} ${which === "cam" ? "CAM" : "CAS"}</title>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>${css}
body{background:#fff;padding:0;margin:0}
.paper{margin:0 auto;box-shadow:none;border:0}
@media screen{body{background:#eaf0f7;padding:18px}.paper{box-shadow:0 2px 14px rgba(10,35,66,.2);background:#fff}}
</style></head><body>${inner}</body></html>`;
}

/* ---------------- CSV ---------------- */
function toCSV(rows) {
  return rows.map(r => r.map(v => {
    const s = v == null ? "" : String(v);
    return /[",\n]/.test(s) ? '"' + s.replace(/"/g, '""') + '"' : s;
  }).join(",")).join("\r\n");
}
function parseCSV(text) {
  const rows = []; let row = [], cell = "", q = false;
  text = text.replace(/\r\n?/g, "\n");
  for (let i = 0; i < text.length; i++) {
    const ch = text[i];
    if (q) { if (ch === '"') { if (text[i + 1] === '"') { cell += '"'; i++; } else q = false; } else cell += ch; }
    else if (ch === '"') q = true;
    else if (ch === ",") { row.push(cell); cell = ""; }
    else if (ch === "\n") { row.push(cell); rows.push(row); row = []; cell = ""; }
    else cell += ch;
  }
  if (cell !== "" || row.length) { row.push(cell); rows.push(row); }
  return rows.filter(r => r.some(v => String(v).trim() !== ""));
}

function exportMarksCSV(c, res) {
  const os = res.outs.filter(x => x.o.fullMark > 0);
  const head = ["No", "Matric", "Name", ...c.assessments.map(a => `${a.name} (/${a.fullMark})`),
    "Total", "Percent", "Grade", ...os.map(x => x.o.code + " %"), "Counted"];
  const body = res.rows.map((r, i) => [i + 1, r.s.matric || "", r.s.name || "",
    ...c.assessments.map(a => r.s.marks?.[a.id] ?? ""),
    r.total, r.totalPct, r.grade, ...os.map(x => r.oPct[x.key]), "yes"]);
  (c.students || []).filter(s => s.excluded).forEach(s => body.push(["", s.matric || "", s.name || "",
    ...c.assessments.map(a => s.marks?.[a.id] ?? ""), "", "", "", ...os.map(() => ""), "no"]));
  saveFile(fileStem(c) + "-marks.csv", toCSV([head, ...body]), "text/csv");
}

function exportAnalysisCSV(c, res) {
  const rows = [
    ["Course Assessment Summary"], ["Programme", c.programme], ["Department", c.department],
    ["Semester/Session", c.semester], ["Course code", c.courseCode], ["Course name", c.courseName],
    ["Lecturer", c.lecturer], ["Group", c.group], ["Curriculum", c.curriculum],
    ["Students counted", res.overall.n], ["Student attainment threshold (%)", res.baseT], [],
    ["Outcome", "Kind", "Measured by", "Marks", "Y", "Z (%)", "Min. attainment (%)", "Attained"],
    ...res.outs.filter(x => x.o.fullMark > 0).map(x =>
      [x.o.code, x.o.kind, x.o.members.map(m => m.name).join(" + "), x.o.fullMark, x.y, x.z, x.o.tgt, x.verdict ? "Y" : "N"]),
    [],
    ["Assessment", "Delivery", "Marks", "Pass mark", "Mean (%)", "Y", "Z (%)"],
    ...res.cols.map(col => [col.a.name, col.a.delivery, col.a.fullMark, col.cut, col.meanPct, col.y, col.z]),
    [], ["Grade", "Students"], ...Object.entries(res.gradeCount).sort()
  ];
  saveFile(fileStem(c) + "-analysis.csv", toCSV(rows), "text/csv");
}

/* ---------------- workbook with live formulas ---------------- */
function colLetter(n) { let s = ""; while (n > 0) { const m = (n - 1) % 26; s = String.fromCharCode(65 + m) + s; n = (n - m - 1) / 26; } return s; }

function exportXLSX(c, res) {
  if (typeof XLSX === "undefined") { toast("Workbook export is unavailable here — use the CSV instead."); return; }
  const A = c.assessments, outs = res.outs.filter(x => x.o.fullMark > 0);
  const ws = {}; const put = (r, cn, cell) => { if (cell) ws[colLetter(cn) + r] = cell; };
  const S_ = v => ({ t: "s", v: String(v == null ? "" : v) });
  const N_ = v => ({ t: "n", v: Number(v) || 0 });
  const FN = (f, v) => ({ t: "n", f, v: Number(v) || 0 });
  const FS = (f, v) => ({ t: "s", f, v: String(v == null ? "" : v) });

  put(1, 1, S_("COURSE ASSESSMENT MATRIX — CLO / EAC ATTAINMENT"));
  const meta = [["SEMESTER/SESSION", c.semester], ["COURSE NAME", c.courseName], ["COURSE CODE", c.courseCode],
    ["LECTURER", c.lecturer], ["GROUP", c.group], ["NO. OF STUDENTS", res.overall.n]];
  meta.forEach((m, i) => { put(3 + i, 1, S_(m[0])); put(3 + i, 2, i === 5 ? N_(m[1]) : S_(m[1])); });
  const nRef = "$B$8";

  const C0 = 4;
  const cTotal = C0 + A.length, cPct = cTotal + 1, cGrade = cPct + 1, cOut = cGrade + 1;
  const HR = 11, FR = 12, R0 = 13;
  const RN = R0 + Math.max(res.rows.length, 1) - 1;

  put(HR, 1, S_("No")); put(HR, 2, S_("Matric")); put(HR, 3, S_("Name"));
  A.forEach((a, i) => put(HR, C0 + i, S_(a.name)));
  put(HR, cTotal, S_("TOTAL")); put(HR, cPct, S_("PERCENT")); put(HR, cGrade, S_("GRADE"));
  outs.forEach((x, i) => put(HR, cOut + i, S_(x.o.code + " %")));

  put(FR, 3, S_("FULL MARKS"));
  A.forEach((a, i) => put(FR, C0 + i, N_(a.fullMark)));
  put(FR, cTotal, N_(res.fullTotal));
  outs.forEach((x, i) => {
    const terms = x.o.members.map(m => colLetter(C0 + A.indexOf(m)) + FR).join("+");
    put(FR, cOut + i, terms ? FN(terms, x.o.fullMark) : N_(0));
  });

  const gs = res.gradeScale;
  res.rows.forEach((r, ri) => {
    const R = R0 + ri;
    put(R, 1, N_(ri + 1)); put(R, 2, S_(r.s.matric)); put(R, 3, S_(r.s.name));
    A.forEach((a, i) => put(R, C0 + i, N_(r.s.marks?.[a.id])));
    put(R, cTotal, FN(`SUM(${colLetter(C0)}${R}:${colLetter(C0 + A.length - 1)}${R})`, r.total));
    put(R, cPct, FN(`ROUND(${colLetter(cTotal)}${R}/${colLetter(cTotal)}$${FR}*100,2)`, r.totalPct));
    const pc = colLetter(cPct) + R;
    let g = '"F"';
    for (let i = gs.length - 1; i >= 0; i--) g = `IF(${pc}>=${gs[i].min},"${gs[i].grade}",${g})`;
    put(R, cGrade, FS(g, r.grade));
    outs.forEach((x, i) => {
      const terms = x.o.members.map(m => colLetter(C0 + A.indexOf(m)) + R).join("+");
      put(R, cOut + i, FN(`ROUND((${terms})/${colLetter(cOut + i)}$${FR}*100,2)`, r.oPct[x.key]));
    });
  });

  const rY = RN + 2, rZ = RN + 3, rT = RN + 4, rV = RN + 5;
  put(rY, 3, S_(`Y — students reaching ${res.baseT}% of the marks`));
  put(rZ, 3, S_("Z — attainment (%) = Y / students × 100"));
  put(rT, 3, S_("Minimum attainment required this semester (%)"));
  put(rV, 3, S_("Attained (Z ≥ the minimum)"));
  const band = (cn, cut, y, z, tgt, verdict) => {
    const L = colLetter(cn);
    put(rY, cn, FN(`COUNTIF(${L}${R0}:${L}${RN},">="&${cut})`, y));
    put(rZ, cn, FN(`ROUND(${L}${rY}/${nRef}*100,2)`, z));
    if (tgt !== null) {
      put(rT, cn, N_(tgt));
      put(rV, cn, FS(`IF(${L}${rZ}>=${L}${rT},"Y","N")`, verdict ? "Y" : "N"));
    }
  };
  A.forEach((a, i) => { const col = res.cols[i]; band(C0 + i, `${colLetter(C0 + i)}$${FR}*${res.baseT}/100`, col.y, col.z, null, null); });
  band(cPct, "49.5", res.overall.passY, res.overall.passZ, null, null);
  outs.forEach((x, i) => band(cOut + i, String(x.o.stuT), x.y, x.z, x.o.tgt, x.verdict));

  put(rV + 2, 3, S_(`Generated ${new Date().toLocaleString()} — formulas are live, so edited marks recalculate.`));
  ws["!ref"] = "A1:" + colLetter(cOut + Math.max(outs.length, 1)) + (rV + 2);
  ws["!cols"] = [{ wch: 5 }, { wch: 14 }, { wch: 30 },
    ...A.map(() => ({ wch: 12 })), { wch: 9 }, { wch: 9 }, { wch: 7 }, ...outs.map(() => ({ wch: 10 }))];

  const wb = XLSX.utils.book_new();
  XLSX.utils.book_append_sheet(wb, ws, "CAM");
  const buf = XLSX.write(wb, { bookType: "xlsx", type: "array" });
  saveFile(fileStem(c) + "-CAM.xlsx", new Blob([buf],
    { type: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet" }));
}

/* ---------------- import ---------------- */
function pickFile(accept, cb) {
  const inp = document.createElement("input");
  inp.type = "file"; inp.accept = accept;
  inp.onchange = () => { const f = inp.files[0]; if (!f) return; const fr = new FileReader(); fr.onload = () => cb(fr.result, f.name); fr.readAsText(f); };
  inp.click();
}

function importRows(c, rows, hasHeader) {
  const A = c.assessments;
  let head = null, start = 0;
  if (hasHeader) { head = rows[0].map(h => String(h).trim().toLowerCase()); start = 1; }
  let iM = 0, iN = 1, map = A.map((a, j) => 2 + j);
  if (head) {
    const find = re => head.findIndex(h => re.test(h));
    const m = find(/matric|matrik|no\.?\s*matrik|student\s*id/), n = find(/name|nama/);
    if (m >= 0) iM = m; if (n >= 0) iN = n;
    map = A.map((a, j) => {
      const exact = head.findIndex(h => h === a.name.toLowerCase());
      if (exact >= 0) return exact;
      const loose = head.findIndex(h => h.includes(a.name.toLowerCase().split(" ")[0]));
      if (loose >= 0) return loose;
      return head.map((_, k) => k).filter(k => ![iM, iN].includes(k))[j];
    });
  }
  let added = 0, updated = 0;
  rows.slice(start).forEach(r => {
    const matric = String(r[iM] ?? "").trim();
    const name = String(r[iN] ?? "").trim();
    if (!matric && !name) return;
    let s = c.students.find(x => matric && (x.matric || "").trim() === matric);
    if (s) updated++; else { s = { id: uid("s"), matric, name, marks: {}, excluded: false }; c.students.push(s); added++; }
    if (name) s.name = name;
    A.forEach((a, j) => {
      const k = map[j]; if (k == null) return;
      const raw = String(r[k] ?? "").trim(); if (raw === "") return;
      const v = Number(raw.replace(/[^0-9.\-]/g, ""));
      if (isFinite(v)) s.marks[a.id] = v;
    });
  });
  markDirty(); flush(); render();
  toast(`${added} row${added === 1 ? "" : "s"} added, ${updated} updated`);
}

/* ---------------- grid keyboard + paste ---------------- */
const cellAt = (si, aj) => $(`#mBody .cellin[data-si="${si}"][data-aj="${aj}"]`);

function gridKey(e) {
  const el = e.target;
  if (!el.classList.contains("cellin") || !el.dataset.si) return;
  const si = +el.dataset.si, aj = +el.dataset.aj;
  let t = null;
  if (e.key === "Enter") t = cellAt(si + (e.shiftKey ? -1 : 1), aj);
  else if (e.key === "ArrowDown") t = cellAt(si + 1, aj);
  else if (e.key === "ArrowUp") t = cellAt(si - 1, aj);
  else return;
  e.preventDefault();
  if (t) { t.focus(); t.select(); }
}

function gridPaste(e) {
  const el = e.target;
  if (!el.classList.contains("cellin") || !el.dataset.si) return;
  const text = (e.clipboardData || window.clipboardData).getData("text");
  if (!text || !/[\t\n]/.test(text)) return;
  e.preventDefault();
  const c = course(), A = c.assessments;
  const si0 = +el.dataset.si, aj0 = +el.dataset.aj;
  const lines = text.replace(/\r\n?/g, "\n").replace(/\n$/, "").split("\n");
  lines.forEach((line, ri) => {
    const cells = line.split("\t");
    let s = c.students[si0 + ri];
    if (!s) { s = { id: uid("s"), matric: "", name: "", marks: {}, excluded: false }; c.students.push(s); }
    cells.forEach((raw, ci) => {
      const a = A[aj0 + ci]; if (!a) return;
      const v = String(raw).trim();
      s.marks[a.id] = v === "" ? null : (isFinite(Number(v)) ? Number(v) : v);
    });
  });
  markDirty(); flush(); render();
  toast(`Pasted ${lines.length} row${lines.length === 1 ? "" : "s"}`);
}

/* ---------------- delegated handlers ---------------- */
function bindOnce() {
  $("#tabs").addEventListener("click", e => {
    const b = e.target.closest(".tab"); if (b) setView(b.dataset.view);
  });
  $("#coursePick").addEventListener("change", e => {
    S.activeId = e.target.value;
    try { localStorage.setItem("cas.active", S.activeId); } catch (err) {}
    render();
  });
  $("#newCourse").addEventListener("click", newCourse);
  $("#resetTop").addEventListener("click", () => {
    const c = course();
    if (!c) { toast("There is no course open to reset."); return; }
    openReset(c);
  });
  $("#themeBtn").addEventListener("click", () => {
    const cur = document.documentElement.getAttribute("data-theme");
    const next = cur === "dark" ? "light" : cur === "light" ? "" : "dark";
    if (next) document.documentElement.setAttribute("data-theme", next);
    else document.documentElement.removeAttribute("data-theme");
    try { localStorage.setItem("cas.theme", next); } catch (e) {}
  });

  const app = $("#app");
  app.addEventListener("keydown", gridKey);
  app.addEventListener("keydown", e => {
    const card = e.target.closest?.("[data-open]");
    if (card && (e.key === "Enter" || e.key === " ")) { e.preventDefault(); card.click(); }
  });
  app.addEventListener("paste", gridPaste);

  app.addEventListener("input", e => {
    const el = e.target, d = el.dataset;
    const c = course(); if (!c) return;
    if (d.fld !== undefined) {
      c[d.fld] = (el.type === "number") ? (el.value === "" ? "" : Number(el.value)) : el.value;
      markDirty(false);
      if (["courseCode", "courseName", "group"].includes(d.fld)) renderChrome();
      return;
    }
    if (d.cas !== undefined) { c.cas[d.cas] = el.value; markDirty(false); return; }
    if (d.casmap !== undefined) {
      c.cas[d.casmap] = c.cas[d.casmap] || {};
      c.cas[d.casmap][d.oid] = el.value; markDirty(false); return;
    }
    const aHost = el.closest(".acard, tr[data-aid]");
    if (aHost && (d.aname !== undefined || d.afull !== undefined)) {
      const a = c.assessments.find(x => x.id === aHost.dataset.aid); if (!a) return;
      if (d.aname !== undefined) a.name = el.value;
      if (d.afull !== undefined) a.fullMark = el.value === "" ? 0 : Number(el.value);
      markDirty(false); return;
    }
    const oTr = el.closest("tr[data-oid]");
    if (oTr) {
      const list = oTr.dataset.kind === "clos" ? c.clos : c.eacs;
      const o = list.find(x => x.id === oTr.dataset.oid); if (!o) return;
      if (d.ocode !== undefined) o.code = el.value;
      if (d.odesc !== undefined) o.desc = el.value;
      if (d.otarget !== undefined) o.target = el.value === "" ? "" : Number(el.value);
      markDirty(false); return;
    }
    const gTr = el.closest("tr[data-gi]");
    if (gTr) {
      const g = c.gradeScale[+gTr.dataset.gi]; if (!g) return;
      if (d.gname !== undefined) g.grade = el.value;
      if (d.gmin !== undefined) g.min = Number(el.value);
      markDirty(false); return;
    }
    const sTr = el.closest("tr[data-sid]");
    if (sTr) {
      const s = c.students.find(x => x.id === sTr.dataset.sid); if (!s) return;
      if (d.matric !== undefined) { s.matric = el.value; markDirty(false); return; }
      if (d.name !== undefined) { s.name = el.value; markDirty(false); return; }
      if (d.aid !== undefined) {
        const a = c.assessments.find(x => x.id === d.aid);
        const v = el.value.trim();
        s.marks[d.aid] = v === "" ? null : Number(v);
        const num = Number(v);
        el.classList.toggle("bad", v !== "" && (!isFinite(num) || num < 0 || num > Number(a.fullMark) + 1e-9));
        markDirty(false); softRefresh(); return;
      }
    }
  });

  app.addEventListener("change", e => {
    const c = course(); if (!c) return;
    const d = e.target.dataset;
    if (d.map !== undefined) {
      const a = c.assessments.find(x => x.id === e.target.closest("tr[data-aid]").dataset.aid); if (!a) return;
      const set = new Set(a[d.map] || []);
      if (e.target.checked) set.add(d.oid); else set.delete(d.oid);
      a[d.map] = [...set];
      markDirty(); render(); return;
    }
    if (d.adeliv !== undefined) {
      const a = c.assessments.find(x => x.id === e.target.closest(".acard, tr[data-aid]").dataset.aid);
      if (a) { a.delivery = e.target.value; markDirty(); render(); }
      return;
    }
    if (d.sinc !== undefined) {
      const s = c.students.find(x => x.id === e.target.closest("tr[data-sid]").dataset.sid);
      if (s) { s.excluded = !e.target.checked; markDirty(); render(); }
      return;
    }
    if (d.afull !== undefined || d.gmin !== undefined || d.otarget !== undefined ||
        d.fld === "studentThreshold" || d.fld === "defaultTarget" || d.fld === "curriculum") {
      markDirty(); render();
    }
  });

  app.addEventListener("click", e => {
    const del = e.target.closest("[data-cdel]");
    if (del) {
      e.stopPropagation();
      const victim = S.courses.find(x => x.id === del.dataset.cdel); if (!victim) return;
      const label = [victim.courseCode, victim.courseName].filter(x => (x || "").trim()).join(" · ") || "this untitled course";
      confirmDo(`Delete ${label}?`, "Its roster, marks and CAS narrative go with it.", async () => {
        await Store.remove(victim.id).catch(() => {});
        S.courses = S.courses.filter(x => x.id !== victim.id);
        if (S.activeId === victim.id) S.activeId = S.courses[0] ? S.courses[0].id : null;
        render();
      });
      return;
    }
    const card = e.target.closest("[data-open]");
    if (card) {
      S.activeId = card.dataset.open; S.view = "setup";
      try { localStorage.setItem("cas.active", S.activeId); } catch (err) {}
      render(); return;
    }
    const b = e.target.closest("button"); if (!b) return;
    const c = course(); const id = b.id, d = b.dataset;

    if (id === "mkBlank") { newCourse(); return; }
    if (id === "mkDemo") { const n = templateCourse(); S.courses.push(n); S.activeId = n.id; S.view = "analysis"; Store.save(n).catch(() => {}); render(); return; }
    if (d.go) { setView(d.go); return; }
    if (!c) return;

    if (d.doc) { S.doc = d.doc; render(); return; }
    if (d.chip !== undefined) {
      const a = c.assessments.find(x => x.id === b.closest(".acard").dataset.aid); if (!a) return;
      const set = new Set(a[d.chip] || []);
      if (set.has(d.oid)) set.delete(d.oid); else set.add(d.oid);
      a[d.chip] = [...set];
      if (d.chip === "eacs") {
        const used = new Set(); c.assessments.forEach(x => (x.eacs || []).forEach(k => used.add(k)));
        c.eacs.forEach(o => { o.selected = used.has(o.id); });
      }
      markDirty(); render(); return;
    }
    if (id === "resetBtn" || id === "resetBtn2") { openReset(c); return; }
    if (id === "addA") { c.assessments.push({ id: uid("a"), name: "New assessment", fullMark: 10, delivery: "Lecture", clos: [], eacs: [] }); markDirty(); render(); return; }
    if (id === "addCLO") { c.clos.push({ id: uid("o"), code: "CO" + (c.clos.length + 1), desc: "", taxonomy: "", target: c.defaultTarget, studentThreshold: null }); markDirty(); render(); return; }
    if (id === "addG") { c.gradeScale.push({ grade: "New", min: 0 }); markDirty(); render(); return; }
    if (id === "addS") { c.students.push({ id: uid("s"), matric: "", name: "", marks: {}, excluded: false }); markDirty(); render(); return; }
    if (id === "add10") { for (let i = 0; i < 10; i++) c.students.push({ id: uid("s"), matric: "", name: "", marks: {}, excluded: false }); markDirty(); render(); return; }
    if (id === "sortName") { c.students.sort((x, y) => (x.name || "").localeCompare(y.name || "")); markDirty(); render(); return; }
    if (id === "sortMatric") { c.students.sort((x, y) => (x.matric || "").localeCompare(y.matric || "", undefined, { numeric: true })); markDirty(); render(); return; }

    if (d.adel !== undefined) {
      const a = c.assessments.find(x => x.id === b.closest(".acard, tr[data-aid]").dataset.aid);
      confirmDo(`Remove “${a.name}”?`, "Its marks are deleted from every student row.", () => {
        c.assessments = c.assessments.filter(x => x.id !== a.id);
        c.students.forEach(s => { delete s.marks[a.id]; });
        markDirty(); render();
      }); return;
    }
    if (d.odel !== undefined) {
      const tr = b.closest("tr[data-oid]"), key = tr.dataset.kind, oid = tr.dataset.oid;
      c[key] = c[key].filter(o => o.id !== oid);
      c.assessments.forEach(a => { a[key] = (a[key] || []).filter(x => x !== oid); });
      markDirty(); render(); return;
    }
    if (d.gdel !== undefined) { c.gradeScale.splice(+b.closest("tr[data-gi]").dataset.gi, 1); markDirty(); render(); return; }
    if (d.sdel !== undefined) {
      const sid = b.closest("tr[data-sid]").dataset.sid;
      c.students = c.students.filter(s => s.id !== sid); markDirty(); render(); return;
    }

    const res = calc(c);
    if (id === "printBtn") { window.print(); return; }
    if (id === "dlDoc") {
      saveFile(fileStem(c) + "-" + (S.doc === "cam" ? "CAM" : "CAS") + ".html",
        standaloneDoc(c, res, S.doc), "text/html"); return;
    }
    if (id === "exMarks") { exportMarksCSV(c, res); return; }
    if (id === "exAnalysis") { exportAnalysisCSV(c, res); return; }
    if (id === "exXlsx") { exportXLSX(c, res); return; }
    if (id === "exJson") { saveFile(fileStem(c) + "-backup.json", JSON.stringify(c, null, 2), "application/json"); return; }

    if (id === "impCsv" || id === "impCsv2") {
      pickFile(".csv,text/csv", txt => {
        const rows = parseCSV(txt);
        if (!rows.length) { toast("That file has no rows."); return; }
        dialog("Import " + rows.length + " lines",
          `<p class="hint">Columns are matched to assessment names where possible, otherwise left to right.</p>
           <label style="font-size:13px"><input type="checkbox" id="hasHead" checked> The first line is a header row</label>`,
          [{ label: "Import", primary: true, onClick: dd => { importRows(c, rows, $("#hasHead", dd).checked); } },
           { label: "Cancel" }]);
      }); return;
    }
    if (id === "impRoster") {
      dialog("Paste a roster", `<p class="hint">One student per line: matric number, then name, separated by a tab or a comma.</p>
        <textarea rows="8" id="rosterTxt" spellcheck="false" placeholder="190234&#9;Aisyah binti Rahman"></textarea>`,
        [{ label: "Add students", primary: true, onClick: dd => {
            const lines = $("#rosterTxt", dd).value.replace(/\r\n?/g, "\n").split("\n").filter(l => l.trim());
            lines.forEach(l => {
              const p = l.split(/\t|,/).map(x => x.trim());
              c.students.push({ id: uid("s"), matric: p[0] || "", name: p.slice(1).join(", ") || "", marks: {}, excluded: false });
            });
            markDirty(); flush(); render(); toast(lines.length + " students added");
          } }, { label: "Cancel" }]); return;
    }
    if (id === "impJson") {
      pickFile(".json,application/json", txt => {
        let obj; try { obj = JSON.parse(txt); } catch (err) { toast("That is not a valid backup file."); return; }
        if (!obj || !Array.isArray(obj.assessments)) { toast("That backup has no course in it."); return; }
        obj = migrate(obj);
        obj.id = uid("c"); obj.courseName = (obj.courseName || "Restored") + " (restored)";
        S.courses.push(obj); S.activeId = obj.id; Store.save(obj).catch(() => {}); render();
        toast("Backup restored as a new course");
      }); return;
    }
    if (id === "dupEmpty" || id === "dupFull") {
      const n = JSON.parse(JSON.stringify(c));
      n.id = uid("c"); n.semester = ""; n.updated = Date.now();
      n.cas = { prevReview: "", teachingPlan: c.cas.teachingPlan || "", eacComments: {}, cloComments: {}, reflection: "", recommendation: "" };
      if (id === "dupEmpty") n.students = []; else n.students.forEach(s => { s.id = uid("s"); });
      S.courses.push(n); S.activeId = n.id; S.view = "setup"; Store.save(n).catch(() => {}); render();
      toast("Duplicated — set the new semester and its minimums");
      return;
    }
    if (id === "delCourse") {
      confirmDo("Delete this course?", "The roster, marks, CAS narrative and analysis go with it. Download a backup first if you need one.", async () => {
        await Store.remove(c.id).catch(() => {});
        S.courses = S.courses.filter(x => x.id !== c.id);
        S.activeId = S.courses[0] ? S.courses[0].id : null;
        S.view = "home"; render();
      }); return;
    }
  });
}

/* ---------------- startup ---------------- */
(async function start() {
  $("#crestImg").src = CREST;
  try {
    const t = localStorage.getItem("cas.theme");
    if (t) document.documentElement.setAttribute("data-theme", t);
    const v = localStorage.getItem("cas.view"); if (v) S.view = v;
  } catch (e) {}

  bindOnce();
  setSaveState("Loading…", "busy");
  render();

  await Store.init();
  let list = [];
  try { list = await Store.list(); } catch (e) { list = []; }
  S.courses = list.filter(c => c && c.id && Array.isArray(c.assessments)).map(migrate);

  let want = null;
  try { want = localStorage.getItem("cas.active"); } catch (e) {}
  S.activeId = (want && S.courses.some(c => c.id === want)) ? want
    : (S.courses.slice().sort((a, b) => (b.updated || 0) - (a.updated || 0))[0]?.id || null);

  setSaveState(Store.mode === "db" ? "Saved" : "Saved in this browser", "");
  render();
})();

</script>
</body>
</html>
