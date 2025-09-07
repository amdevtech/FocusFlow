# 🌀 FocusFlow

**FocusFlow** — A compact productivity web app that combines a **Task Manager**, **Kanban Board**, and the **Pomodoro** technique in a single HTML file (with its embedded JavaScript).

---

## Summary

FocusFlow helps you create and organize tasks, move them through a Kanban board (Not Started → In Progress → Finished), and run Pomodoro focus sessions per task. The app stores state locally (browser) and allows import/export to JSON so you can backup or restore your data.

---

## Screenshot

> Replace the image below with your app screenshot (for GitHub put the file in `/assets` or the repository root).

![FocusFlow screenshot](assets/screenshot.png)

---

## Explanation of use

1. **Add a new task** from the template. It will automatically appear in the Kanban board in the *Not Started* column. You can drag it between the columns (*Not Started – In Progress – Finished*).

2. **Start a Pomodoro session**: select the task from the Kanban and click the **Start Focus** button. The time and duration will be automatically saved when the session ends.

3. **Resilient timer**: If you close the page or refresh, the timer will continue from the last point it stopped — the state is saved locally in the browser.

4. **Import / Export**: Use the **Import** or **Export** button to save all tasks and sessions to a JSON file or restore them later.

5. **Notifications**: The **Activate Notifications** button allows the app to alert you when your focus or rest time is over, even if you are in another tab.

6. **View All**: The **View All** button displays all previous sessions in a separate window with a scrollable table.

---

## How the project is packaged

- The app is implemented as **one HTML file** (e.g. `index.html`) which contains its HTML, CSS, and JavaScript in the same file. This makes deployment trivial — just open the file in any modern browser.

- Data persistence is handled locally (Web Storage). Import/Export uses JSON files.

---

## Usage (Quick start)

1. Clone the repository or download `index.html`.
2. Open `index.html` in your browser.
3. Add tasks, drag them on the Kanban board, and press **Start Focus** to run Pomodoro sessions.
4. Use **Export** to save a `.json` backup and **Import** to restore.

---

## Roadmap

### ✅ Completed tasks
- Single-file web app (HTML + embedded JS).
- Kanban board with drag & drop (Not Started / In Progress / Finished).
- Pomodoro timer per task with session recording.
- Local persistence (browser storage).
- Import / Export (JSON).
- Notifications & "View All" sessions window.

### 🚧 Planned / To-do tasks
- **MySQL integration** — provide an option to sync/save tasks and sessions to a remote MySQL database (server-side endpoint + API). This will allow multi-device syncing and long-term storage.
- **Projects & Clients** — add the ability to group tasks under projects and attach client information to projects.
- **Detailed Reports** — generate exportable reports (CSV / PDF) showing time spent per task, project summaries, and session statistics.
- Optional: authentication, multi-user support, and server-side backups.

---

## File structure (suggested)

```
/ (repo root)
├─ index.html        # single-file app (HTML + CSS + JS)
├─ assets/
│  └─ screenshot.png
├─ data/             # optional: sample JSON backups
└─ README.md
```

---

## Author
**Ahmed Hafez** — FocusFlow

---

## License
Choose an appropriate license (e.g., MIT). Add the license file `LICENSE` to the repo.

---

> _Want me to generate a ready-to-use `index.html` template (single-file) that implements the features above, or export this README as `README.md` in the repository?_

