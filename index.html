import { useState, useRef, useEffect } from "react";

// ── Inline SVG icons (no external deps) ──────────────────────────────────────

// UI icons — Lucide-style inline SVG strokes
const UI_ICONS = {
  folder:     (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"/></svg>,
  "code-2":   (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>,
  search:     (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><circle cx="11" cy="11" r="7"/><line x1="21" y1="21" x2="16.65" y2="16.65"/></svg>,
  settings:   (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1-2.83 2.83l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-4 0v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83-2.83l.06-.06A1.65 1.65 0 0 0 4.68 15a1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1 0-4h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 2.83-2.83l.06.06A1.65 1.65 0 0 0 9 4.68a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 4 0v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 2.83l-.06.06A1.65 1.65 0 0 0 19.4 9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 0 4h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>,
  play:       (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill={c}><polygon points="5,3 19,12 5,21"/></svg>,
  square:     (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill={c}><rect x="4" y="4" width="16" height="16" rx="2"/></svg>,
  "rotate-ccw":(s,c="currentColor")=> <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M3 12a9 9 0 1 0 9-9 9.75 9.75 0 0 0-6.74 2.74L3 8"/><path d="M3 3v5h5"/></svg>,
  rocket:     (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><path d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"/><path d="m12 15-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"/><path d="M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0"/><path d="M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5"/></svg>,
  "chevron-left":(s,c="currentColor")=><svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><polyline points="15 18 9 12 15 6"/></svg>,
  pencil:     (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.8" strokeLinecap="round" strokeLinejoin="round"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>,
  heart:      (s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill={c}><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"/></svg>,
  "git-branch":(s,c="currentColor")=> <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><line x1="6" y1="3" x2="6" y2="15"/><circle cx="18" cy="6" r="3"/><circle cx="6" cy="18" r="3"/><path d="M18 9a9 9 0 0 1-9 9"/></svg>,
  "gamepad-2":(s,c="currentColor") => <svg width={s} height={s} viewBox="0 0 24 24" fill="none" stroke={c} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><line x1="6" y1="11" x2="10" y2="11"/><line x1="8" y1="9" x2="8" y2="13"/><line x1="15" y1="12" x2="15.01" y2="12"/><line x1="18" y1="10" x2="18.01" y2="10"/><path d="M17.32 5H6.68a4 4 0 0 0-3.978 3.59l-.7 7A4 4 0 0 0 6 20h12a4 4 0 0 0 3.998-4.41l-.7-7A4 4 0 0 0 17.32 5z"/></svg>,
};

function Icon({ name, size = 16, color = "currentColor" }) {
  const fn = UI_ICONS[name];
  return fn ? fn(size, color) : null;
}


// ── File type icons & colors ──────────────────────────────────────────────────
const FILE_ICONS = {
  html:     { color: "#e34c26", lang: "HTML"       },
  css:      { color: "#264de4", lang: "CSS"        },
  js:       { color: "#f7df1e", lang: "JavaScript" },
  p5:       { color: "#ed225d", lang: "p5.js"      },
  ts:       { color: "#3178c6", lang: "TypeScript" },
  lua:      { color: "#7ba9d4", lang: "Lua"        },
  python:   { color: "#ffd43b", lang: "Python"     },
  markdown: { color: "#9090cc", lang: "Markdown"   },
  csharp:   { color: "#9b59b6", lang: "C#"         },
  cpp:      { color: "#00599c", lang: "C++"        },
  swift:    { color: "#f05138", lang: "Swift"      },
  luau:     { color: "#00a2ff", lang: "Luau"         },
};

// ── Default starter code ─────────────────────────────────────────────────────
const DEFAULTS = {
  html: `<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Coin Collector</title>
</head>
<body>
  <canvas id="c"></canvas>
  <div id="hud">
    <span id="score">0</span>
    <span id="label"> pts</span>
  </div>
</body>
</html>`,

  css: `* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: #0d0d1a;
  width: 400px;
  height: 400px;
  overflow: hidden;
  position: relative;
}

canvas {
  display: block;
  width: 400px;
  height: 400px;
}

#hud {
  position: absolute;
  top: 12px;
  right: 14px;
  pointer-events: none;
}

#score {
  color: #569cd6;
  font: bold 20px "Consolas", monospace;
  text-shadow: 0 0 10px #569cd688;
}

#label {
  color: #858585;
  font: 11px monospace;
}`,

  js: `// Coin Collector — Arrow/WASD to move
const canvas=document.getElementById('c'),ctx=canvas.getContext('2d');
let score=0,px=200,py=200;
const coins=Array.from({length:8},()=>({x:Math.random()*360+20,y:Math.random()*360+20}));
const keys={};
document.addEventListener('keydown',e=>keys[e.key]=true);
document.addEventListener('keyup',e=>keys[e.key]=false);
function loop(){
  if(keys['ArrowLeft']||keys['a'])px-=3;
  if(keys['ArrowRight']||keys['d'])px+=3;
  if(keys['ArrowUp']||keys['w'])py-=3;
  if(keys['ArrowDown']||keys['s'])py+=3;
  px=Math.max(10,Math.min(390,px));py=Math.max(10,Math.min(390,py));
  ctx.fillStyle='#0d0d1a';ctx.fillRect(0,0,400,400);
  coins.forEach((c,i)=>{
    if(Math.hypot(px-c.x,py-c.y)<16){score++;document.getElementById('score').textContent=score;coins[i]={x:Math.random()*360+20,y:Math.random()*360+20};}
    ctx.fillStyle='#ffd700';ctx.beginPath();ctx.arc(c.x,c.y,8,0,Math.PI*2);ctx.fill();
  });
  ctx.fillStyle='#a78bfa';ctx.beginPath();ctx.arc(px,py,12,0,Math.PI*2);ctx.fill();
  requestAnimationFrame(loop);
}
loop();`,


  p5: `function setup(){createCanvas(400,400);}
function draw(){
  background(13,13,26);
  fill(167,139,250);noStroke();
  ellipse(mouseX,mouseY,30,30);
  fill(56,189,248);textSize(14);textAlign(CENTER);
  text('Move your mouse!',200,380);
}`,


  ts: `const canvas=document.getElementById('gameCanvas') as HTMLCanvasElement;
const ctx=canvas.getContext('2d')!;
ctx.fillStyle='#0d0d1a';ctx.fillRect(0,0,400,400);
ctx.fillStyle='#a78bfa';ctx.font='bold 28px monospace';ctx.textAlign='center';
ctx.fillText('TypeScript',200,190);
ctx.fillStyle='#3178c6';ctx.font='14px monospace';
ctx.fillText('Edit to get started',200,225);`,


  lua: `-- Lua starter
local x, y = 200, 200
print("Hello from Lua!")
for i = 1, 5 do
  print("Line " .. i)
end`,


  python: `# Python starter
print("Hello from Python!")
for i in range(1, 6):
    print(f"Line {i}")`,


  markdown: `# Hello Yumii!

Welcome to the **Markdown** editor.

- Write *formatted* text
- Add `code` snippets
- Create lists

> Start typing to see a live preview!`,


  csharp: `using System;
class Program {
  static void Main() {
    Console.WriteLine("Hello from C#!");
    for(int i=1;i<=5;i++)
      Console.WriteLine($"Line {i}");
  }
}`,


  cpp: `// C++ — compiled via Emscripten / WASM
#include <cstdio>
#include <cstdlib>
#include <cmath>
#include <ctime>
#include <vector>

struct Vec2 { float x, y; };

struct Particle {
    Vec2 pos, vel;
    float life, hue;
};

const int W = 40, H = 20;
char grid[H][W + 1];

void clear_grid() {
    for (int y = 0; y < H; y++) {
        for (int x = 0; x < W; x++) grid[y][x] = ' ';
        grid[y][W] = '\\0';
    }
}

void set(int x, int y, char c) {
    if (x >= 0 && x < W && y >= 0 && y < H) grid[y][x] = c;
}

int main() {
    srand((unsigned)time(nullptr));
    std::vector<Particle> ps;
    float t = 0.f;

    printf("C++ Particle Fountain — ASCII art demo\\n\\n");

    for (int frame = 0; frame < 60; frame++) {
        // Spawn
        for (int i = 0; i < 3; i++) {
            float angle = (float)rand() / RAND_MAX * 3.14159f;
            float speed = 0.4f + (float)rand() / RAND_MAX * 0.8f;
            ps.push_back({{W / 2.f, H - 2.f},
                          {cosf(angle) * speed, -sinf(angle) * speed - 0.3f},
                          1.f, (float)rand() / RAND_MAX * 360.f});
        }

        // Update + draw
        clear_grid();
        // Floor
        for (int x = 0; x < W; x++) set(x, H - 1, '-');
        // Nozzle
        set(W / 2, H - 2, '^');

        for (auto& p : ps) {
            p.vel.y += 0.08f;   // gravity
            p.pos.x += p.vel.x;
            p.pos.y += p.vel.y;
            p.life  -= 0.018f;
            char c = p.life > 0.7f ? '*' : p.life > 0.4f ? '+' : '.';
            set((int)p.pos.x, (int)p.pos.y, c);
        }
        // Remove dead particles
        ps.erase(std::remove_if(ps.begin(), ps.end(),
            [](const Particle& p){ return p.life <= 0; }), ps.end());

        // Print frame
        printf("Frame %2d  particles: %zu\\n", frame + 1, ps.size());
        for (int y = 0; y < H; y++) printf("|%s|\\n", grid[y]);
        printf("\\n");
        t += 0.1f;
    }
    return 0;
}`
,

  swift: `// Swift — playground-style demo
import Foundation

// ── Data structures ─────────────────────────────────
struct Vec2 {
    var x: Double
    var y: Double

    func distance(to other: Vec2) -> Double {
        let dx = x - other.x
        let dy = y - other.y
        return (dx * dx + dy * dy).squareRoot()
    }

    static func + (a: Vec2, b: Vec2) -> Vec2 { Vec2(x: a.x + b.x, y: a.y + b.y) }
    static func * (v: Vec2, s: Double) -> Vec2 { Vec2(x: v.x * s, y: v.y * s) }
}

// ── Particle system ─────────────────────────────────
struct Particle {
    var pos: Vec2
    var vel: Vec2
    var life: Double
    var symbol: Character

    mutating func update(dt: Double) {
        vel.y += 0.15 * dt   // gravity
        pos = pos + vel * dt
        life -= dt * 0.4
    }

    var isAlive: Bool { life > 0 }
}

class ParticleSystem {
    var particles: [Particle] = []
    private let symbols: [Character] = ["*", "+", "·", "°", "✦"]

    func spawn(at pos: Vec2, count: Int) {
        for _ in 0..<count {
            let angle = Double.random(in: 0...(.pi * 2))
            let speed = Double.random(in: 2...6)
            particles.append(Particle(
                pos: pos,
                vel: Vec2(x: cos(angle) * speed, y: sin(angle) * speed - 4),
                life: Double.random(in: 0.6...1.0),
                symbol: symbols.randomElement()!
            ))
        }
    }

    func update(dt: Double) {
        for i in particles.indices { particles[i].update(dt: dt) }
        particles.removeAll { !$0.isAlive }
    }
}

// ── ASCII canvas ────────────────────────────────────
let W = 50, H = 18
func render(_ ps: ParticleSystem, frame: Int) -> String {
    var grid = Array(repeating: Array(repeating: " ", count: W), count: H)
    // Floor
    for x in 0..<W { grid[H-1][x] = "─" }
    // Particles
    for p in ps.particles {
        let x = Int(p.pos.x), y = Int(p.pos.y)
        if x >= 0 && x < W && y >= 0 && y < H {
            grid[y][x] = String(p.symbol)
        }
    }
    let lines = grid.map { "│" + $0.joined() + "│" }
    return "Frame \\(frame) — \\(ps.particles.count) particles\\n" + lines.joined(separator: "\\n")
}

// ── Run simulation ─────────────────────────────────
let sim = ParticleSystem()
let spawnPoint = Vec2(x: Double(W) / 2, y: Double(H) - 2)
var frame = 0

for _ in 0..<30 {
    if frame % 3 == 0 { sim.spawn(at: spawnPoint, count: 5) }
    sim.update(dt: 1.0)
    print(render(sim, frame: frame))
    frame += 1
}

print("\\n✅ Swift simulation complete — \\(frame) frames rendered.")`,

  luau: `-- Roblox Luau starter
print('Hello from Luau!')

local x = 10
local y = 20
print('Sum: ' .. tostring(x + y))
`,
};

// ── Language modes ────────────────────────────────────────────────────────────
const MODES = {
  web: {
    id:"web", label:"HTML / CSS / JS", color:"#e8724a",
    desc:"3 files compiled to one page",
    tabs:["html","css","js"],
    tabInfo:{
      html:{ label:"index.html", fileKey:"html" },
      css: { label:"style.css",  fileKey:"css"  },
      js:  { label:"script.js",  fileKey:"js"   },
    }
  },
  p5:      { id:"p5",      label:"p5.js",      color:"#ed225d", desc:"Creative coding library", tabs:["p5"],       tabInfo:{ p5:      { label:"sketch.js",  fileKey:"p5"       } } },
  ts:      { id:"ts",      label:"TypeScript", color:"#3178c6", desc:"Types + Babel transpile",  tabs:["ts"],       tabInfo:{ ts:      { label:"game.ts",    fileKey:"ts"       } } },
  lua:     { id:"lua",     label:"Lua",        color:"#7ba9d4", desc:"Fengari WASM runtime",     tabs:["lua"],      tabInfo:{ lua:     { label:"game.lua",   fileKey:"lua"      } } },
  python:  { id:"python",  label:"Python",     color:"#ffd43b", desc:"Pyodide WASM (~5s load)",  tabs:["python"],   tabInfo:{ python:  { label:"game.py",    fileKey:"python"   } } },
  markdown:{ id:"markdown",label:"Markdown",   color:"#9090cc", desc:"Rendered preview",         tabs:["markdown"], tabInfo:{ markdown:{ label:"readme.md",  fileKey:"markdown" } } },
  csharp:  { id:"csharp",  label:"C#",         color:"#9b59b6", desc:"Roslyn WASM runtime",      tabs:["csharp"],   tabInfo:{ csharp:  { label:"Program.cs", fileKey:"csharp"   } } },
  cpp:     { id:"cpp",     label:"C++",        color:"#00599c", desc:"Emscripten WASM compile",  tabs:["cpp"],      tabInfo:{ cpp:     { label:"main.cpp",   fileKey:"cpp"      } } },
  swift:   { id:"swift",   label:"Swift",      color:"#f05138", desc:"SwiftyWASM preview",        tabs:["swift"],    tabInfo:{ swift:   { label:"main.swift", fileKey:"swift"    } } },
  luau:    { id:"luau",    label:"Luau",       color:"#00a2ff", desc:"Roblox Luau runtime",        tabs:["luau"],     tabInfo:{ luau:    { label:"script.luau",fileKey:"luau"     } } },
};

const GENRES = ["All","Arcade","Action","Puzzle","Sports","Sandbox"];

// ── Build preview HTML ────────────────────────────────────────────────────────
function buildPreview(modeId, files) {
  const bg = "#0d0d1a", fg = "#ccc", font = "13px Consolas,monospace";

  const consoleHook = [
    "(function(){var _m=['log','warn','error','info'];_m.forEach(function(m){var o=console[m].bind(console);console[m]=function(){var a=Array.prototype.slice.call(arguments).map(function(x){try{return typeof x==='object'?JSON.stringify(x):String(x);}catch(e){return String(x);}});o.apply(console,arguments);window.parent.postMessage({__yumiiConsole:true,level:m,text:a.join(' ')},'*');};});})();"
  ].join("");

  const gamepadHook = [
    "(function(){var B=[{b:0,k:'z',c:'KeyZ'},{b:1,k:'x',c:'KeyX'},{b:2,k:'c',c:'KeyC'},{b:3,k:'v',c:'KeyV'},{b:4,k:'q',c:'KeyQ'},{b:5,k:'e',c:'KeyE'},{b:8,k:'Escape',c:'Escape'},{b:9,k:'Enter',c:'Enter'},{b:12,k:'ArrowUp',c:'ArrowUp'},{b:13,k:'ArrowDown',c:'ArrowDown'},{b:14,k:'ArrowLeft',c:'ArrowLeft'},{b:15,k:'ArrowRight',c:'ArrowRight'}];",
    "var A=[{a:0,n:{k:'ArrowLeft',c:'ArrowLeft'},p:{k:'ArrowRight',c:'ArrowRight'}},{a:1,n:{k:'ArrowUp',c:'ArrowUp'},p:{k:'ArrowDown',c:'ArrowDown'}},{a:2,n:{k:'a',c:'KeyA'},p:{k:'d',c:'KeyD'}},{a:3,n:{k:'w',c:'KeyW'},p:{k:'s',c:'KeyS'}}];",
    "var DZ=0.25,held={};function fire(t,k,c){var e=new KeyboardEvent(t,{key:k,code:c,bubbles:true,cancelable:true});document.dispatchEvent(e);window.dispatchEvent(e);}",
    "function press(id){if(!held[id]){held[id]=true;var p=id.split('|');fire('keydown',p[0],p[1]);}}function rel(id){if(held[id]){held[id]=false;var p=id.split('|');fire('keyup',p[0],p[1]);}}",
    "function poll(){var pads=navigator.getGamepads?navigator.getGamepads():[];for(var i=0;i<pads.length;i++){var gp=pads[i];if(!gp)continue;B.forEach(function(m){var id=m.k+'|'+m.c;if(gp.buttons[m.b]&&gp.buttons[m.b].pressed)press(id);else rel(id);});A.forEach(function(m){var v=gp.axes[m.a]||0;var ni=m.n.k+'|'+m.n.c,pi=m.p.k+'|'+m.p.c;if(v<-DZ){press(ni);rel(pi);}else if(v>DZ){press(pi);rel(ni);}else{rel(ni);rel(pi);}});}requestAnimationFrame(poll);}requestAnimationFrame(poll);",
    "window.addEventListener('gamepadconnected',function(e){window.parent.postMessage({__yumiiConsole:true,level:'info',text:'🎮 Controller connected: '+e.gamepad.id},'*');});",
    "window.addEventListener('gamepaddisconnected',function(){window.parent.postMessage({__yumiiConsole:true,level:'info',text:'Controller disconnected'},'*');});})();"
  ].join("");

  const errHook = [
    "window.onerror=function(msg,_src,line,col){",
    "window.parent.postMessage({__yumiiConsole:true,level:'error',text:String(msg)+(line?' (line '+line+')':'')},'*');",
    "var cv=document.getElementById('gameCanvas');if(!cv)return;",
    "var x=cv.getContext('2d');x.fillStyle='#0d0d1a';x.fillRect(0,0,400,400);",
    "x.fillStyle='#f48771';x.font='bold 12px Consolas,monospace';x.textAlign='left';x.fillText('RuntimeError',12,166);",
    "x.fillStyle='#ce9178';x.font='11px Consolas,monospace';",
    "var words=String(msg).split(' ');var row='';var y=186;",
    "words.forEach(function(w){if((row+w).length>46){x.fillText(row.trim(),12,y);y+=16;row='';}row+=w+' ';});",
    "if(row.trim())x.fillText(row.trim(),12,y);if(line)x.fillText('Line '+line+(col?', Col '+col:''),12,y+18);};",
  ].join("");

  const hooks = consoleHook + gamepadHook + errHook;

  if (modeId === "web") {
    let html = files.html || DEFAULTS.html;
    const css = files.css || DEFAULTS.css;
    const js  = files.js  || DEFAULTS.js;
    const cssTag = "<style>\n" + css + "\n</style>";
    const jsTag  = "<script>\n" + hooks + "\ntry{\n" + js + "\n}catch(e){window.onerror(e.message,'',e.lineNumber,0);}\n<\/script>";
    html = html.includes("</head>") ? html.replace("</head>", cssTag + "\n</head>") : cssTag + "\n" + html;
    html = html.includes("</body>") ? html.replace("</body>", jsTag  + "\n</body>") : html + "\n" + jsTag;
    return html;
  }

  if (modeId === "p5") {
    return [
      "<!DOCTYPE html><html><head>",
      "<style>*{margin:0;padding:0}body{background:#0d0d1a;overflow:hidden;width:400px;height:400px}</style>",
      "<script src='https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.0/p5.min.js'><\/script>",
      "</head><body><script>", hooks,
      "try{" + (files.p5 || DEFAULTS.p5) + "}catch(e){window.onerror(e.message,'',0,0);}",
      "<\/script></body></html>",
    ].join("");
  }

  // For other modes: syntax-highlighted source viewer
  const code = files[modeId] || DEFAULTS[modeId] || "// No code";
  const escaped = code.replace(/&/g,"&amp;").replace(/</g,"&lt;").replace(/>/g,"&gt;");
  const labels = {ts:"TypeScript",lua:"Lua",python:"Python",markdown:"Markdown",csharp:"C#",cpp:"C++",swift:"Swift",luau:"Luau (Roblox)"};
  const label = labels[modeId] || modeId;
  return `<!DOCTYPE html><html><head><style>
    *{margin:0;padding:0;box-sizing:border-box}
    body{background:#1e1e1e;color:#ccc;font:13px/1.6 Consolas,monospace;padding:0;display:flex;flex-direction:column;height:400px;width:400px;overflow:hidden}
    .bar{background:#252526;padding:6px 14px;font-size:11px;color:#569cd6;font-weight:700;letter-spacing:.05em;border-bottom:1px solid #3e3e42;flex-shrink:0}
    .code{overflow:auto;padding:14px;flex:1;white-space:pre;tab-size:2}
  </style></head><body>
  <div class="bar">${label}</div>
  <div class="code">${escaped}</div>
  </body></html>`;
}
function Thumb({ game, size }) {
  const h = Math.round(size * 0.62);
  const mode = MODES[game.modeId] || {};
  return (
    <div style={{ width:size, height:h, background:game.bg, borderRadius:14, display:"flex", alignItems:"center", justifyContent:"center", fontSize:size>140?40:24, position:"relative", overflow:"hidden", flexShrink:0 }}>
      <div style={{ position:"absolute", inset:0, background:"radial-gradient(circle at 60% 30%,"+game.accent+"28 0%,transparent 65%)" }}/>
      <span style={{ position:"relative", zIndex:1 }}>{game.emoji}</span>
      <div style={{ position:"absolute", bottom:5, left:6, background:"rgba(0,0,0,.75)", borderRadius:3, padding:"2px 6px", fontSize:8, color:game.accent, fontWeight:700, letterSpacing:".06em", textTransform:"uppercase" }}>{game.genre}</div>
    </div>
  );
}

// ── Syntax highlighter (basic, inline) ───────────────────────────────────────
function tokenize(line, lang) {
  // Returns array of {text, color} spans — minimal but visually useful
  const spans = [];
  let rest = line;

  // Helpers
  const push = (text, color) => { if (text) spans.push({ text, color }); };

  // Comment patterns
  const commentPatterns = {
    js: /^(\s*\/\/.*)/, ts: /^(\s*\/\/.*)/, p5: /^(\s*\/\/.*)/, html: null,
    css: /^(\s*\/\*.*)/, lua: /^(\s*--.*)/, python: /^(\s*#.*)/, markdown: null,
    csharp: /^(\s*\/\/.*)/, cpp: /^(\s*\/\/.*)/,
    swift:  /^(\s*\/\/.*)/, luau: /^(\s*--.*)/,
  };

  const cPat = commentPatterns[lang];
  if (cPat) {
    const m = rest.match(cPat);
    if (m) { push(rest, "#6a9955"); return spans; }
  }

  if (lang === "html") {
    // Tag coloring
    const tagRe = /(<\/?)([a-zA-Z][a-zA-Z0-9]*)([^>]*)(>)/g;
    let last = 0, match;
    while ((match = tagRe.exec(rest)) !== null) {
      push(rest.slice(last, match.index), "#cccccc");
      push(match[1], "#808080");
      push(match[2], "#569cd6");
      // attrs
      const attrs = match[3];
      const attrRe = /(\s+[a-zA-Z-:]+)(="[^"]*")?/g;
      let am;
      while ((am = attrRe.exec(attrs)) !== null) {
        push(am[1], "#9cdcfe");
        if (am[2]) {
          push("=", "#cccccc");
          push(am[2].slice(1), "#ce9178");
        }
      }
      push(match[4], "#808080");
      last = match.index + match[0].length;
    }
    push(rest.slice(last), "#cccccc");
    return spans;
  }

  if (lang === "css") {
    // Property: value
    if (rest.match(/^\s*[\w-]+\s*:/)) {
      const colonIdx = rest.indexOf(":");
      push(rest.slice(0, colonIdx), "#9cdcfe");
      push(":", "#cccccc");
      push(rest.slice(colonIdx + 1), "#ce9178");
      return spans;
    }
    if (rest.match(/^\s*[.#]?[\w-]+\s*\{?/)) { push(rest, "#d7ba7d"); return spans; }
    push(rest, "#cccccc");
    return spans;
  }

  if (lang === "markdown") {
    if (rest.match(/^#{1,3} /)) { push(rest, "#569cd6"); return spans; }
    if (rest.match(/^\|/)) { push(rest, "#4ec9b0"); return spans; }
    if (rest.match(/^[-*] /)) { push(rest, "#d7ba7d"); return spans; }
    if (rest.match(/^>/)) { push(rest, "#6a9955"); return spans; }
    if (rest.match(/^```/)) { push(rest, "#c586c0"); return spans; }
    push(rest, "#cccccc");
    return spans;
  }

  // JS/TS/p5/Lua/Python/C#/C++ — keyword + string + number coloring
  const kwJS   = /\b(const|let|var|function|return|if|else|for|while|new|class|import|export|default|this|typeof|instanceof|true|false|null|undefined|async|await|=\>|break|continue|switch|case)\b/g;
  const kwPy   = /\b(def|import|from|return|if|elif|else|for|while|class|True|False|None|and|or|not|in|is|global|pass|break|continue|async|await|lambda|yield)\b/g;
  const kwLua  = /\b(local|function|return|if|then|else|elseif|end|for|while|do|repeat|until|and|or|not|in|nil|true|false)\b/g;
  const kwCS   = /\b(using|namespace|class|struct|interface|enum|public|private|protected|static|void|int|float|double|bool|string|char|long|var|new|return|if|else|for|foreach|while|do|switch|case|break|continue|null|true|false|this|base|override|virtual|abstract|readonly|const|async|await|try|catch|finally|throw|in|out|ref)\b/g;
  const kwCPP  = /\b(include|define|ifdef|ifndef|endif|using|namespace|class|struct|union|enum|public|private|protected|static|void|int|float|double|bool|char|long|short|unsigned|auto|const|return|if|else|for|while|do|switch|case|break|continue|nullptr|true|false|this|new|delete|virtual|override|template|typename|inline|extern|try|catch|throw)\b/g;
  const kwSwift = /\b(import|class|struct|enum|protocol|extension|func|var|let|const|return|if|else|guard|for|while|repeat|switch|case|break|continue|fallthrough|throw|throws|try|catch|defer|in|is|as|nil|true|false|self|super|init|deinit|get|set|override|final|static|lazy|weak|unowned|mutating|nonmutating|public|private|internal|fileprivate|open|async|await)\b/g;
  const kwLuau = /\b(local|function|return|if|then|else|elseif|end|for|while|do|repeat|until|and|or|not|in|nil|true|false|break|continue|type|export)\b/g;
  const kwPat  = lang === "python" ? kwPy : lang === "lua" ? kwLua : lang === "csharp" ? kwCS : lang === "cpp" ? kwCPP : lang === "swift" ? kwSwift : lang === "luau" ? kwLuau : kwJS;

  const strRe  = /(["'`])(?:(?!\1)[^\\]|\\.)*\1/g;
  const numRe  = /\b(\d+\.?\d*)\b/g;

  // Interleave: strings first, then keywords, then numbers
  let colored = rest;
  const parts = [];

  // We'll do a simpler pass: split by strings, color each segment
  const strSplit = [];
  let lastIdx = 0;
  let sm;
  strRe.lastIndex = 0;
  while ((sm = strRe.exec(rest)) !== null) {
    strSplit.push({ start: lastIdx, end: sm.index, type: "code" });
    strSplit.push({ start: sm.index, end: sm.index + sm[0].length, type: "string" });
    lastIdx = sm.index + sm[0].length;
  }
  strSplit.push({ start: lastIdx, end: rest.length, type: "code" });

  for (const seg of strSplit) {
    const txt = rest.slice(seg.start, seg.end);
    if (!txt) continue;
    if (seg.type === "string") { push(txt, "#ce9178"); continue; }
    // Color keywords
    kwPat.lastIndex = 0;
    let kLast = 0, km;
    while ((km = kwPat.exec(txt)) !== null) {
      // Before keyword
      const before = txt.slice(kLast, km.index);
      // Color numbers in before
      numRe.lastIndex = 0;
      let nLast = 0, nm;
      while ((nm = numRe.exec(before)) !== null) {
        push(before.slice(nLast, nm.index), "#cccccc");
        push(nm[0], "#b5cea8");
        nLast = nm.index + nm[0].length;
      }
      push(before.slice(nLast), "#cccccc");
      push(km[0], "#569cd6");
      kLast = km.index + km[0].length;
    }
    const after = txt.slice(kLast);
    numRe.lastIndex = 0;
    let nLast = 0, nm;
    while ((nm = numRe.exec(after)) !== null) {
      push(after.slice(nLast, nm.index), "#cccccc");
      push(nm[0], "#b5cea8");
      nLast = nm.index + nm[0].length;
    }
    push(after.slice(nLast), "#cccccc");
  }

  return spans;
}

// ── Editor component ──────────────────────────────────────────────────────────
function CodeEditor({ code, onChange, lang, onRun }) {
  const taRef     = useRef(null);
  const hlRef     = useRef(null);
  const scrollRef = useRef(null);
  const [cursor, setCursor] = useState({ line: 1, col: 1 });

  // Sync textarea scroll → highlight layer
  function syncScroll() {
    if (hlRef.current && taRef.current) {
      hlRef.current.scrollTop  = taRef.current.scrollTop;
      hlRef.current.scrollLeft = taRef.current.scrollLeft;
    }
  }

  function onKeyDown(e) {
    if (e.key === "Tab") {
      e.preventDefault();
      const ta = taRef.current, s = ta.selectionStart, en = ta.selectionEnd;
      const next = code.substring(0, s) + "  " + code.substring(en);
      onChange(next);
      setTimeout(() => { ta.selectionStart = ta.selectionEnd = s + 2; }, 0);
    }
    if ((e.ctrlKey || e.metaKey) && e.key === "Enter") { e.preventDefault(); onRun && onRun(); }
  }

  function onSel() {
    const ta = taRef.current;
    if (!ta) return;
    const text = ta.value.substring(0, ta.selectionStart);
    const lines = text.split("\n");
    setCursor({ line: lines.length, col: lines[lines.length - 1].length + 1 });
  }

  const lines = code.split("\n");
  const lineCount = lines.length;

  const highlightedLines = lines.map((line, i) => {
    const spans = tokenize(line, lang);
    return (
      <div key={i} style={{ height:"1.6em", lineHeight:"1.6em", whiteSpace:"pre" }}>
        {spans.length === 0 ? "\u00A0" : spans.map((sp, j) => (
          <span key={j} style={{ color: sp.color }}>{sp.text}</span>
        ))}
      </div>
    );
  });

  return (
    <div style={{ flex:1, display:"flex", overflow:"hidden", position:"relative", background:"#060614" }}>
      {/* Line numbers */}
      <div style={{ width:52, flexShrink:0, background:"#060614", borderRight:"1px solid rgba(255,255,255,.05)", overflow:"hidden", userSelect:"none" }}>
        <div style={{ paddingTop:14, paddingBottom:14, textAlign:"right" }}>
          {Array.from({ length: lineCount }, (_, i) => (
            <div key={i} style={{
              height:"1.6em", lineHeight:"1.6em", paddingRight:12,
              fontSize:13, fontFamily:"Consolas,'Courier New',monospace",
              color: i + 1 === cursor.line ? "#a78bfa" : "#1e1e3a",
            }}>
              {i + 1}
            </div>
          ))}
        </div>
      </div>

      {/* Highlight layer (visual only) */}
      <div ref={hlRef} style={{
        position:"absolute", left:52, right:0, top:0, bottom:0,
        overflow:"hidden", pointerEvents:"none",
        padding:"14px 14px 14px 16px",
        fontSize:13, fontFamily:"Consolas,'Courier New',monospace",
        lineHeight:"1.6em", letterSpacing:0,
        whiteSpace:"pre", color:"#cccccc", background:"#060614",
      }}>
        {highlightedLines}
      </div>

      {/* Actual textarea (transparent text so we see the highlight layer) */}
      <textarea
        ref={taRef}
        value={code}
        onChange={e => onChange(e.target.value)}
        onKeyDown={onKeyDown}
        onKeyUp={onSel}
        onClick={onSel}
        onScroll={syncScroll}
        spellCheck={false}
        autoComplete="off"
        autoCorrect="off"
        autoCapitalize="off"
        style={{
          position:"absolute", left:52, right:0, top:0, bottom:0,
          background:"transparent",
          color:"transparent",
          caretColor:"#aeafad",
          fontSize:13,
          fontFamily:"Consolas,'Courier New',monospace",
          lineHeight:"1.6em",
          padding:"14px 14px 14px 16px",
          border:"none", resize:"none",
          overflow:"auto",
          outline:"none",
          tabSize:2,
          letterSpacing:0,
          zIndex:2,
          whiteSpace:"pre",
        }}
      />
    </div>
  );
}

// ── Explore Page (original Yumii home) ───────────────────────────────────────
function ExplorePage({ games, setPage, openGame, onRefresh }) {
  const [filter, setFilter] = useState("All");
  const filtered = filter === "All" ? games : games.filter(g => g.genre === filter);

  return (
    <div style={{ position:"fixed", inset:0, display:"flex", flexDirection:"column", overflow:"hidden", background:"#05050f", fontFamily:"'Nunito',system-ui,sans-serif" }}>
      <style>{`*{box-sizing:border-box}@keyframes fadeIn{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:translateY(0)}}::-webkit-scrollbar{width:8px}::-webkit-scrollbar-track{background:#0d0d1a}::-webkit-scrollbar-thumb{background:#2a2a44;border-radius:6px}`}</style>

      {/* Top bar */}
      <div style={{ height:52, flexShrink:0, background:"rgba(5,5,15,.97)", backdropFilter:"blur(16px)", borderBottom:"1px solid #16162a", display:"flex", alignItems:"center", padding:"0 20px", gap:8 }}>
        <button onClick={() => onRefresh?.()}
          style={{ background:"transparent", border:"none", cursor:"pointer", display:"flex", alignItems:"center", fontFamily:"inherit", padding:"4px 8px", borderRadius:8 }}
          onMouseEnter={e => e.currentTarget.style.opacity=".7"}
          onMouseLeave={e => e.currentTarget.style.opacity="1"}>
          <span style={{ fontFamily:"Syne", fontWeight:800, fontSize:20, background:"linear-gradient(90deg,#a78bfa,#38bdf8,#4ade80)", WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>Yumii</span>
        </button>
        <div style={{ flex:1 }}/>
        <button onClick={() => setPage("home")}
          style={{ background:"rgba(167,139,250,.1)", color:"#c4b5fd", border:"1px solid rgba(167,139,250,.25)", borderRadius:10, padding:"6px 16px", fontSize:12, fontWeight:700, cursor:"pointer", fontFamily:"inherit" }}>
          Yumii Studio →
        </button>
      </div>

      <div style={{ flex:1, overflowY:"auto" }}>
        {/* Hero */}
        <div style={{ position:"relative", height:240, overflow:"hidden", flexShrink:0 }}>
          <div style={{ position:"absolute", inset:0, background:"linear-gradient(135deg,#1a0a3a,#0a1a3a,#0a2a1a)" }}/>
          <div style={{ position:"absolute", inset:0, background:"linear-gradient(180deg,rgba(5,5,15,.1) 0%,rgba(5,5,15,.65) 55%,#05050f 100%)" }}/>
          <div style={{ position:"relative", zIndex:2, height:"100%", display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", gap:8 }}>
            <div style={{ fontFamily:"Syne", fontSize:52, fontWeight:800, color:"#fff", letterSpacing:".07em", textShadow:"0 2px 40px rgba(0,0,0,.9)", lineHeight:1 }}>EXPLORE</div>
            <div style={{ color:"rgba(255,255,255,.3)", fontSize:13 }}>Discover games built with Yumii</div>
          </div>
        </div>

        {/* Gallery */}
        <div style={{ padding:"22px 26px 56px" }}>
          <div style={{ display:"flex", alignItems:"baseline", justifyContent:"space-between", marginBottom:16 }}>
            <div style={{ fontFamily:"Syne", fontSize:18, fontWeight:800, color:"#e8e8f8" }}>All Games</div>
            <div style={{ color:"#252535", fontSize:12 }}>{filtered.length} games</div>
          </div>
          <div style={{ display:"flex", gap:7, marginBottom:18, flexWrap:"wrap" }}>
            {GENRES.map(g => (
              <div key={g} onClick={() => setFilter(g)}
                style={{ cursor:"pointer", padding:"5px 14px", borderRadius:20, fontSize:12, fontWeight:700, transition:"all .12s",
                  background: filter===g ? "rgba(167,139,250,.16)" : "rgba(255,255,255,.04)",
                  color:      filter===g ? "#c4b5fd" : "#44446a",
                  border:     "1px solid "+(filter===g ? "rgba(167,139,250,.3)" : "transparent") }}>
                {g}
              </div>
            ))}
          </div>

          {filtered.length === 0 ? (
            <div style={{ display:"flex", flexDirection:"column", alignItems:"center", padding:"52px 0", gap:12 }}>
              <div style={{ opacity:.12 }}><Icon name="gamepad-2" size={44} color="#a78bfa"/></div>
              <div style={{ color:"#252535", fontSize:14, fontWeight:700 }}>No games yet</div>
              <div style={{ color:"#1a1a2e", fontSize:12 }}>Write something in the editor and publish it!</div>
              <button onClick={() => setPage("editor")}
                style={{ background:"rgba(167,139,250,.1)", color:"#c4b5fd", padding:"8px 20px", borderRadius:14, border:"1px solid rgba(167,139,250,.25)", fontSize:13, fontWeight:700, cursor:"pointer", fontFamily:"inherit", marginTop:4 }}>
                Open Editor →
              </button>
            </div>
          ) : (
            <div style={{ display:"grid", gridTemplateColumns:"repeat(auto-fill,minmax(165px,1fr))", gap:16 }}>
              {filtered.map((g, i) => (
                <div key={g.id} onClick={() => openGame(g)}
                  style={{ cursor:"pointer", animation:"fadeIn .3s ease "+(i*.04)+"s both", transition:"transform .16s, box-shadow .16s" }}
                  onMouseEnter={e => { e.currentTarget.style.transform="translateY(-3px)"; e.currentTarget.style.boxShadow="0 8px 24px rgba(0,0,0,.4)"; }}
                  onMouseLeave={e => { e.currentTarget.style.transform=""; e.currentTarget.style.boxShadow=""; }}>
                  <Thumb game={g} size={165}/>
                  <div style={{ padding:"8px 2px 0" }}>
                    <div style={{ fontSize:13, fontWeight:800, color:"#e0e0f8", marginBottom:2, overflow:"hidden", textOverflow:"ellipsis", whiteSpace:"nowrap" }}>{g.title}</div>
                    <div style={{ fontSize:11, color:"#2a2a48", marginBottom:4 }}>{g.author}</div>
                    <div style={{ display:"flex", gap:10, fontSize:11, color:"#33334a" }}>
                      <span style={{ display:"flex", alignItems:"center", gap:3 }}><Icon name="play" size={10}/>{g.plays >= 1000 ? (g.plays/1000).toFixed(1)+"k" : g.plays}</span>
                      <span style={{ display:"flex", alignItems:"center", gap:3 }}><Icon name="heart" size={10} color="#fb7185"/>{g.likes}</span>
                    </div>
                  </div>
                </div>
              ))}
              <div onClick={() => setPage("editor")}
                style={{ border:"2px dashed #1c1c2e", borderRadius:18, display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", gap:8, minHeight:130, opacity:.4, cursor:"pointer" }}>
                <div style={{ fontSize:22, color:"#252535" }}>+</div>
                <div style={{ fontSize:10, color:"#252535", fontWeight:800, letterSpacing:".07em" }}>CREATE</div>
              </div>
            </div>
          )}
        </div>
      </div>
    </div>
  );
}


function StudioHome({ projects, games, filter, setFilter, setPage, setApid, setActiveTab, setProjects, addProject, openGame, stopCode, newProject }) {
  return (
    <div style={{ position:"fixed", inset:0, display:"flex", overflow:"hidden", background:"#0e0e16", fontFamily:"'Nunito',system-ui,sans-serif" }}>

      {/* ── Left sidebar ── */}
      <div style={{ width:220, flexShrink:0, background:"#0a0a12", borderRight:"1px solid rgba(255,255,255,.06)", display:"flex", flexDirection:"column", padding:"20px 0" }}>
        <div style={{ padding:"0 20px 20px", borderBottom:"1px solid rgba(255,255,255,.05)" }}>
          <div style={{ fontFamily:"Syne", fontSize:20, fontWeight:800, background:"linear-gradient(90deg,#a78bfa,#38bdf8)", WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>Yumii Studio</div>
          <div style={{ fontSize:10, color:"#33334a", marginTop:2 }}>Game Development Platform</div>
        </div>

        <div style={{ padding:"14px 12px 10px" }}>
          <button onClick={() => { addProject(); setPage("editor"); }}
            style={{ width:"100%", background:"linear-gradient(135deg,#7c3aed,#6d28d9)", color:"#fff", border:"none", borderRadius:10, padding:"9px 0", fontSize:13, fontWeight:800, cursor:"pointer", fontFamily:"inherit", display:"flex", alignItems:"center", justifyContent:"center", gap:7 }}>
            <span style={{ fontSize:18, lineHeight:1 }}>+</span> New Project
          </button>
        </div>

        {[
          { label:"MY PROJECTS", icon:"folder",   section:"projects"  },
          { label:"PUBLISHED",   icon:"gamepad-2", section:"published" },
          { label:"TEMPLATES",   icon:"code-2",    section:"templates" },
        ].map(item => (
          <div key={item.section} onClick={() => setFilter(item.section)}
            style={{ display:"flex", alignItems:"center", gap:10, padding:"9px 20px", cursor:"pointer", fontSize:12, fontWeight:700, transition:"all .12s",
              background:   filter===item.section ? "rgba(124,58,237,.18)" : "transparent",
              color:        filter===item.section ? "#a78bfa" : "#3a3a60",
              borderLeft:   filter===item.section ? "2px solid #7c3aed" : "2px solid transparent" }}>
            <Icon name={item.icon} size={14} color={filter===item.section?"#a78bfa":"#3a3a60"}/>
            {item.label}
          </div>
        ))}

        <div style={{ margin:"6px 12px", height:1, background:"rgba(255,255,255,.05)" }}/>

        <div style={{ flex:1 }}/>

        {/* Back to Yumii */}
        <div onClick={() => setPage("explore")}
          style={{ display:"flex", alignItems:"center", gap:10, padding:"9px 20px", cursor:"pointer", fontSize:12, fontWeight:700, transition:"all .12s", color:"#3a3a60", borderLeft:"2px solid transparent" }}
          onMouseEnter={e => { e.currentTarget.style.color="#a78bfa"; e.currentTarget.style.background="rgba(124,58,237,.1)"; }}
          onMouseLeave={e => { e.currentTarget.style.color="#3a3a60"; e.currentTarget.style.background="transparent"; }}>
          <Icon name="chevron-left" size={14} color="currentColor"/>
          Back to Yumii
        </div>

        <div style={{ padding:"12px 16px", borderTop:"1px solid rgba(255,255,255,.05)", display:"flex", alignItems:"center", gap:10 }}>
          <div style={{ width:30, height:30, borderRadius:"50%", background:"linear-gradient(135deg,#f97316,#7c3aed)", flexShrink:0 }}/>
          <div>
            <div style={{ fontSize:12, fontWeight:800, color:"#6060a0" }}>Developer</div>
            <div style={{ fontSize:10, color:"#2a2a44" }}>Free Plan</div>
          </div>
        </div>
      </div>

      {/* ── Main content ── */}
      <div style={{ flex:1, display:"flex", flexDirection:"column", overflow:"hidden" }}>

        {/* Top bar */}
        <div style={{ height:52, flexShrink:0, borderBottom:"1px solid rgba(255,255,255,.05)", display:"flex", alignItems:"center", padding:"0 24px", gap:12 }}>
          <div style={{ fontSize:16, fontWeight:800, color:"#e0e0f8" }}>
            {filter==="projects"||filter==="templates"||filter==="published" ? filter.charAt(0).toUpperCase()+filter.slice(1) : filter+" Games"}
          </div>
          <div style={{ flex:1 }}/>
          <div style={{ display:"flex", alignItems:"center", gap:8, background:"rgba(255,255,255,.05)", border:"1px solid rgba(255,255,255,.08)", borderRadius:10, padding:"6px 12px" }}>
            <Icon name="search" size={13} color="#3a3a60"/>
            <input placeholder="Search…" style={{ background:"transparent", border:"none", outline:"none", color:"#c4b5fd", fontSize:12, fontFamily:"inherit", width:160 }}/>
          </div>
        </div>

        <div style={{ flex:1, overflowY:"auto", padding:"24px 28px" }}>

          {/* MY PROJECTS */}
          {filter === "projects" && (
            <>
              <div style={{ fontSize:12, fontWeight:800, color:"#3a3a60", letterSpacing:".1em", marginBottom:16 }}>YOUR PROJECTS</div>
              <div style={{ display:"grid", gridTemplateColumns:"repeat(auto-fill,minmax(200px,1fr))", gap:14, marginBottom:32 }}>
                <div onClick={() => { addProject(); setPage("editor"); }}
                  style={{ borderRadius:14, border:"2px dashed rgba(124,58,237,.3)", background:"rgba(124,58,237,.04)", display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", gap:10, minHeight:150, cursor:"pointer", transition:"all .15s" }}
                  onMouseEnter={e => { e.currentTarget.style.background="rgba(124,58,237,.1)"; e.currentTarget.style.borderColor="rgba(124,58,237,.6)"; }}
                  onMouseLeave={e => { e.currentTarget.style.background="rgba(124,58,237,.04)"; e.currentTarget.style.borderColor="rgba(124,58,237,.3)"; }}>
                  <div style={{ width:40, height:40, borderRadius:12, background:"rgba(124,58,237,.2)", display:"flex", alignItems:"center", justifyContent:"center", fontSize:22, color:"#7c3aed" }}>+</div>
                  <div style={{ fontSize:12, fontWeight:800, color:"#7c3aed" }}>New Project</div>
                </div>
                {projects.list.map(p => {
                  const mc = MODES[p.modeId]?.color || "#a78bfa";
                  const ml = MODES[p.modeId]?.label || p.modeId;
                  return (
                    <div key={p.id} onClick={() => { setApid(p.id); setActiveTab(MODES[p.modeId].tabs[0]); setPage("editor"); }}
                      style={{ borderRadius:14, background:"rgba(255,255,255,.04)", border:"1px solid rgba(255,255,255,.07)", overflow:"hidden", cursor:"pointer", transition:"all .15s" }}
                      onMouseEnter={e => { e.currentTarget.style.background="rgba(255,255,255,.08)"; e.currentTarget.style.borderColor="rgba(167,139,250,.3)"; e.currentTarget.style.transform="translateY(-2px)"; }}
                      onMouseLeave={e => { e.currentTarget.style.background="rgba(255,255,255,.04)"; e.currentTarget.style.borderColor="rgba(255,255,255,.07)"; e.currentTarget.style.transform=""; }}>
                      <div style={{ height:90, background:`linear-gradient(135deg,${mc}22,${mc}08)`, borderBottom:"1px solid rgba(255,255,255,.05)", display:"flex", alignItems:"center", justifyContent:"center", position:"relative" }}>
                        <div style={{ width:44, height:44, borderRadius:14, background:`${mc}22`, border:`1px solid ${mc}44`, display:"flex", alignItems:"center", justifyContent:"center" }}>
                          <Icon name="code-2" size={20} color={mc}/>
                        </div>
                        <div style={{ position:"absolute", top:8, right:8, background:"rgba(0,0,0,.5)", borderRadius:6, padding:"2px 7px", fontSize:9, fontWeight:800, color:mc }}>{ml}</div>
                      </div>
                      <div style={{ padding:"10px 12px 12px" }}>
                        <div style={{ fontSize:13, fontWeight:800, color:"#e0e0f8", marginBottom:3, overflow:"hidden", textOverflow:"ellipsis", whiteSpace:"nowrap" }}>{p.name}</div>
                        <div style={{ fontSize:10, color:"#3a3a60" }}>Click to open</div>
                      </div>
                    </div>
                  );
                })}
              </div>
            </>
          )}

          {/* TEMPLATES */}
          {filter === "templates" && (
            <>
              <div style={{ fontSize:12, fontWeight:800, color:"#3a3a60", letterSpacing:".1em", marginBottom:16 }}>START FROM A TEMPLATE</div>
              <div style={{ display:"grid", gridTemplateColumns:"repeat(auto-fill,minmax(200px,1fr))", gap:14 }}>
                {Object.values(MODES).map(m => (
                  <div key={m.id}
                    onClick={() => {
                      const p = newProject(m.label + " Game");
                      p.modeId = m.id;
                      setProjects(prev => ({ list:[...prev.list, p], apid:p.id }));
                      setApid(p.id);
                      setActiveTab(m.tabs[0]);
                      setPage("editor");
                    }}
                    style={{ borderRadius:14, background:"rgba(255,255,255,.04)", border:"1px solid rgba(255,255,255,.07)", overflow:"hidden", cursor:"pointer", transition:"all .15s" }}
                    onMouseEnter={e => { e.currentTarget.style.background="rgba(255,255,255,.08)"; e.currentTarget.style.transform="translateY(-2px)"; }}
                    onMouseLeave={e => { e.currentTarget.style.background="rgba(255,255,255,.04)"; e.currentTarget.style.transform=""; }}>
                    <div style={{ height:80, background:`linear-gradient(135deg,${m.color}22,${m.color}08)`, display:"flex", alignItems:"center", justifyContent:"center" }}>
                      <div style={{ width:38, height:38, borderRadius:12, background:`${m.color}22`, border:`1px solid ${m.color}44`, display:"flex", alignItems:"center", justifyContent:"center" }}>
                        <Icon name="code-2" size={18} color={m.color}/>
                      </div>
                    </div>
                    <div style={{ padding:"10px 12px 12px" }}>
                      <div style={{ fontSize:13, fontWeight:800, color:"#e0e0f8", marginBottom:2 }}>{m.label}</div>
                      <div style={{ fontSize:10, color:"#3a3a60" }}>{m.desc}</div>
                    </div>
                  </div>
                ))}
              </div>
            </>
          )}

          {/* PUBLISHED / GENRES */}
          {filter !== "projects" && filter !== "templates" && (
            <>
              <div style={{ fontSize:12, fontWeight:800, color:"#3a3a60", letterSpacing:".1em", marginBottom:16 }}>
                {filter === "published" ? "YOUR PUBLISHED GAMES" : filter.toUpperCase()+" GAMES"}
              </div>
              {(() => {
                const list = filter==="published" ? games : filter==="All" ? games : games.filter(g=>g.genre===filter);
                return list.length === 0 ? (
                  <div style={{ display:"flex", flexDirection:"column", alignItems:"center", padding:"60px 0", gap:14 }}>
                    <div style={{ opacity:.12 }}><Icon name="gamepad-2" size={52} color="#a78bfa"/></div>
                    <div style={{ color:"#3a3a60", fontSize:14, fontWeight:800 }}>No games here yet</div>
                    <div style={{ color:"#2a2a44", fontSize:12 }}>Build something and hit Publish!</div>
                    <button onClick={() => setPage("editor")}
                      style={{ background:"rgba(124,58,237,.15)", color:"#a78bfa", padding:"8px 20px", borderRadius:10, border:"1px solid rgba(124,58,237,.3)", fontSize:13, fontWeight:700, cursor:"pointer", fontFamily:"inherit", marginTop:4 }}>
                      Open Editor →
                    </button>
                  </div>
                ) : (
                  <div style={{ display:"grid", gridTemplateColumns:"repeat(auto-fill,minmax(180px,1fr))", gap:16 }}>
                    {list.map((g,i) => (
                      <div key={g.id} onClick={() => openGame(g)}
                        style={{ cursor:"pointer", animation:"fadeIn .3s ease "+(i*.04)+"s both", borderRadius:14, overflow:"hidden", background:"rgba(255,255,255,.04)", border:"1px solid rgba(255,255,255,.07)", transition:"all .15s" }}
                        onMouseEnter={e => { e.currentTarget.style.transform="translateY(-3px)"; e.currentTarget.style.boxShadow="0 10px 30px rgba(0,0,0,.4)"; e.currentTarget.style.borderColor="rgba(167,139,250,.3)"; }}
                        onMouseLeave={e => { e.currentTarget.style.transform=""; e.currentTarget.style.boxShadow=""; e.currentTarget.style.borderColor="rgba(255,255,255,.07)"; }}>
                        <Thumb game={g} size={180}/>
                        <div style={{ padding:"10px 12px 12px" }}>
                          <div style={{ fontSize:13, fontWeight:800, color:"#e0e0f8", marginBottom:2, overflow:"hidden", textOverflow:"ellipsis", whiteSpace:"nowrap" }}>{g.title}</div>
                          <div style={{ fontSize:10, color:"#3a3a60", marginBottom:6 }}>by {g.author}</div>
                          <div style={{ display:"flex", gap:10, fontSize:10, color:"#3a3a60" }}>
                            <span style={{ display:"flex", alignItems:"center", gap:3 }}><Icon name="play" size={9}/>{g.plays>=1000?(g.plays/1000).toFixed(1)+"k":g.plays}</span>
                            <span style={{ display:"flex", alignItems:"center", gap:3 }}><Icon name="heart" size={9} color="#fb7185"/>{g.likes}</span>
                          </div>
                        </div>
                      </div>
                    ))}
                  </div>
                );
              })()}
            </>
          )}
        </div>
      </div>
    </div>
  );
}

// ── Main App ──────────────────────────────────────────────────────────────────
function newProject(name = "Untitled", modeId = "web") {
  return { id: "p" + Date.now() + Math.random().toString(36).slice(2,6), name, modeId, files: { ...DEFAULTS } };
}

export default function Yumii() {
  const [page, setPage]           = useState("explore");
  const [exploreKey, setExploreKey] = useState(0);
  const [projects, setProjects]   = useState(() => { const p = newProject("My Game"); return { list:[p], apid:p.id }; });
  const apid  = projects.apid;
  const setApid = (id) => setProjects(prev => ({ ...prev, apid: id }));
  const [activeTab, setActiveTab] = useState("html");
  const [running, setRunning]     = useState(false);
  const [games, setGames]         = useState([]);
  const [playing, setPlaying]     = useState(null);
  const [filter, setFilter]       = useState("projects");
  const [pubOpen, setPubOpen]     = useState(false);
  const [pubForm, setPubForm]     = useState({ title:"", author:"", genre:"Arcade", desc:"" });
  const [toast, setToast]         = useState(null);
  const [actPanel, setActPanel]   = useState("explorer");
  const [editingProjId, setEditingProjId] = useState(null);

  const proj    = projects.list.find(p => p.id === apid) || projects.list[0];
  const modeId  = proj.modeId;
  const files   = proj.files;

  // Force the entire DOM to fill the viewport — required for Claude artifact sandbox
  useEffect(() => {
    const style = document.createElement('style');
    style.id = 'yumii-global';
    style.textContent = `
      html, body, #root { height: 100% !important; width: 100% !important; margin: 0 !important; padding: 0 !important; overflow: hidden !important; background: #05050f !important; }
      * { box-sizing: border-box; }
      @keyframes fadeIn { from { opacity:0; transform:translateY(6px) } to { opacity:1; transform:translateY(0) } }
      @keyframes pop { from { opacity:0; transform:scale(.95) } to { opacity:1; transform:scale(1) } }
      @keyframes pulse { 0%,100% { opacity:.5 } 50% { opacity:1 } }
      @keyframes blink { 0%,100% { opacity:1 } 50% { opacity:0 } }
      ::-webkit-scrollbar { width:8px; height:8px }
      ::-webkit-scrollbar-track { background:#1e1e1e }
      ::-webkit-scrollbar-thumb { background:#424242; border-radius:6px }
      .hov-btn:hover { background:rgba(255,255,255,.08) !important }
      input:focus, select:focus, textarea:focus { outline: none }
      select option { background:#252526; color:#cccccc }
    `;
    if (!document.getElementById('yumii-global')) document.head.appendChild(style);
    // Also force root element
    const root = document.getElementById('root') || document.body;
    root.style.height = '100%';
    root.style.overflow = 'hidden';
    document.documentElement.style.height = '100%';
    document.documentElement.style.overflow = 'hidden';
  }, []);

  // Load fonts
  useEffect(() => {
    if (document.getElementById('yumii-fonts')) return;
    const link = document.createElement('link');
    link.id = 'yumii-fonts';
    link.rel = 'stylesheet';
    link.href = 'https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800;900&family=Syne:wght@700;800&family=JetBrains+Mono:wght@400;500&display=swap';
    document.head.appendChild(link);
  }, []);

  const previewRef = useRef(null);
  const playRef    = useRef(null);
  const [consoleLogs, setConsoleLogs] = useState([]);
  const [consoleOpen, setConsoleOpen] = useState(true);
  const [gamepadConnected, setGamepadConnected] = useState(false);
  function showToast(msg, err) { setToast({ msg, err }); setTimeout(() => setToast(null), 3000); }

  useEffect(() => {
    function onMsg(e) {
      if (e.data && e.data.__yumiiConsole) {
        setConsoleLogs(prev => [...prev, e.data]);
        if (e.data.text && e.data.text.includes('Controller connected')) setGamepadConnected(true);
        if (e.data.text && e.data.text.includes('Controller disconnected')) setGamepadConnected(false);
      }
    }
    function onGPConnect() { setGamepadConnected(true); }
    function onGPDisconnect() { setGamepadConnected(false); }
    window.addEventListener("message", onMsg);
    window.addEventListener("gamepadconnected", onGPConnect);
    window.addEventListener("gamepaddisconnected", onGPDisconnect);
    if (navigator.getGamepads) {
      for (const gp of navigator.getGamepads()) { if (gp) { setGamepadConnected(true); break; } }
    }
    return () => {
      window.removeEventListener("message", onMsg);
      window.removeEventListener("gamepadconnected", onGPConnect);
      window.removeEventListener("gamepaddisconnected", onGPDisconnect);
    };
  }, []);

  function runCode() {
    setConsoleLogs([]);
    setRunning(true);
    if (previewRef.current) previewRef.current.srcdoc = buildPreview(modeId, files);
  }

  function stopCode() {
    setRunning(false);
    if (previewRef.current) previewRef.current.srcdoc = "";
  }

  function openGame(g) {
    setPlaying(g);
    setGames(prev => prev.map(x => x.id === g.id ? { ...x, plays: x.plays + 1 } : x));
    setPage("play");
    setTimeout(() => { if (playRef.current) playRef.current.srcdoc = buildPreview(g.modeId, g.files || {}); }, 60);
  }

  function publishGame() {
    if (!pubForm.title || !pubForm.author) { showToast("Title and name required.", true); return; }
    const emojis  = { Arcade:"🕹️", Action:"💥", Puzzle:"🧩", Sports:"⚽", Sandbox:"🎨" };
    const bgs     = { Arcade:"linear-gradient(135deg,#1e1a08,#2a1e08)", Action:"linear-gradient(135deg,#0a0a1e,#1a0a2e)", Puzzle:"linear-gradient(135deg,#081a2a,#080e1a)", Sports:"linear-gradient(135deg,#08200a,#081a10)", Sandbox:"linear-gradient(135deg,#1e0810,#1a0a2e)" };
    const accents = { Arcade:"#dcdcaa", Action:"#c586c0", Puzzle:"#4ec9b0", Sports:"#4ade80", Sandbox:"#ce9178" };
    setGames(prev => [{ id:"g"+Date.now(), title:pubForm.title, author:pubForm.author, genre:pubForm.genre,
      emoji:emojis[pubForm.genre]||"🎮", bg:bgs[pubForm.genre]||bgs.Arcade, accent:accents[pubForm.genre]||"#569cd6",
      plays:0, likes:0, desc:pubForm.desc||"A brand new game!", modeId, files:{ ...files } }, ...prev]);
    setPubOpen(false); setPubForm({ title:"", author:"", genre:"Arcade", desc:"" });
    showToast("Published!");
  }

  function updateProj(id, fn) {
    setProjects(prev => ({ ...prev, list: prev.list.map(p => p.id === id ? fn(p) : p) }));
  }
  function setFile(key, val) { updateProj(proj.id, p => ({ ...p, files: { ...p.files, [key]: val } })); }
  function switchMode(id) { updateProj(proj.id, p => ({ ...p, modeId: id })); setActiveTab(MODES[id].tabs[0]); stopCode(); }

  function addProject() {
    const p = newProject("Untitled");
    setProjects(prev => ({ list: [...prev.list, p], apid: p.id }));
    setActiveTab(MODES[p.modeId].tabs[0]);
    stopCode();
  }
  function closeProject(id, e) {
    e.stopPropagation();
    setProjects(prev => {
      const list = prev.list.filter(p => p.id !== id);
      if (list.length === 0) { const p = newProject("Untitled"); return { list:[p], apid:p.id }; }
      const newApid = prev.apid === id ? list[list.length-1].id : prev.apid;
      if (prev.apid === id) {
        const nextProj = list.find(p => p.id === newApid);
        if (nextProj) setActiveTab(MODES[nextProj.modeId]?.tabs[0] || "html");
      }
      return { list, apid: newApid };
    });
    stopCode();
  }
  function renameProject(id, name) {
    updateProj(id, p => ({ ...p, name: name || "Untitled" }));
    setEditingProjId(null);
  }

  const mode        = MODES[modeId];
  const curTabInfo  = mode.tabInfo[activeTab] || {};
  const curFileKey  = curTabInfo.fileKey || activeTab;
  const currentCode = files[curFileKey] || "";
  const curLang     = FILE_ICONS[curFileKey] || {};
  const filtered    = filter === "All" ? games : games.filter(g => g.genre === filter);
  const lineCount   = currentCode.split("\n").length;
  const charCount   = currentCode.length;

  if (page === "explore") return (
    <div style={{ position:"fixed", inset:0, background:"#05050f" }}>
      <ExplorePage key={exploreKey} games={games} setPage={setPage} openGame={openGame} onRefresh={() => setExploreKey(k => k+1)}/>
    </div>
  );

  // ── Home page renders as completely separate full-screen component ──
  if (page === "home") return (
    <div style={{ position:"fixed", inset:0, background:"#0e0e16" }}>
      <StudioHome
        projects={projects} games={games} filter={filter}
        setFilter={setFilter} setPage={setPage} setApid={setApid}
        setActiveTab={setActiveTab} setProjects={setProjects}
        addProject={addProject} openGame={openGame}
        stopCode={stopCode} newProject={newProject}
      />
    </div>
  );

  return (
    <div style={{ position:"fixed", inset:0, fontFamily:"'Nunito',system-ui,sans-serif", background:"#05050f", color:"#e0e4f8", display:"flex", flexDirection:"column", overflow:"hidden" }}>

      {/* Toast */}
      {toast && (
        <div style={{ position:"fixed", top:14, right:14, zIndex:9999, background:toast.err?"#1c0606":"#061806", border:"1px solid "+(toast.err?"#f87171":"#4ade80"), color:toast.err?"#fca5a5":"#86efac", padding:"9px 18px", borderRadius:14, fontSize:13, fontWeight:700, animation:"fadeIn .18s ease", boxShadow:"0 8px 28px rgba(0,0,0,.7)", display:"flex", alignItems:"center", gap:8 }}>
          {toast.msg}
        </div>
      )}

      {/* Publish modal (Yumii style) */}
      {pubOpen && (
        <div style={{ position:"fixed", inset:0, background:"rgba(0,0,0,.82)", zIndex:1000, display:"flex", alignItems:"center", justifyContent:"center", backdropFilter:"blur(8px)" }} onClick={e => e.target === e.currentTarget && setPubOpen(false)}>
          <div style={{ background:"#0c0c1e", border:"1px solid #1a3028", borderRadius:20, padding:32, width:430, animation:"pop .18s ease", boxShadow:"0 24px 70px rgba(0,0,0,.9)" }}>
            <div style={{ fontFamily:"Syne", fontSize:17, fontWeight:800, color:"#4ade80", marginBottom:3, display:"flex", alignItems:"center", gap:7 }}><Icon name="rocket" size={15}/>Publish Game</div>
            <div style={{ color:"#2a2a50", fontSize:11, marginBottom:20 }}>Mode: <span style={{ color:mode.color, fontWeight:700 }}>{mode.label}</span></div>
            {[["title","Title *","My Awesome Game"],["author","Your Name *","CoolDev"],["desc","Description","A fun game…"]].map(([k,lbl,ph]) => (
              <div key={k} style={{ marginBottom:13 }}>
                <div style={{ color:"#33334a", fontSize:9, fontWeight:800, letterSpacing:".1em", marginBottom:4 }}>{lbl.toUpperCase()}</div>
                <input value={pubForm[k]||""} onChange={e => setPubForm(p=>({...p,[k]:e.target.value}))} placeholder={ph}
                  style={{ width:"100%", background:"#06061a", border:"1px solid #1c1c30", borderRadius:12, color:"#d8dcf4", padding:"8px 11px", fontSize:13, fontFamily:"inherit" }}/>
              </div>
            ))}
            <div style={{ marginBottom:20 }}>
              <div style={{ color:"#33334a", fontSize:9, fontWeight:800, letterSpacing:".1em", marginBottom:4 }}>GENRE</div>
              <select value={pubForm.genre} onChange={e => setPubForm(p=>({...p,genre:e.target.value}))}
                style={{ width:"100%", background:"#06061a", border:"1px solid #1c1c30", borderRadius:12, color:"#d8dcf4", padding:"8px 11px", fontSize:13, fontFamily:"inherit" }}>
                {["Arcade","Action","Puzzle","Sports","Sandbox"].map(g => <option key={g}>{g}</option>)}
              </select>
            </div>
            <div style={{ display:"flex", gap:9, justifyContent:"flex-end" }}>
              <button onClick={() => setPubOpen(false)}
                style={{ background:"transparent", color:"#33334a", padding:"7px 16px", borderRadius:12, border:"1px solid #1e1e30", fontSize:13, cursor:"pointer", fontFamily:"inherit" }}>Cancel</button>
              <button onClick={publishGame}
                style={{ background:"linear-gradient(135deg,#064a38,#053d2e)", color:"#6ee7b7", padding:"7px 20px", borderRadius:12, border:"1px solid #064a38", fontSize:13, fontWeight:700, cursor:"pointer", fontFamily:"inherit" }}>Publish →</button>
            </div>
          </div>
        </div>
      )}

      {/* ── EDITOR ── */}
      {page === "editor" && (
        <div style={{ flex:1, display:"flex", flexDirection:"column", overflow:"hidden", background:"#05050f", fontFamily:"'Nunito',system-ui,sans-serif" }}>

          {/* ── Project tabs bar ── */}
          <div style={{ height:40, flexShrink:0, display:"flex", alignItems:"center", gap:4, padding:"0 10px", background:"rgba(255,255,255,.02)", borderBottom:"1px solid rgba(255,255,255,.05)", overflowX:"auto" }}>
            {/* Yumii logo + home button */}
            <div onClick={() => { setPage("explore"); stopCode(); }}
              style={{ height:28, padding:"0 12px", borderRadius:10, background:"transparent", color:"#3a3a60", fontSize:12, fontWeight:700, cursor:"pointer", display:"flex", alignItems:"center", gap:7, flexShrink:0, transition:"all .12s" }}
              onMouseEnter={e => e.currentTarget.style.background="rgba(167,139,250,.08)"}
              onMouseLeave={e => e.currentTarget.style.background="transparent"}>
              <Icon name="chevron-left" size={12} color="#3a3a60"/>
              <span style={{ fontFamily:"Syne", fontWeight:800, fontSize:13, background:"linear-gradient(90deg,#a78bfa,#38bdf8)", WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>Yumii</span>
            </div>
            <div style={{ width:1, height:18, background:"rgba(255,255,255,.07)", flexShrink:0, margin:"0 4px" }}/>
            {projects.list.map(p => (
              <div key={p.id} onClick={() => { setApid(p.id); setActiveTab(MODES[p.modeId].tabs[0]); stopCode(); }}
                style={{ display:"flex", alignItems:"center", gap:6, padding:"0 10px 0 12px", height:28, borderRadius:10, flexShrink:0, cursor:"pointer", fontSize:12, fontWeight:700, transition:"all .12s",
                  background: p.id === apid ? "rgba(167,139,250,.18)" : "rgba(255,255,255,.04)",
                  border: p.id === apid ? "1px solid rgba(167,139,250,.3)" : "1px solid transparent",
                  color: p.id === apid ? "#c4b5fd" : "#3a3a60" }}>
                {editingProjId === p.id ? (
                  <input autoFocus defaultValue={p.name}
                    style={{ background:"transparent", border:"none", outline:"none", color:"#c4b5fd", fontFamily:"inherit", fontSize:12, fontWeight:700, width:90 }}
                    onBlur={e => renameProject(p.id, e.target.value)}
                    onKeyDown={e => { if (e.key==="Enter") renameProject(p.id, e.target.value); if (e.key==="Escape") setEditingProjId(null); }}
                    onClick={e => e.stopPropagation()}/>
                ) : (
                  <span onDoubleClick={e => { e.stopPropagation(); setEditingProjId(p.id); }}>{p.name}</span>
                )}
                <span onClick={e => closeProject(p.id, e)}
                  style={{ opacity:.4, fontSize:14, lineHeight:1, padding:"0 2px", borderRadius:4, cursor:"pointer" }}>×</span>
              </div>
            ))}
            <button onClick={addProject}
              style={{ height:28, width:28, borderRadius:10, border:"1px dashed rgba(255,255,255,.1)", background:"transparent", color:"#3a3a60", fontSize:18, cursor:"pointer", display:"flex", alignItems:"center", justifyContent:"center", flexShrink:0, lineHeight:1 }}>+</button>
            <div style={{ flex:1 }}/>
            <button onClick={() => setPubOpen(true)}
              style={{ height:28, padding:"0 14px", borderRadius:10, background:"rgba(16,185,129,.13)", color:"#34d399", border:"1px solid rgba(16,185,129,.28)", fontSize:12, fontWeight:700, cursor:"pointer", fontFamily:"inherit", display:"flex", alignItems:"center", gap:6, flexShrink:0 }}>
              <Icon name="rocket" size={12} color="#34d399"/> Publish
            </button>
          </div>

        <div style={{ flex:1, display:"flex", overflow:"hidden", padding:10, gap:8 }}>

          {/* Activity bar — floating pill */}
          <div style={{ width:48, flexShrink:0, background:"rgba(255,255,255,.04)", border:"1px solid rgba(255,255,255,.07)", borderRadius:18, display:"flex", flexDirection:"column", alignItems:"center", paddingTop:10, paddingBottom:10, gap:4, backdropFilter:"blur(12px)" }}>
            {[
              { id:"explorer", icon:(s)=><Icon name="folder"   size={s}/>, title:"Explorer" },
              { id:"langs",    icon:(s)=><Icon name="code-2"    size={s}/>, title:"Languages" },
              { id:"search",   icon:(s)=><Icon name="search"    size={s}/>, title:"Search" },
            ].map(item => (
              <div key={item.id} onClick={() => setActPanel(prev => prev === item.id ? null : item.id)}
                title={item.title}
                style={{ width:36, height:36, display:"flex", alignItems:"center", justifyContent:"center", cursor:"pointer", color:actPanel===item.id?"#c4b5fd":"#3a3a60", background:actPanel===item.id?"rgba(167,139,250,0.18)":"transparent", borderRadius:12, transition:"all .15s" }}>
                {item.icon(16)}
              </div>
            ))}
            <div style={{ flex:1 }}/>
            <div style={{ width:36, height:36, display:"flex", alignItems:"center", justifyContent:"center", color:"#2a2a44", borderRadius:12, cursor:"pointer" }}><Icon name="settings" size={16}/></div>
          </div>

          {/* Side panel — floating card */}
          {actPanel && (
            <div style={{ width:210, flexShrink:0, background:"rgba(255,255,255,.04)", border:"1px solid rgba(255,255,255,.07)", borderRadius:18, display:"flex", flexDirection:"column", overflow:"hidden", backdropFilter:"blur(12px)" }}>
              {actPanel === "explorer" && (
                <>
                  <div style={{ padding:"12px 14px 10px", fontSize:9, fontWeight:800, color:"#44446a", letterSpacing:".14em", textTransform:"uppercase" }}>Explorer</div>
                  <div style={{ width:"calc(100% - 16px)", height:1, background:"rgba(255,255,255,.06)", margin:"0 8px 8px" }}/>
                  <div style={{ padding:"4px 8px", flex:1, overflowY:"auto" }}>
                    <div style={{ padding:"3px 8px", fontSize:10, color:"#2a2a50", fontFamily:"Consolas,monospace", display:"flex", alignItems:"center", gap:5, marginBottom:4 }}>
                      <span style={{ fontSize:9 }}>▾</span>
                      <span>YUMII PROJECT</span>
                    </div>
                    {mode.tabs.map(tabKey => {
                      const info = mode.tabInfo[tabKey];
                      const fk = info.fileKey;
                      const fi = FILE_ICONS[fk] || {};
                      const isActive = activeTab === tabKey;
                      return (
                        <div key={tabKey} onClick={() => setActiveTab(tabKey)}
                          style={{ padding:"7px 10px 7px 18px", marginBottom:2, fontSize:12, fontFamily:"Consolas,monospace", display:"flex", alignItems:"center", gap:8, cursor:"pointer", background:isActive?"rgba(167,139,250,.15)":"transparent", color:isActive?"#c4b5fd":"#44446a", borderRadius:12, transition:"all .12s" }}>
                          <span>{info.label}</span>
                        </div>
                      );
                    })}
                  </div>
                </>
              )}
              {actPanel === "langs" && (
                <>
                  <div style={{ padding:"12px 14px 10px", fontSize:9, fontWeight:800, color:"#44446a", letterSpacing:".14em", textTransform:"uppercase" }}>Languages</div>
                  <div style={{ width:"calc(100% - 16px)", height:1, background:"rgba(255,255,255,.06)", margin:"0 8px 8px" }}/>
                  <div style={{ flex:1, overflowY:"auto", padding:"4px 8px" }}>
                    {Object.values(MODES).map(m => (
                      <div key={m.id} onClick={() => switchMode(m.id)}
                        style={{ padding:"9px 10px", marginBottom:2, cursor:"pointer", background:modeId===m.id?"rgba(167,139,250,.15)":"transparent", borderRadius:12, transition:"all .12s" }}>
                        <div style={{ display:"flex", alignItems:"center", gap:9 }}>
                          <div>
                            <div style={{ fontSize:12, fontWeight:700, color:modeId===m.id?"#c4b5fd":"#44446a" }}>{m.label}</div>
                            <div style={{ fontSize:10, color:modeId===m.id?"#a78bfa":"#6060a0", fontFamily:"Consolas,monospace", marginTop:1 }}>{m.desc}</div>
                          </div>
                        </div>
                      </div>
                    ))}
                  </div>
                </>
              )}
              {actPanel === "search" && (
                <>
                  <div style={{ padding:"12px 14px 10px", fontSize:9, fontWeight:800, color:"#44446a", letterSpacing:".14em", textTransform:"uppercase" }}>Search</div>
                  <div style={{ width:"calc(100% - 16px)", height:1, background:"rgba(255,255,255,.06)", margin:"0 8px 8px" }}/>
                  <div style={{ padding:"4px 8px" }}>
                    <input placeholder="Search…" style={{ width:"100%", background:"rgba(255,255,255,.06)", border:"1px solid rgba(255,255,255,.1)", borderRadius:12, color:"#c4b5fd", padding:"8px 12px", fontSize:12, fontFamily:"Consolas,monospace" }}/>
                  </div>
                  <div style={{ padding:"10px 16px", fontSize:11, color:"#2a2a44", fontFamily:"Consolas,monospace" }}>Press Enter to search in files</div>
                </>
              )}
            </div>
          )}

          {/* ── Editor main — floating card ── */}
          <div style={{ flex:1, display:"flex", flexDirection:"column", overflow:"hidden", background:"rgba(255,255,255,.035)", border:"1px solid rgba(255,255,255,.07)", borderRadius:18, backdropFilter:"blur(12px)" }}>

            {/* Tab bar */}
            <div style={{ height:44, background:"transparent", borderBottom:"1px solid rgba(255,255,255,.06)", display:"flex", alignItems:"center", flexShrink:0, overflowX:"auto", padding:"0 8px", gap:4 }}>
              {mode.tabs.map(tabKey => {
                const info    = mode.tabInfo[tabKey];
                const fk      = info.fileKey;
                const fi      = FILE_ICONS[fk] || {};
                const isActive = activeTab === tabKey;
                return (
                  <div key={tabKey} onClick={() => setActiveTab(tabKey)}
                    style={{ minWidth:110, maxWidth:170, padding:"0 14px", height:32, display:"flex", alignItems:"center", gap:7, cursor:"pointer", fontSize:12, fontFamily:"Consolas,monospace", background:isActive?"rgba(167,139,250,.15)":"transparent", color:isActive?"#c4b5fd":"#33334a", borderRadius:12, flexShrink:0, transition:"all .12s", border:isActive?"1px solid rgba(167,139,250,.25)":"1px solid transparent" }}>
                    <span style={{ overflow:"hidden", textOverflow:"ellipsis", whiteSpace:"nowrap" }}>{info.label}</span>
                  </div>
                );
              })}
              <div style={{ flex:1 }}/>
              {/* Run/Stop/Reset */}
              <div style={{ display:"flex", alignItems:"center", gap:6, paddingRight:4 }}>
                <button onClick={runCode}
                  style={{ background:"rgba(16,185,129,.15)", color:"#34d399", border:"1px solid rgba(16,185,129,.3)", borderRadius:12, padding:"6px 16px", fontSize:12, cursor:"pointer", fontFamily:"inherit", fontWeight:700, display:"flex", alignItems:"center", gap:5 }}>
                  <Icon name="play" size={10}/> Run
                </button>
                {running && (
                  <button onClick={stopCode}
                    style={{ background:"rgba(244,63,94,.1)", color:"#fb7185", border:"1px solid rgba(244,63,94,.25)", borderRadius:12, padding:"6px 14px", fontSize:12, cursor:"pointer", fontFamily:"inherit", fontWeight:700, display:"flex", alignItems:"center", gap:5 }}>
                    <Icon name="square" size={10}/> Stop
                  </button>
                )}
                <button onClick={() => { setFile(curFileKey, DEFAULTS[curFileKey] || ""); stopCode(); }}
                  style={{ background:"rgba(255,255,255,.05)", color:"#44446a", border:"1px solid rgba(255,255,255,.08)", borderRadius:10, padding:"6px 10px", fontSize:14, cursor:"pointer", display:"flex", alignItems:"center" }}
                  title="Reset file"><Icon name="rotate-ccw" size={13}/></button>
              </div>
            </div>

            {/* Breadcrumb */}
            <div style={{ height:28, background:"transparent", display:"flex", alignItems:"center", padding:"0 16px", gap:5, flexShrink:0 }}>
              <span style={{ fontSize:11, color:"#2a2a44", fontFamily:"Consolas,monospace" }}>project</span>
              <span style={{ fontSize:11, color:"#2a2a3a" }}>/</span>
              <span style={{ fontSize:11, color:"#6060a0", fontFamily:"Consolas,monospace" }}>{curTabInfo.label || "untitled"}</span>
            </div>

            {/* Editor + preview split */}
            <div style={{ flex:1, display:"flex", overflow:"hidden", gap:8, padding:"0 8px 8px" }}>

              {/* Code editor */}
              <div style={{ flex:1, display:"flex", flexDirection:"column", overflow:"hidden", background:"#060614", borderRadius:14, border:"1px solid rgba(255,255,255,.06)" }}>
                <CodeEditor
                  code={currentCode}
                  onChange={val => setFile(curFileKey, val)}
                  lang={curFileKey}
                  onRun={runCode}
                />
              </div>

              {/* Preview panel */}
              <div style={{ width:430, flexShrink:0, background:"rgba(255,255,255,.025)", border:"1px solid rgba(255,255,255,.06)", borderRadius:14, display:"flex", flexDirection:"column", overflow:"hidden" }}>
                {/* Preview header */}
                <div style={{ height:40, display:"flex", alignItems:"center", padding:"0 14px", gap:10, flexShrink:0, borderBottom:"1px solid rgba(255,255,255,.06)" }}>
                  <span style={{ fontSize:11, fontWeight:800, color:"#44446a", letterSpacing:".05em" }}>PREVIEW</span>
                  <div style={{ flex:1 }}/>
                  {gamepadConnected && (
                    <div style={{ display:"flex", alignItems:"center", gap:5, background:"rgba(99,102,241,.1)", border:"1px solid rgba(99,102,241,.25)", borderRadius:20, padding:"3px 10px" }}>
                      <Icon name="gamepad-2" size={11} color="#818cf8"/>
                      <span style={{ fontSize:10, color:"#818cf8", fontWeight:700 }}>controller</span>
                    </div>
                  )}
                  {running && (
                    <div style={{ display:"flex", alignItems:"center", gap:6, background:"rgba(52,211,153,.1)", border:"1px solid rgba(52,211,153,.25)", borderRadius:20, padding:"3px 10px" }}>
                      <div style={{ width:6, height:6, borderRadius:"50%", background:"#34d399", animation:"pulse 1.4s infinite" }}/>
                      <span style={{ fontSize:10, color:"#34d399", fontWeight:700 }}>running</span>
                    </div>
                  )}
                </div>

                {/* Preview content */}
                <div style={{ display:"flex", alignItems:"center", justifyContent:"center", padding:"10px 0 0" }}>
                  {running ? (
                    <iframe ref={previewRef}
                      style={{ width:400, height:400, border:"1px solid rgba(100,80,220,.2)", borderRadius:16, background:"#05050f", boxShadow:"0 0 60px rgba(100,80,220,.12),0 8px 40px rgba(0,0,0,.6)" }}
                      sandbox="allow-scripts" title="preview"/>
                  ) : (
                    <div onClick={runCode}
                      style={{ width:400, height:400, background:"rgba(255,255,255,.02)", border:"1px solid rgba(255,255,255,.07)", borderRadius:16, display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", gap:18, cursor:"pointer", transition:"all .15s" }}
                      onMouseEnter={e => { e.currentTarget.style.background="rgba(167,139,250,.05)"; e.currentTarget.style.borderColor="rgba(167,139,250,.25)"; }}
                      onMouseLeave={e => { e.currentTarget.style.background="rgba(255,255,255,.02)"; e.currentTarget.style.borderColor="rgba(255,255,255,.07)"; }}>
                      <div style={{ width:64, height:64, background:"rgba(167,139,250,.12)", border:"1px solid rgba(167,139,250,.28)", borderRadius:22, display:"flex", alignItems:"center", justifyContent:"center" }}>
                        <Icon name="gamepad-2" size={32} color="rgba(167,139,250,.5)"/>
                      </div>
                      <div style={{ textAlign:"center", gap:4 }}>
                        <div style={{ color:"#6060a0", fontSize:14, fontWeight:700, marginBottom:5 }}>{mode.label}</div>
                        <div style={{ color:"#2a2a44", fontSize:11, fontFamily:"Consolas,monospace" }}>{mode.desc}</div>
                      </div>
                      <div style={{ background:"rgba(16,185,129,.15)", color:"#34d399", padding:"9px 26px", borderRadius:14, border:"1px solid rgba(16,185,129,.3)", fontSize:13, fontWeight:700, display:"flex", alignItems:"center", gap:7 }}>
                        <Icon name="play" size={12}/> Run Code
                      </div>
                      <div style={{ color:"#2a2a44", fontSize:10, fontFamily:"Consolas,monospace" }}>Ctrl + Enter</div>
                    </div>
                  )}
                </div>

                {/* Console panel */}
                <div style={{ borderTop:"1px solid rgba(255,255,255,.06)", marginTop:8, display:"flex", flexDirection:"column", maxHeight: consoleOpen ? 160 : 32, transition:"max-height .2s ease", overflow:"hidden", flexShrink:0 }}>
                  {/* Console header */}
                  <div onClick={() => setConsoleOpen(o => !o)}
                    style={{ height:32, display:"flex", alignItems:"center", padding:"0 12px", gap:8, cursor:"pointer", userSelect:"none", flexShrink:0 }}>
                    <span style={{ display:"flex", transform: consoleOpen ? "rotate(-90deg)" : "rotate(90deg)", transition:"transform .2s" }}>
                      <Icon name="chevron-left" size={11} color="#44446a"/>
                    </span>
                    <span style={{ fontSize:10, fontWeight:800, color:"#44446a", letterSpacing:".1em" }}>CONSOLE</span>
                    {consoleLogs.filter(l => l.level === "error").length > 0 && (
                      <span style={{ background:"rgba(244,63,94,.2)", color:"#fb7185", fontSize:9, fontWeight:800, padding:"1px 6px", borderRadius:8 }}>
                        {consoleLogs.filter(l => l.level === "error").length} error{consoleLogs.filter(l => l.level === "error").length > 1 ? "s" : ""}
                      </span>
                    )}
                    <div style={{ flex:1 }}/>
                    {consoleLogs.length > 0 && (
                      <span onClick={e => { e.stopPropagation(); setConsoleLogs([]); }}
                        style={{ fontSize:9, color:"#33334a", cursor:"pointer", padding:"2px 6px", borderRadius:6, background:"rgba(255,255,255,.05)" }}>clear</span>
                    )}
                  </div>
                  {/* Console entries */}
                  <div style={{ flex:1, overflowY:"auto", padding:"0 12px 8px", fontFamily:"Consolas,monospace", fontSize:11 }}>
                    {consoleLogs.length === 0 ? (
                      <div style={{ color:"#2a2a44", padding:"4px 0" }}>No output yet.</div>
                    ) : consoleLogs.map((log, i) => (
                      <div key={i} style={{
                        color: log.level === "error" ? "#f48771" : log.level === "warn" ? "#cca700" : "#b0b0d0",
                        borderLeft: log.level === "error" ? "2px solid #f4877155" : log.level === "warn" ? "2px solid #cca70055" : "2px solid transparent",
                        paddingLeft:6, marginBottom:2, lineHeight:1.5, whiteSpace:"pre-wrap", wordBreak:"break-all"
                      }}>
                        <span style={{ opacity:.45, marginRight:6 }}>{log.level === "error" ? "✖" : log.level === "warn" ? "⚠" : "›"}</span>
                        {log.text}
                      </div>
                    ))}
                  </div>
                </div>
              </div>
            </div>

            {/* Status bar */}
            <div style={{ height:28, background:"rgba(167,139,250,.06)", borderTop:"1px solid rgba(255,255,255,.05)", borderRadius:"0 0 18px 18px", display:"flex", alignItems:"center", padding:"0 16px", gap:10, flexShrink:0 }}>
              <span style={{ fontSize:10, color:"#a78bfa", fontFamily:"Consolas,monospace", fontWeight:700, display:"flex", alignItems:"center", gap:4 }}><Icon name="git-branch" size={11}/>main</span>
              <div style={{ width:1, height:10, background:"rgba(255,255,255,.08)" }}/>
              {running && (
                <>
                    <span style={{ fontSize:10, color:"#34d399", fontFamily:"Consolas,monospace", fontWeight:700, display:"flex", alignItems:"center", gap:4 }}>
                    <span style={{ width:6, height:6, borderRadius:"50%", background:"#34d399", display:"inline-block", animation:"pulse 1.4s infinite" }}/> Running
                  </span>
                  <div style={{ width:1, height:10, background:"rgba(255,255,255,.08)" }}/>
                </>
              )}
              <div style={{ flex:1 }}/>
              <span style={{ fontSize:10, color:"#44446a", fontFamily:"Consolas,monospace" }}>{curLang.lang || "Plain Text"}</span>
              <div style={{ width:1, height:10, background:"rgba(255,255,255,.08)" }}/>
              <span style={{ fontSize:10, color:"#44446a", fontFamily:"Consolas,monospace" }}>{lineCount} lines</span>
              <div style={{ width:1, height:10, background:"rgba(255,255,255,.08)" }}/>
              <span style={{ fontSize:10, color:"#44446a", fontFamily:"Consolas,monospace" }}>UTF-8</span>
              <div style={{ width:1, height:10, background:"rgba(255,255,255,.08)" }}/>
              <span style={{ fontSize:10, color:"#44446a", fontFamily:"Consolas,monospace" }}>Spaces: 2</span>
            </div>
          </div>
        </div>
        </div>
      )}
      {/* ── PLAY (Yumii gaming aesthetic) ── */}
      {page === "play" && playing && (
        <div style={{ flex:1, overflow:"auto", display:"flex", flexDirection:"column", alignItems:"center", padding:24, gap:16, background:"#05050f", fontFamily:"'Nunito',system-ui,sans-serif" }}>
          <div style={{ display:"flex", alignItems:"center", gap:10, width:"100%", maxWidth:800, flexWrap:"wrap" }}>
            <button onClick={() => { setPage("explore"); if (playRef.current) playRef.current.srcdoc = ""; }}
              style={{ background:"rgba(255,255,255,.05)", color:"#44446a", padding:"6px 14px", borderRadius:12, border:"1px solid #1e1e2e", fontSize:12, fontWeight:700, cursor:"pointer", fontFamily:"inherit", display:"flex", alignItems:"center", gap:5 }}><Icon name="chevron-left" size={13}/>Back</button>
            <div style={{ fontFamily:"Syne", color:"#e8e8f8", fontSize:17, fontWeight:800 }}>{playing.title}</div>
            <div style={{ color:"#252545", fontSize:12 }}>by {playing.author}</div>
            <div style={{ background:playing.accent+"1a", color:playing.accent, padding:"3px 10px", borderRadius:12, fontSize:10, fontWeight:800, border:"1px solid "+playing.accent+"33" }}>{playing.genre}</div>
            {playing.modeId && <div style={{ color:(MODES[playing.modeId]||{color:"#888"}).color, fontSize:11, fontWeight:700, display:"flex", alignItems:"center", gap:4 }}>{(MODES[playing.modeId]||{}).label}</div>}
            <div style={{ flex:1 }}/>
            <button onClick={() => { updateProj(proj.id, p => ({ ...p, modeId: playing.modeId||"web", files: playing.files||{} })); setActiveTab(MODES[playing.modeId||"web"].tabs[0]); setPage("editor"); if (playRef.current) playRef.current.srcdoc = ""; }}
              style={{ background:"rgba(99,102,241,.12)", color:"#818cf8", padding:"6px 14px", borderRadius:12, border:"1px solid rgba(99,102,241,.25)", fontSize:12, fontWeight:700, cursor:"pointer", fontFamily:"inherit", display:"flex", alignItems:"center", gap:5 }}><Icon name="pencil" size={13}/>Edit</button>
            <button onClick={() => setGames(prev => prev.map(g => g.id===playing.id?{...g,likes:g.likes+1}:g))}
              style={{ background:"rgba(244,63,94,.08)", color:"#fb7185", padding:"6px 14px", borderRadius:12, border:"1px solid rgba(244,63,94,.2)", fontSize:12, fontWeight:700, cursor:"pointer", fontFamily:"inherit", display:"flex", alignItems:"center", gap:5 }}><Icon name="heart" size={13}/>Like</button>
          </div>

          <iframe ref={playRef} style={{ width:400, height:400, border:"1px solid #1e1e3a", borderRadius:18, background:"#05050f", boxShadow:"0 0 60px rgba(100,80,220,.12),0 8px 40px rgba(0,0,0,.5)", flexShrink:0 }} sandbox="allow-scripts" title="play"/>

          <div style={{ color:"#252545", fontSize:13, maxWidth:420, textAlign:"center", lineHeight:1.65 }}>{playing.desc}</div>

          {games.filter(g => g.id !== playing.id).length > 0 && (
            <div style={{ width:"100%", maxWidth:800 }}>
              <div style={{ fontFamily:"Syne", fontSize:13, fontWeight:800, color:"#33334a", marginBottom:12 }}>More Games</div>
              <div style={{ display:"flex", gap:12, overflowX:"auto", paddingBottom:8 }}>
                {games.filter(g => g.id !== playing.id).slice(0, 5).map(g => (
                  <div key={g.id} onClick={() => openGame(g)} style={{ flexShrink:0, width:112, cursor:"pointer", transition:"transform .15s" }}
                    onMouseEnter={e => e.currentTarget.style.transform="translateY(-2px)"}
                    onMouseLeave={e => e.currentTarget.style.transform=""}>
                    <Thumb game={g} size={112}/>
                    <div style={{ fontSize:11, fontWeight:800, color:"#b0b4d0", marginTop:5, overflow:"hidden", textOverflow:"ellipsis", whiteSpace:"nowrap" }}>{g.title}</div>
                  </div>
                ))}
              </div>
            </div>
          )}
        </div>
      )}
      {page === "play" && !playing && (
        <div style={{ flex:1, display:"flex", alignItems:"center", justifyContent:"center" }}>
          <button onClick={() => setPage("explore")}
            style={{ background:"rgba(167,139,250,.1)", color:"#c4b5fd", padding:"10px 24px", borderRadius:14, border:"1px solid rgba(167,139,250,.25)", fontSize:13, fontWeight:700, cursor:"pointer", fontFamily:"inherit" }}>
            ← Back to Explore
          </button>
        </div>
      )}
    </div>
  );
}
