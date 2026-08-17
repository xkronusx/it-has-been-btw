# it has been, btw

A single dark-themed page that counts up — years, months, days, hours, minutes, seconds — since **August 1st, 2026**. Pure HTML/CSS/JS, no build step, no dependencies to install.

## Preview

Open `index.html` in any browser and it just works.

## Deploy it as a free GitHub Page

1. Create a new repository on GitHub (public repos get free Pages hosting), e.g. `it-has-been-btw`.
2. Upload `index.html` (and this `README.md` if you like) to the repo — either drag-and-drop on github.com, or via git:
   ```bash
   git init
   git add index.html README.md
   git commit -m "it has been, btw"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, pick `main` and folder `/ (root)`, then **Save**.
6. Wait a minute or two — GitHub will give you a live URL, usually:
   ```
   https://<your-username>.github.io/<your-repo>/
   ```

That's it — no build process, since it's a static file.

## Changing the start date

Edit this line near the bottom of `index.html`:

```js
const START = new Date(2026, 7, 1, 0, 0, 0); // August 1, 2026, 00:00:00 local time
```

Note JavaScript months are zero-indexed, so `7` means August. The clock runs on each visitor's local time zone.
