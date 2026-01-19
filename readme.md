# Git Hooks – Very Simple

## What is a Git Hook?

A Git hook is a **script that runs automatically** during Git actions (like commit).

---

## Where are Hooks?

```
.git/hooks/
```

---

## Basic Rules

* No file extension
* Must be executable
* Not shared by Git

---

## Simple pre-commit Hook

Go to hooks folder:

```bash
cd .git/hooks
```

Create hook:

```bash
touch pre-commit
```

Add code:

```bash
#!/bin/sh
echo "Pre-commit hook running"
```

Make executable:

```bash
chmod +x pre-commit
```

Now commit → message will appear ✅

---

## Common Hooks

* `pre-commit` – before commit
* `commit-msg` – check message
* `post-commit` – after commit

---

## Disable Hook

```bash
mv pre-commit pre-commit.bak
```

---

