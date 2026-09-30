# Web Programming - Assignment 2

**Name:** Özcan Öztürk

In this assignment I made one HTML page that looks different with two CSS files.
I used only HTML and CSS, no JavaScript.

## Files

- `index.html` - the page, it has 6 boxes (A, B, C, D, E, F)
- `styleA.css` - Version A (boxes are in a column)
- `styleB.css` - Version B (boxes are in a row, F is in the bottom right)
- `README.md` - this file

The page uses `styleA.css` now. To see Version B, change the link in `index.html`
to `styleB.css`.

## What I did

**Version A:** I used flexbox with `flex-direction: column` and
`justify-content: space-evenly`, so the space between boxes changes when the
window size changes. The boxes are always 100x100 and they never overlap.

**Version B:** I used flexbox for the row and `flex-wrap: nowrap` so the boxes
don't go to the next line. The last box has `position: fixed` so it stays in the
bottom right corner.

## Challenges

- At first the boxes in Version A overlapped when the window was small. I fixed it with
  `min-height` on the body and `flex: none` on the boxes.
- The border made the boxes bigger than 100px. `box-sizing: border-box` fixed this.
- I had to look up how to keep the last box in the corner for Version B, and
  `position: fixed` worked.
