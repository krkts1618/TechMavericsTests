# TechMavericsTests

A complete, professional online examination website for **Node.js — Week 1 Technical Assessment**, built using clean HTML5, CSS3, and vanilla JavaScript in a single, lightweight static architecture.

---

## 📋 Assessment Overview

- **Title:** Node.js — Week 1 Technical Assessment
- **Total Questions:** 40 Multiple-Choice Questions
- **Total Marks:** 100 Marks (2.5 marks per correct answer)
- **Time Limit:** 90 Minutes (5400 seconds) live countdown
- **Pass Threshold:** 60% (60.0 Marks / 24 correct answers)
- **Negative Marking:** None (0.0 marks for incorrect or skipped answers)
- **Question Layout:** 4 options per question (A, B, C, D) with single choice selection

---

## 📚 Curriculum & Section Breakdown

The 40 questions are organized into 5 core technical modules:

1. **Backend and Node.js Fundamentals (Q1–Q8):**
   - V8 JavaScript Engine & JIT machine code compilation
   - Single-threaded event loop architecture & non-blocking I/O
   - `libuv` cross-platform asynchronous I/O and worker thread pool
   - Synchronous vs. asynchronous execution blocking mechanics
   - Call stack LIFO structure and `global` / `globalThis` scope

2. **Node.js Modules and Built-in Modules (Q9–Q15):**
   - CommonJS module specification (`require` and `module.exports`)
   - Module wrapper function parameters: `(exports, require, module, __filename, __dirname)`
   - Built-in `path` module (`path.join()`, `path.resolve()`)
   - Built-in `os` module (`os.cpus()`, platform telemetry)
   - `exports` vs. `module.exports` object binding references
   - Event-driven architecture with `events.EventEmitter`

3. **File System and Asynchronous Programming (Q16–Q23):**
   - Standard Node-style error-first callback convention `(err, data)`
   - Buffer binary streams in `fs.readFile()`
   - Asynchronous file deletion using `fs.unlink()`
   - Production pitfalls of synchronous operations (`fs.readFileSync()`)
   - Non-destructive file writes using `fs.appendFile()`
   - Promise-based asynchronous file I/O (`fs/promises`)
   - Event loop microtask execution order (`process.nextTick()`) and Check phase (`setImmediate()`)

4. **npm and Environment Configuration (Q24–Q30):**
   - Non-interactive project initialization (`npm init -y`)
   - `dependencies` vs. `devDependencies` lifecycle roles
   - Semantic versioning caret (`^`) and tilde (`~`) update ranges
   - Deterministic dependency trees with `package-lock.json`
   - Secure environment variable ingestion with `dotenv` and `process.env`
   - Production security hygiene with `.gitignore`

5. **HTTP and Node.js HTTP Server (Q31–Q40):**
   - Native HTTP server instantiation (`http.createServer()`)
   - Stream abstractions of `req` (Readable) and `res` (Writable)
   - Route and query parsing via `req.url` and request methods
   - Finalizing HTTP streams with `res.end()`
   - Atomic header and status dispatch with `res.writeHead()`
   - HTTP status code conventions (200, 201, 404, 500)
   - Handling chunked POST request streams (`data` and `end` events)
   - Server network binding with `server.listen(port, callback)`
   - MIME type configuration (`Content-Type: application/json`)

---

## ⚡ EmailJS Automated Grading Notifications

This project integrates the official **EmailJS Browser SDK** to automatically dispatch the candidate's graded scorecard to the examiner's configured inbox upon exam completion.

### EmailJS Credentials
- **Public Key:** `mUoANnPLdaqJ-6Frf`
- **Service ID:** `service_8xdq3zc`
- **Template ID:** `template_as501fp`

### Payload Parameters Dispatched:
- `student_name`: Candidate's legal name
- `exam_name`: "Node.js — Week 1 Technical Assessment"
- `total_marks`: "100"
- `score`: Total marks obtained (e.g., `85.0`)
- `percentage`: Percentage score (e.g., `85.0%`)
- `status`: `"PASSED"` or `"FAILED"`
- `correct_answers`: Correct response count
- `incorrect_answers`: Incorrect response count
- `unanswered_questions`: Skipped question count
- `submission_time`: Formatted timestamp
- `topic_breakdown`: Module-by-module performance breakdown
- `message`: Complete plaintext summary for standard email templates

---

## 🚀 Deployment Instructions for Vercel

Because this application is a lightweight, zero-dependency static site consisting of an `index.html` file, it can be deployed to Vercel in seconds with zero build configuration.

### Option A: Deploy via GitHub (Recommended)
1. Push this repository to GitHub:
   ```bash
   git remote add origin https://github.com/krkts1618/TechMavericsTests.git
   git push -u origin main
   ```
2. Go to **[vercel.com](https://vercel.com)** and sign in with GitHub.
3. Click **"Add New..."** > **"Project"**.
4. Select the **`TechMavericsTests`** repository from your GitHub repository list.
5. In the **Configure Project** screen:
   - **Framework Preset:** Leave as `Other` (or static).
   - **Root Directory:** `./`
   - **Build Command:** Leave blank (no build step required).
   - **Output Directory:** Leave blank (or `./`).
6. Click **"Deploy"**.
7. Vercel will instantly generate a live production URL (e.g., `https://nodejs-test.vercel.app`).

### Option B: Deploy via Vercel CLI
1. Install the Vercel CLI globally (if not already installed):
   ```bash
   npm install -g vercel
   ```
2. Navigate to the project directory:
   ```bash
   cd C:\Users\krkts\.gemini\antigravity\scratch\nodejs-exam
   ```
3. Run the deploy command:
   ```bash
   vercel --prod
   ```
4. Follow the interactive CLI prompts to link and deploy your site.

---

## 💻 Local Usage
To view and take the exam locally, open `index.html` in any modern web browser:
```bash
# In Windows PowerShell
Start-Process index.html
```
