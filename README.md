<h1 align="center">Hi, I'm Krischan 👋</h1>
<p align="center">
  <strong>Full-Stack Web Dev (React/Next.js) • Unity/C# Game Developer • Linux & Windows Server</strong><br/>
  I build fast web apps, ship games with Unity, and maintain production servers.
</p>

<p align="center">
  <a href="https://github.com/Krischan-Klug?tab=followers">
    <img alt="GitHub followers" src="https://img.shields.io/github/followers/Krischan-Klug?label=Follow&style=social">
  </a>
  <img alt="Profile views" src="https://komarev.com/ghpvc/?username=Krischan-Klug&style=flat&label=Views">
</p>

---

## 🪪 About Me (as an object)
```javascript
const krischan = {
  name: "Krischan Klug",
  roles: ["Full-Stack Web Dev", "Unity Game Developer", "Server Admin"],
  tech: {
    web: ["React", "Next.js", "Node.js", "TypeScript/JavaScript", "MongoDB"],
    game: ["Unity", "C#"],
    ops: ["Linux", "Windows Server", "CI/CD", "Docker (Basics)"]
  },
  focus: [
    "Clean auth & API design",
    "Reusable components",
    "Performance & Developer Experience",
    "Secure deployments & monitoring"
  ],
  currently: "Refining a Next.js architecture with clear auth, stable state management, and MySQL access",
  values: ["Clean Code", "Transparent docs", "Pragmatic solutions"]
};

``` 
## 🔧 Currently

```javascript
import React, { StrictMode } from "react";
import { createRoot } from "react-dom/client";
import App from "./App";

import * as db from "./backend/db";
import * as api from "./backend/api";
import * as auth from "./backend/auth";
import * as rt from "./backend/realtime"; // websockets/events

(async function boot() {
  await db.connect();
  await api.warmup({ cache: true });
  await auth.init({ strategy: "jwt" });
  rt.connect();

  console.log(" DB +  API +  Auth => ready.");

  const root = createRoot(document.getElementById("root"));
  root.render(
    <StrictMode>
      <App />
    </StrictMode>
  );

  api.health().then(({ ok }) => ok && console.log("/api/health OK"));
})();
```

## ⌨️ Tech Stack
**Core:** HTML • CSS • JS • C# • C++ • Python <br>
**Web:** React • Next.js • TypeScript/JavaScript • Node.js  <br>
**Backend/DB:** REST • MongoDB • JWT/NextAuth • WebSockets  <br>
**Game:** Unity <br>
**Ops:** Linux/Windows Server • Git • CI/CD • Docker (Basics) <br>

---

## 📊 Strengths
- Structured apps with clean auth & API layer  
- UI/UX with a focus on **performance**, **state management**, and **reusability**  
- **Unity** games: gameplay programming, tooling, packets (**C#**)  
- **Server Ops**: deployments, logging, monitoring, automation

---

## 🛠️ Languages & Tools
<p align="center">
  <!-- Icons: https://github.com/MikeCodesDotNET/ColoredBadges -->
  <img src="https://raw.githubusercontent.com/8bithemant/8bithemant/master/svg/dev/languages/csharp.svg" alt="csharp" style="vertical-align:top; margin:6px">
  <img src="https://github.com/MikeCodesDotNET/ColoredBadges/blob/master/svg/dev/frameworks/unity.svg" alt="Unity" style="vertical-align:top; margin:6px">
  <img src="https://raw.githubusercontent.com/8bithemant/8bithemant/master/svg/dev/languages/html.svg" alt="html" style="vertical-align:top; margin:6px">
  <img src="https://github.com/MikeCodesDotNET/ColoredBadges/blob/master/svg/dev/languages/css3.svg" alt="css" style="vertical-align:top; margin:6px">
  <img src="https://raw.githubusercontent.com/8bithemant/8bithemant/master/svg/dev/languages/js.svg" alt="js" style="vertical-align:top; margin:6px">
  <img src="https://github.com/MikeCodesDotNET/ColoredBadges/blob/master/svg/dev/frameworks/react.svg" alt="React" style="vertical-align:top; margin:6px">
  <img src="https://raw.githubusercontent.com/8bithemant/8bithemant/master/svg/dev/misc/chrome.svg" alt="chrome" style="vertical-align:top; margin:6px">
  <img src="https://raw.githubusercontent.com/8bithemant/8bithemant/master/svg/dev/tools/visualstudio_code.svg" alt="vscode" style="vertical-align:top; margin:6px">
</p>



