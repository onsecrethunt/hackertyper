
---

### 6. README.md for **hackertyper.app**

```markdown
# HackerTyper.app

A playful website that simulates hacker-style typing when any key is pressed.

## How it works

JavaScript listens to keydown events and reveals code character by character.

### Demo snippet

```html
<div id="screen" style="font-family: monospace; background: black; color: #0f0; padding: 1rem; height: 200px; overflow-y: auto;"></div>

<script>
const screen = document.getElementById('screen');
const code = "console.log('Hello Hacker!');\nfunction test() { return true; }\n";
let index = 0;

document.addEventListener('keydown', () => {
  if (index < code.length) {
    screen.textContent += code[index++];
    screen.scrollTop = screen.scrollHeight;
  }
});
</script>
