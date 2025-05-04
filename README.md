## What Is Bare-Metal Programming?

Bare-metal programming means writing code that runs *directly on the hardware*—without an operating system, without a scheduler, and often without any abstraction layers.

Unlike Arduino, which provides friendly APIs like `digitalWrite()` or `analogRead()`, bare-metal programming involves talking to the hardware via memory-mapped registers.

```c
#define GPIO_PORT (*(volatile unsigned int*)0x40021018)
GPIO_PORT |= (1 << 5); // Set pin 5 high
```

---

### ✅ **Step 3: Add to Your GitHub Repo**

You now want to put this in your course's GitHub repo, under `Module-1/README.md`.

#### Option A: **Using GitHub Web UI (Easiest)**

1. Go to [github.com](https://github.com)
2. Open your repo
3. Navigate to (or create) the `Module-1` folder
4. Inside it, create a file called `README.md` (if it doesn’t exist)
5. Paste in your Markdown content
6. Scroll down → Add a commit message like:
7. Click **Commit changes**

🎉 Done—your section is now published.

---

### ✅ **Step 4: Add Diagram or Extra Code (Optional)**

If you have an image (e.g., `sfr-map.png`):

1. Go to the `Module-1` folder on GitHub
2. Click **Add file > Upload files**
3. Upload your image (e.g., `sfr-map.png`)
4. Then reference it in your README.md:

```markdown
![SFR Map](./sfr-map.png)

