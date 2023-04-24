# Codequest Browser Extension

Add code snippets to your WhatsApp messages.

![Screenshot](https://raw.githubusercontent.com/Frank-Mayer/codequest.ext/main/screenshot.jpg)

## Use markdown syntax

Write a markdown code block in your message:

<pre><code>```rust
fn main() {
    for x in 1..=100 {
        match (x % 3, x % 5) {
            (0, 0) => println!("FizzBuzz"),
            (0, _) => println!("Fizz"),
            (_, 0) => println!("Buzz"),
            _ => println!("{}", x),
        }
    }
}
```</code></pre>

## Use the CodeQuest Website

Upload your code to [https://codequest.frank-mayer.io](https://codequest.frank-mayer.io) and share a link to the rendered image.

# Install from a store

Chrome: https://chrome.google.com/webstore/detail/codequest/fhibkmjnpghekmolkfpbemmhfiokagdj
Firefox: https://addons.mozilla.org/de/firefox/addon/codequest/

## Build

Using [npm](https://nodejs.org)

### Install dependencies

```bash
npm install
```
### Compile code

```bash
npm run build
```

## Installation

Make sure the extension is build before you install it.

### Chrome

1. At the top right, click `More ⋮` > `More tools` > `Extensions` or go to [`chrome://extensions`](chrome://extensions).
2. Enable `Developer mode` at the top right corner.
3. Click `Load unpacked` at the top left corner.
4. Choose this repository.

### Firefox (temporarily)

1. Go to [`about:debugging#/runtime/this-firefox`](about:debugging#/runtime/this-firefox).
2. Click `Load Temporary Add-on`.
3. Select the `manifest.json` file of this repository.

### Firefox (permanently)

1. Pack the compiled addon into a zip archive or download it from the releases.
2. Go to [`about:addons`](about:addons).
3. Click the :gear: button.
4. Click `Install Add-on From File`.
5. Select the downloaded ZIP.
