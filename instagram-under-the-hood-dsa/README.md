# Instagram Under the Hood: Interactive Data Structure Visualizer

An academic, interactive single-page prototype for Data Structures & Algorithms (DSA) courses demonstrating how core Instagram features map to fundamental data structures.

> **Activity**: Data Structures & Algorithms Activity  
> **Institution**: Zeal College of Engineering and Research, Pune  

---

## 🚀 Features & Data Structure Mappings

| Module | Core Instagram Feature | Data Structure | Key Operations & Complexity |
| :--- | :--- | :--- | :--- |
| **Module 1** | **Social Follower Graph** | Directed Graph + Dual Hash Sets (`Map<User, Set<User>>`) | Follow / Unfollow: $O(1)$<br>Check Follow: $O(1)$<br>Mutuals $\text{Out}(A) \cap \text{In}(B)$: $O(\min(d_A, d_B))$ |
| **Module 2** | **Algorithmic Home Feed** | Max-Heap / Priority Queue | Floyd Bottom-Up Heap: $O(N)$<br>Extract Top-$K$: $O(K \log N)$<br>Push vs Pull Celebrity Fan-out |
| **Module 3** | **Direct Messaging (DM)** | FIFO Queue + Doubly Linked List (DLL) | Broker Buffer: $O(1)$ Enqueue / Dequeue<br>History Scroll Prepend: $O(1)$<br>Monotonic Unread Badge Sync |
| **Module 4** | **Story Editor** | Dual LIFO Stacks + Command Pattern | Undo / Redo: $O(1)$<br>Bounded Stack Capacity $S_{\max} = 50$<br>Memory Savings: $>99.9\%$ vs 8.3 MB RGBA frames |
| **Module 5** | **Complexity Summary** | Empirical Profiler & Matrix | Live synthetic in-browser benchmarking with real-time microsecond performance profiling |

---

## 📦 What's Inside

- `index.html` — Completely self-contained single-page web application (HTML5, CSS3, vanilla JavaScript). Zero external dependencies or build pipelines needed.
- `server.ps1` — Lightweight PowerShell static HTTP server script for instant local hosting on Windows.
- `vercel.json` & `netlify.toml` — Pre-configured deployment manifests for 1-click cloud hosting.

---

## 💻 How to Run Locally

### Option 1: Direct File Open (Zero Setup)
Simply double-click `index.html` or open it with Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari.

### Option 2: PowerShell Local Server (Windows)
Open PowerShell in the project directory and run:
```powershell
powershell -ExecutionPolicy Bypass -File .\server.ps1
```
Then visit: `http://localhost:8080/`

### Option 3: Python (if installed)
```bash
python -m http.server 8080
```

### Option 4: Node.js / npx (if installed)
```bash
npx serve .
```

---

## 🌐 How to Deploy Online (Free & Instant)

### 1. GitHub Pages
1. Create a new GitHub repository.
2. Push `index.html`, `README.md`, etc. to the `main` branch.
3. Go to **Settings** > **Pages** > Select `main` branch as source > Click **Save**.
4. Your site will be live at `https://<username>.github.io/<repo-name>/`.

### 2. Vercel
1. Install Vercel CLI: `npm i -g vercel` or visit [vercel.com](https://vercel.com).
2. Drag and drop this folder, or run `vercel` in terminal.
3. Instant deployment with automatic HTTPS!

### 3. Netlify
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop the unzipped folder.
3. Deployed in 3 seconds with a live global URL!

---

## 🎓 Academic Attribution
**Data Structures & Algorithms Activity**  
*Zeal College of Engineering and Research, Pune*
