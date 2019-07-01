---
id: tutorial
title: "ಟುಟೋರಿಯಲ್: ರಿಯಾಕ್ಟ್ ಗೆ ಪರಿಚಯ"
layout: tutorial
sectionid: tutorial
permalink: tutorial/tutorial.html
redirect_from:
  - "docs/tutorial.html"
  - "docs/why-react.html"
  - "docs/tutorial-ja-JP.html"
  - "docs/tutorial-ko-KR.html"
  - "docs/tutorial-zh-CN.html"
---


ಊಹೆ: ನಿಮಗೆ ರಿಯಾಕ್ಟ್ ಬಗ್ಗೆ ಮೊದಲಿನ ಜ್ಞಾನ ಅಗತ್ಯವಿಲ್ಲ.
  
## ನಾವು ಟ್ಯುಟೋರಿಯಲ್ ಪ್ರಾರಂಭಿಸುವ ಮೊದಲು {#before-we-start-the-tutorial}


ಈ ಟ್ಯುಟೋರಿಯಲ್ ಸಮಯದಲ್ಲಿ ನಾವು ಒಂದು ಸಣ್ಣ ಆಟವನ್ನು ನಿರ್ಮಿಸುತ್ತೇವೆ. **ನೀವು ಆಟಗಳನ್ನು ನಿರ್ಮಿಸುತ್ತಿಲ್ಲವಾದ್ದರಿಂದ, ನೀವು ಅದನ್ನು ಬಿಟ್ಟುಬಿಡಲು ಬಯಸಬಹುದು -- ಆದರೆ ಇದಕ್ಕೆ ಒಂದು ಅವಕಾಶ ನೀಡಿ.** ನೀವು ಈ ಟ್ಯುಟೋರಿಯಲ್ನಿಂದ ಕಲಿಯುವ ತಂತ್ರಗಳು ಯಾವುದೇ ರಿಯಾಕ್ಟ್ ಅಪ್ಲಿಕೇಶನ್ ನಿರ್ಮಿಸಲು ನಿಮಗೆ ಬಲವಾದ ಮೂಲಭೂತ  ತಿಳುವಳಿಕೆ ನೀಡುತ್ತದೆ.

>ಸಲಹೆ
>
> ಈ ಟ್ಯುಟೋರಿಯಲ್  **ಮಾಡುವ ಮೂಲಕ ಕಲಿಯುವವರಿಗೆ**. ನೀವು ಬೇಸಿಕ್ಸ್ಗಳಿಂದ ಕಲಿಯಲು ಬಯಸಿದರೆ, ನೀವು [ಸ್ಟೆಪ್ ಬೈ ಸ್ಟೆಪ್ ಗೈಡ್](/docs/hello-world.html) ನೋಡಿ. ಈ ಟ್ಯುಟೋರಿಯಲ್ ಮತ್ತು ಗೈಡ್ ಪೂರಕವನ್ನು ನೀವು ಕಾಣಬಹುದು.


ಟ್ಯುಟೋರಿಯಲ್ ಹಲವಾರು ಭಾಗಗಳಾಗಿ ವಿಂಗಡಿಸಲಾಗಿದೆ:


* [ಟ್ಯುಟೋರಿಯಲ್ಗಾಗಿ ಸೆಟಪ್](#setup-for-the-tutorial) ಟ್ಯುಟೋರಿಯಲ್ ಅನ್ನು ಅನುಸರಿಸಲು **ಪ್ರಾರಂಭದ ಬಿಂದುವನ್ನು** ನಿಮಗೆ ನೀಡುತ್ತದೆ.
* [ಅವಲೋಕನ (ಓವರ್ವ್ಯೂ)](#overview) ನಿಮಗೆ ರಿಯಾಕ್ಟ್ **ಮೂಲಭೂತ** ಶಿಕ್ಷಣವನ್ನು ನೀಡುತ್ತದೆ:  ಕಾಂಪೊನೆಂಟ್ಸ್, ಪ್ರಾಪ್ಸ್, ಮತ್ತು  ಸ್ಟೇಟ್.
* [ನೀವು ಆಟ ಮುಗಿಸಿದರೆ](#completing-the-game), "ರಿಯಾಕ್ಟ್"ಲ್ಲಿರುವ ಎಲ್ಲಾ ತಂತ್ರಗಳು ಕಲಿಯುವಿರಿ
* [ಸಮಯ ಪ್ರಯಾಣವನ್ನು ಸೇರಿಸುವುದು](#adding-time-travel) (ಇದು ಕೊನೆಯ ಅಭ್ಯಾಸ),  ನಿಮಗೆ "ರಿಯಾಕ್ಟ್"ಲ್ಲಿರುವ ಅನನ್ಯ ಸಾಮರ್ಥ್ಯದ **ಆಳವಾದ ಒಳನೋಟ(ಇನ್ಸೈಟ್)** ಸಸಿಗುತ್ತದೆ.


ಈ ಟ್ಯುಟೋರಿಯಲ್ನ ಮೌಲ್ಯವನ್ನು ಪಡೆಯಲು ನೀವು ಎಲ್ಲಾ ವಿಭಾಗಗಳನ್ನು ಏಕಕಾಲದಲ್ಲಿ ಪೂರ್ಣಗೊಳಿಸಬೇಕಾಗಿಲ್ಲ. ನೀವು ಸಾಧ್ಯವಾದಷ್ಟು ಪ್ರಯತ್ನಿಸಿ -- ಒಂದು ಅಥವಾ ಎರಡು ವಿಭಾಗಗಳಿದ್ದರೂ ಸಹ, ನೀವು ಅದರ ಉಪಯೋಗ ಕಾಣುತ್ತೀರಿ.

### ನಾವು ಏನು ನಿರ್ಮಿಸಲು ಪ್ರಯತ್ನಿಸುತ್ತಿದ್ದೇವೆ? {#what-are-we-building}

ಈ ಟ್ಯುಟೋರಿಯಲ್ ನಲ್ಲಿ, ನಾವು ನಿಮಗೆ ರಿಯಾಕ್ಟ್ ಮೂಲಕ "ಟಿಕ್-ಟಾಕ್-ಟೊ" ಆಟ ಹೇಗೆ ಮಾಡುವುದೆ೦ದು ತೋರಿಸುತ್ತೇವೆ.

ನಾವು ಇಲ್ಲಿ ಏನು ಮಾಡುತ್ತಿದ್ದೇವೆಂದು ನೀವು ನೋಡಬಹುದು: **[ಫೈನಲ್  ರಿಸಲ್ಟ್ ](https://codepen.io/gaearon/pen/gWWZgR?editors=0010)**. ಕೋಡ್ ನಿಮಗೆ ಅರ್ಥವಾಗುತ್ತಿಲ್ಲ, ಅಥವಾ, ಕೋಡ್ ಸಿಂಟ್ಯಾಕ್ಸ್ ಅರ್ಥವಾಗುತ್ತಿಲ್ಲ, ಚಿಂತಿಸಬೇಡಿ! ಈ ಟ್ಯುಟೋರಿಯಲ್ ಗುರಿ ನಿಮಗೆ ಕೋಡ್ ಮತ್ತು ಸಿಂಟ್ಯಾಕ್ಸ್ ನಿಮಗೆ ಅರ್ಥಮಾಡಿಕೊಳ್ಳಲು ಸಹಾಯ ಮಾಡುತ್ತದೆ.

ನಮ್ಮ ಶಿಫಾರಸು - ನೀವು ಟ್ಯುಟೋರಿಯಲ್ ಅನ್ನು ಮುಂದುವರಿಸುವ ಮೊದಲು ಒಮ್ಮೆ ನೀವು ಟಿಕ್-ಟಾಕ್-ಟೋ ಕೋಡ್ ನೋಡಿ.


ಈ ಆಟದಲ್ಲಿ ಹಲವಾರು ವೈಶಿಷ್ಟ್ಯಗಳಿವೆ, ಅವುಗಳಲ್ಲಿ ಒಂದು, ಗೇಮ್ ಬೋರ್ಡಿನ ಬಲಭಾಗದಲ್ಲಿ ಸಂಖ್ಯೆಯ ಪಟ್ಟಿ ಇದೆ. ಈ ಪಟ್ಟಿಯಲ್ಲಿ ನೀವು ಆಟದ ಎಲ್ಲಾ ಚಲನೆಗಳ ಇತಿಹಾಸವನ್ನು ನೀಡುತ್ತದೆ, ಮತ್ತು ಆಟದ ಮುಂದುವರೆದಂತೆ ಅದನ್ನು ನವೀಕರಿಸಲಾಗುತ್ತದೆ.


ನಿಮಗೆ ತಿಳಿದಿರುವ ನಂತರ ನೀವು ಟಿಕ್-ಟಾಕ್-ಟೋ ಆಟವನ್ನು ಮುಚ್ಚಬಹುದು. ಈ ಟ್ಯುಟೋರಿಯಲ್ನಲ್ಲಿ ನಾವು ಸರಳ ಟೆಂಪ್ಲೆಟ್ನಿಂದ ಪ್ರಾರಂಭಿಸುತ್ತೇವೆ. ನಮ್ಮ ಮುಂದಿನ ಹಂತವು ನಿಮ್ಮನ್ನು ಸ್ಥಾಪಿಸುವ ಮೂಲಕ ನೀವು ಆಟವನ್ನು ನಿರ್ಮಿಸಲು ಪ್ರಾರಂಭಿಸಬಹುದು.

### ಪೂರ್ವಾಪೇಕ್ಷಿತಗಳು (ಪ್ರೇರೆಕ್ಕ್ಇಸಿಟಿಎಸ್) {#prerequisites}

ಎಚ್ಟಿಎಮ್ಎಲ್(HTML) ಮತ್ತು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್(JavaScript) ಗೆ ನಿಮಗೆ ಪರಿಚಯವಿದೆ ಎಂದು ನಾವು ಭಾವಿಸುತ್ತೇವೆ, ಆದರೆ ನೀವು ಬೇರೊಂದು ಪ್ರೋಗ್ರಾಮಿಂಗ್ ಭಾಷೆಯಿಂದ ಬಂದರೂ ಸಹ ನೀವು ಅನುಸರಿಸಲು ಸಾಧ್ಯವಾಗುತ್ತದೆ. ನೀವು ಪ್ರೋಗ್ರಾಮಿಂಗ್ ಪರಿಕಲ್ಪನೆಗಳಾದ ಫುನ್ಕ್ಷನ್ಸ್(Functions), ಒಬ್ಜೆಕ್ಟ್ಸ್(Objects), ಅರ್ರಯ್ಸ್(Arrays) ಮತ್ತು ಸ್ವಲ್ಪ ಮಟ್ಟಿಗೆ  ಕ್ಲಾಸೆಸ್(Classes) ತಿಳಿದಿರುವಿರಿ ಎಂದು ನಾವು ಭಾವಿಸುತ್ತೇವೆ.

ನೀವು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ರಿಫ್ರೆಶ್ ಮಾಡಬೇಕಾದರೆ, ನಾವು [ಈ ಗೈಡ್](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) ಓದಲು ಶಿಫಾರಸು ಮಾಡುತ್ತೇವೆ. ನಾವು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ನ ಇತ್ತೀಚಿನ ಆವೃತ್ತಿಯನ್ನು ES6 ನಿಂದ ಕೆಲವು ವೈಶಿಷ್ಟ್ಯಗಳನ್ನು ಬಳಸಿತೇವೆ ಎಂಬುದನ್ನು ಗಮನಿಸಿ. ಈ ಟ್ಯುಟೋರಿಯಲ್ ನಲ್ಲಿ, ನಾವು ಬಳಸುತ್ತಿದ್ದೇವೆ [ಆರೋ ಫುನ್ಕ್ಷನ್ಸ್](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions), [ಕ್ಲಾಸೆಸ್](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes), [`ಲೆಟ್`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let), ಮತ್ತು [`ಕಾಂಸ್ಟ್`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const) ಸ್ಟೇಟಮೆಂಟ್ಸ್. ನೀವು [ಬಾಬೆಲ್ ರೆಪ್ಲ್](babel://es5-syntax-example) ಬಳಿಸಿ ಯಾವ ES6 ಕೋಡ್ ಜೊತೆ ಕಂಪೈಲ್ ಹಾಗುವುದೆಂದು ನೋಡಬಹುದು.

## ಟ್ಯುಟೋರಿಯಲ್ಗಾಗಿ ಸೆಟಪ್ {#setup-for-the-tutorial}

ಈ ಟ್ಯುಟೋರಿಯಲ್ ಪೂರ್ಣಗೊಳಿಸಲು ಎರಡು ಮಾರ್ಗಗಳಿವೆ: ನೀವು ನಿಮ್ಮ ಬ್ರೌಸರ್ನಲ್ಲಿ ಕೋಡ್ ಅನ್ನು ಬರೆಯಬಹುದು, ಅಥವಾ ನೀವು ನಿಮ್ಮ ಕಂಪ್ಯೂಟರ್ನಲ್ಲಿ ಲೋಕಲ್ ಡೆವಲಪ್ಮೆಂಟ್ ಸೆಟಪ್ ಮಾಡಬಹುದು

### ಸೆಟಪ್ ಮಾರ್ಗ ಒಂದು: ಬ್ರೌಸರ್ನಲ್ಲಿ ಕೋಡ್ ಅನ್ನು ಬರೆಯಬಹುದು {#setup-option-1-write-code-in-the-browser}

ಪ್ರಾರಂಭಿಸಲು ಇದು ತ್ವರಿತ ಮಾರ್ಗ!

ಮೊದಲು, ಇದನ್ನು  ಹೊಸ ಟ್ಯಾಬ್ನಲ್ಲಿ ತೆರೆಯಿರಿ **[ಸ್ಟಾರ್ಟರ್ ಕೋಡ್](https://codepen.io/gaearon/pen/oWWQNa?editors=0010)**. ಹೊಸ ಟ್ಯಾಬ್ ಖಾಲಿ "ಟಿಕ್-ಟಾಕ್-ಟೋ" ಗೇಮ್ ಬೋರ್ಡ್ ಮತ್ತು ರಿಯಾಕ್ಟ್ ಕೋಡ್ ಅನ್ನು ತೋರಿಸುತ್ತದೆ. ಈ ಟ್ಯುಟೋರಿಯಲ್ ನಲ್ಲಿ ನಾವು ರಿಯಾಕ್ಟ್ ಕೋಡ್ ಅನ್ನು ಸಂಪಾದಿಸುತ್ತೇವೆ (ಎಡಿಟ್ ಮಾಡುವುದು).

ನೀವು ಈಗ ಎರಡನೇ ಸೆಟಪ್ ಆಯ್ಕೆಯನ್ನು ಬಿಟ್ಟುಬಿಡಬಹುದು ಮತ್ತು ಪ್ರತಿಕ್ರಿಯೆಯ [ಅವಲೋಕನ (ಓವರ್ವ್ಯೂ)](#overview) ವಿಭಾಗಕ್ಕೆ ಹೋಗಬಹುದು.

### ಸೆಟಪ್ ಮಾರ್ಗ ಎರಡು: ಲೋಕಲ್ ಡೆವಲಪ್ಮೆಂಟ್ ಎನ್ವಿರಾನ್ಮೆಂಟ್ {#setup-option-2-local-development-environment}

ಈ ಟ್ಯುಟೋರಿಯಲ್ಗೆ ಇದು ಸಂಪೂರ್ಣವಾಗಿ ಐಚ್ಛಿಕವಾಗಿರುತ್ತದೆ ಮತ್ತು ಅಗತ್ಯವಿಲ್ಲ!

<br>

<details>

<summary><b>ಐಚ್ಛಿಕ: ನಿಮ್ಮ ಆದ್ಯತೆಯ ಲೋಕಲ್ ಟೆಕ್ಸ್ಟ್ ಎಡಿಟರ್ ಬಳೆಸುವುದಕೆ ಸೂಚನೆಗಳು</b></summary>


ಈ ಸೆಟಪ್ಗೆ ಹೆಚ್ಚಿನ ಕೆಲಸ ಬೇಕಾಗುತ್ತದೆ ಆದರೆ ನಿಮ್ಮ ಆಯ್ಕೆಯ ಟೆಕ್ಸ್ಟ್ ಎಡಿಟರ್ ಬಳಸಿಕೊಂಡು ಟ್ಯುಟೋರಿಯಲ್ ಅನ್ನು ಪೂರ್ಣಗೊಳಿಸಬಹುದು. ಅನುಸರಿಸಲು ಹಂತಗಳು ಇಲ್ಲಿವೆ:

1. ನೀವು "nodejs" ನ ಇತ್ತೀಚಿನ ಆವೃತ್ತಿಯನ್ನು(ವರ್ಷನ್) ಹೊಂದಿರುವಿರಾ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ [Node.js](https://nodejs.org/en/).

2. ಇಲ್ಲಿ ನೀಡಿರುವ ರ [ಿಯಾಕ್ಟ್ ಅಪ್ಲಿಕೇಶನ್ ಇನ್ಸ್ಟಾಲೇಷನ್ ಸೂಚನೆಗಳನ್ನು](/docs/create-a-new-react-app.html#create-react-app)  ಪಾಲಿಸಿದರೆ, ಒಂದು ಹೊಸ ಪ್ರಾಜೆಕ್ಟ್ ರಚಿಸಲಾಗುವುದು.

```bash
npx create-react-app my-app
```

3. ಹೊಸ ಪ್ರಾಜೆಕ್ಟ್ನ `src/` ಫೋಲ್ಡರ್ನಲ್ಲಿ ಎಲ್ಲಾ ಫೈಲ್ಗಳನ್ನು ಅಳಿಸಿ. 

> ಸೂಚನೆ:
>
>**ಸಂಪೂರ್ಣ `src` ಫೋಲ್ಡರ್ ಅಳಿಸಬೇಡಿ, ಅದರೊಳಗೆ ಮೂಲ ಮೂಲ ಫೈಲ್ಗಳು ಮಾತ್ರ.** ಮುಂದಿನ ಹಂತದಲ್ಲಿ ಪ್ರಾಜೆಕ್ಟ್ನ ಡೀಫಾಲ್ಟ್ ಫೈಲ್ಗಳನ್ನು ಉದಾಹರಣೆಗೆ ಫೈಲ್ಗಳೊಂದಿಗೆ ಬದಲಾಯಿಸಲಾಗುತ್ತದೆ.

```bash
cd my-app
cd src

# ನೀವು ಮ್ಯಾಕ್ ಅಥವಾ ಲಿನಕ್ಸ್ ಅನ್ನು ಬಳಸುತ್ತಿದ್ದರೆ:
rm -f *

# ಅಥವಾ, ನೀವು Windows ನಲ್ಲಿದ್ದರೆ:
del *

# ನಂತರ, ಯೋಜನೆಯ ಫೋಲ್ಡರ್ಗೆ ಹಿಂತಿರುಗಿ
cd ..
```

4. `index.css` ಎ೦ಬ ಫೈಲ್ ಮಾಡಿ [ಈ ಸಿಎಸ್ಎಸ್ ಕೋಡ್](https://codepen.io/gaearon/pen/oWWQNa?editors=0100) ನಕಲು ಅಂಟಿಸಿ `src/` ಫೋಲ್ಡರ್ನಲ್ಲಿ ಇಟ್ಟುಕೊಳ್ಳಿ.

5. `index.js` ಎ೦ಬ ಫೈಲ್ ಮಾಡಿ [ಈ ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಕೋಡ್](https://codepen.io/gaearon/pen/oWWQNa?editors=0100) ನಕಲು ಅಂಟಿಸಿ `src/` ಫೋಲ್ಡರ್ನಲ್ಲಿ ಇಟ್ಟುಕೊಳ್ಳಿ.

6. `src/` ಫೋಲ್ಡರ್ನಲ್ಲಿರುವ `index.js` ಫೈಲಿನಲ್ಲಿ ಈ ಮೂರು ಸಾಲುಗಳನ್ನು ೇಲ್ಭಾಗಕ್ಕೆ ಸೇರಿಸಿ.

```js
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
```

ಈಗ ನೀವು ಪ್ರಾಜೆಕ್ಟ್ ಫೋಲ್ಡೆರ್ನಲ್ಲಿದು, `npm start`ಕಮಾಂಡ್ ಕೊಟ್ಟಾದಮೇಲೆ, ನಿಮ್ಮ ಬ್ರೌಸರ್ನಲ್ಲಿ `http://localhost:3000` ಎಂದು ಟೈಪ್ ಮಾಡಿಧರೆ, ನೀವು "ಟಿಕ್-ಟಾಕ್-ಟೋ" ಆಟದ ಖಾಲಿ ಬೋರ್ಡ್ ನೋಡುತ್ತೀರಿ.
 
[ಈ ಸೂಚನೆಗಳನ್ನು] (https://babeljs.io/docs/editors/) ಅನುಸರಿಸಿಸಲು ನಾವು ಶಿಫಾರಸು ಮಾಡುತ್ತೇವೆ. ಇದರೊಂದಿಗೆ ನಿಮ್ಮ ಎಡಿಟರ್ ಸಿಂಟ್ಯಾಕ್ಸ್ ಹೈಲೈಟ್ ಅನ್ನು ಸಂರಚಿಸಲು (ಕಾನ್ಫಿಗರ್) ಆಗುವುದು.

</details>

### ಸಹಾಯ, ನಾನು ಮುಂದುವರೆಯಲು ಸಾಧ್ಯವಾಗುತಿಲ್ಲ! {#help-im-stuck}

ನಿಮಗೆ ಮುಂದೂಡಲು ಸಾಧ್ಯವಾಗುತಿಲ್ಲವೆಂದರೆ, [ಕಮ್ಯೂನಿಟಿ ಸಪೋರ್ಟ್ ರಿಸೋರ್ಸಸ್](/community/support.html) ನಲ್ಲಿ ನಿಮಗೆ ಸಹಾಯ ಸಿಗುತ್ತದೆ. ನಿರ್ದಿಷ್ಟವಾಗಿ, [ರಿಯಾಕ್ಟ್ ಫ್ಲಕ್ಸ್ ಚಾಟ್](https://discord.gg/0ZcbPKXt5bZjGY5n) ನಲ್ಲಿ ನೀವು ಶೀಘ್ರ ಸಹಾಯ ಪಡೆಯುತ್ತೀರಿ. ನೀವು ಉತ್ತರವನ್ನು ಸಿಗದಿದ್ದರೆ, ಅಥವಾ ನಿಮಗೆ ಮುಂದೂಡಲು ಸಾಧ್ಯವಾಗದಿದ್ದರೆ, ದಯವಿಟ್ಟು ಸಮಸ್ಯೆಯನ್ನು (ಇಶ್ಯೂ) ಫೈಲ್ ಮಾಡಿ, ಮತ್ತು ನಾವು ನಿಮಗೆ ಸಹಾಯ ಮಾಡುತ್ತೇವೆ.

## ಅವಲೋಕನ (ಓವರ್ವ್ಯೂ) {#overview}

ಈಗ ಸೆಟಪ್ಆಗಿರುವುದರಿಂದ, ಮುಂದೆ ನಾವು ಈಗ ರಿಯಾಕ್ಟ್ ಎಂದರೇನು ಅಂತ ನೋಡೋಣ (ಓವರ್ವ್ಯೂ)

### ರಿಯಾಕ್ಟ್ ಎಂದರೇನು? {#what-is-react}

ರಿಯಾಕ್ಟ್ ಒಂದು ಘೋಷಣಾತ್ಮಕ (ಡೆಕ್ಲಾರಟಿವೆ), ಸಮರ್ಥ, and ಹೊಂದಿಕೊಳ್ಳುವ (ಫ್ಲೆಕ್ಸಿಬಲ್) ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಲೈಬ್ರರಿ. ಇದು ಬಳಕೆದಾರ ಅಥವಾ ಉಪಯೋಗಿಸುವವನು (ಯೂಸರ್) ಇಂಟರ್ಫೇಸ್ಗಳನ್ನು (ಯು ಐ ಇಂಟರ್ಫೇಸ್) ತಯಾರಿಸಲು ಬಳಸಲಾಗುತ್ತದೆ. 
<br>
ಸಂಕೀರ್ಣ ಯುಐಗಳನ್ನು "ಘಟಕಗಳು"(ಕಾಂಪೊನೆಂಟ್ಸ್) ಎಂಬ ಸಣ್ಣ ಮತ್ತು ಪ್ರತ್ಯೇಕವಾದ ತುಣುಕುಗಳಿಂದ ಸಂಯೋಜಿಸಲು ಇದರಿ೦ದ ಸಾಧ್ಯ.


ಪ್ರತಿಕ್ರಿಯೆಯು ಕೆಲವು ವಿಭಿನ್ನ ರೀತಿಯ ಅಂಶಗಳನ್ನು ಹೊಂದಿದೆ, ಆದರೆ ನಾವು `ರಿಯಾಕ್ಟ್.ಕಂಪೋನೆಂಟ್` ಉಪವರ್ಗಗಳೊಂದಿಗೆ ಪ್ರಾರಂಭಿಸುತ್ತೇವೆ:

```javascript
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}

// Example usage: <ShoppingList name="Mark" />
```

ನಾವು ಶೀಘ್ರದಲ್ಲೇ XML- ನಂತಹ ಟ್ಯಾಗ್ಗಳ ಬಗ್ಗೆ ಮಾತನಾಡುತ್ತೇವೆ. ನಾವು ಕಾಂಪೊನೆಂಟ್ಸ್ ಮೂಲಕ ರಿಯಾಕ್ಟ್ ಗೆ ಸ್ಕ್ರೀನ್ ಮೇಲೆ ಏನು ನೋಡಬೇಕೆಂದು ಹೇಳುತ್ತೆವೆ. ನಮ್ಮ ಡೇಟಾ ಬದಲಾದರೆ, ರಿಯಾಕ್ಟ್, ನಮ್ಮ ಘಟಕಗಳನ್ನು (ಕಾಂಪೊನೆಂಟ್ಸ್) ಪರಿಣಾಮಕಾರಿಯಾಗಿ ನವೀಕರಿಸಿ ಮರು-ನಿರೂಪಿಸುತ್ತದೆ.

ಇಲ್ಲಿ, ShoppingList ಒಂದು **ರಿಯಾಕ್ಟ್ ಕಂಪೋನೆಂಟ್ ಕ್ಲಾಸ್**, ಅಥವಾ **ರಿಯಾಕ್ಟ್ ಕಂಪೋನೆಂಟ್ ಟೈಪ್**. ಒಂದು ಕಂಪೋನೆಂಟ್ ಹಲವಾರು ನಿಯತಾಂಕಗಳು (ಪಾರಮೇಟರ್ಸ್) ತೆಗೆದುಕೊಳ್ಳುತದೆ. ಇದನ್ನು  `ಪ್ರಾಪ್ಸ್`(`props`) ("ಪ್ರಾಪರ್ಟೀಸ್" ಶಬ್ದದ ಸಣ್ಣ ರೂಪ) ಎಂದು ಕರೆಯಲಾಗುತ್ತದೆ,  ಮತ್ತು `render`(ರಂಡೆರ್) ಮೆಥಡ್ ಮೂಲಕ ಪ್ರದರ್ಶಿಸಲು ವೀಕ್ಷಣೆಗಳ ಕ್ರಮಾನುಗತವನ್ನು ಹಿಂದಿರುಗಿಸುತ್ತದೆ.


ರಿಯಾಕ್ಟ್ `render (ರೆಂಡೆರ್)` ಮೆಥಡ್ ಸ್ಕ್ರೀನ್ ಮೇಲೆ ನೀವು ನೋಡಲು ಬಯಸುವ * ವಿವರಣೆಯನ್ನು * ಹಿಂದಿರುಗಿಸುತ್ತದೆ. ರಿಯಾಕ್ಟ್ ವಿವರಣೆಯನ್ನು ತೆಗೆದುಕೊಳ್ಳುತ್ತದೆ ಮತ್ತು ಫಲಿತಾಂಶವನ್ನು ಪ್ರದರ್ಶಿಸುತ್ತದೆ. ನಿರ್ದಿಷ್ಟವಾಗಿ, `ರೆಂಡರ್` ರಿಟರ್ನ್ಸ್ ** ರಿಯಾಕ್ಟ್ ಎಲಿಮೆಂಟ್ **, ಅದು ಏನು ನಿರೂಪಿಸಲು ಒಂದು ಹಗುರವಾದ ವಿವರಣೆಯಾಗಿದೆ. ಹೆಚ್ಚಿನ ರಿಯಾಕ್ಟ್ ಡೆವೆಲೊಫೇರ್ಸ್ "JSX" ಎಂಬ ವಿಶೇಷ ಸಿಂಟ್ಯಾಕ್ಸ್ ಅನ್ನು ಬಳಸುತ್ತಾರೆ, ಅದು ಈ ರಚನೆಗಳನ್ನು ಬರೆಯಲು ಸುಲಭವಾಗುತ್ತದೆ. `<Div />` ಸಿಂಟ್ಯಾಕ್ಸ್ ಅನ್ನು 'ರಿಯಾಕ್ಟ್.ಕ್ರೀಟ್ ಎಲಿಮೆಂಟ್' ('ಡಿವಿ') `ಗೆ ಬಿಲ್ಡ್ ಸಮಯದಲ್ಲಿ ಬದಲಾಯಿಸಲಾಗುತ್ತದೆ. ಮೇಲಿನ ಉದಾಹರಣೆಯು ಇದಕ್ಕೆ ಸಮನಾಗಿರುತ್ತದೆ:

```javascript
return React.createElement('div', {className: 'shopping-list'},
  React.createElement('h1', /* ... h1 children ... */),
  React.createElement('ul', /* ... ul children ... */)
);
```

[ಪೂರ್ಣ ವಿಸ್ತರಿತ ಆವೃತ್ತಿಯನ್ನು ನೋಡಿ.](babel://tutorial-expanded-version)

ನೀವು ಕುತೂಹಲಕಾರಿಯಾಗಿದ್ದರೆ `createElement()` ಇಲ್ಲಿ, [API reference](/docs/react-api.html#createelement), ಹೆಚ್ಚು ವಿವರವಾಗಿ ವಿವರಿಸಲಾಗಿದೆ. ಆದರೆ ನಾವು ಈ ಟ್ಯುಟೋರಿಯಲ್ನಲ್ಲಿ ಅದನ್ನು ಬಳಸುವುದಿಲ್ಲ. ಬದಲಾಗಿ, ನಾವು JSX ಅನ್ನು ಬಳಸುತ್ತೇವೆ.

JSX ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ನ ಪೂರ್ಣ ಶಕ್ತಿಯೊಂದಿಗೆ ಬರುತ್ತದೆ. ನೀವು JSX ಒಳಗೆ ಕಟ್ಟುಪಟ್ಟಿಗಳಲ್ಲಿ ಯಾವುದೇ ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಅಭಿವ್ಯಕ್ತಿಗಳನ್ನು ಹಾಕಬಹುದು. ಪ್ರತಿ ಪ್ರತಿಕ್ರಿಯಾ ಅಂಶವು ಒಂದು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ವಸ್ತುವೆಂದರೆ ನೀವು ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಂನಲ್ಲಿ ವೇರಿಯೇಬಲ್ ಅಥವಾ ಪಾಸ್ನಲ್ಲಿ ಸಂಗ್ರಹಿಸಬಹುದು.

The `ShoppingList` component above only renders built-in DOM components like `<div />` and `<li />`. But you can compose and render custom React components too. For example, we can now refer to the whole shopping list by writing `<ShoppingList />`. Each React component is encapsulated and can operate independently; this allows you to build complex UIs from simple components.

## Inspecting the Starter Code {#inspecting-the-starter-code}

If you're going to work on the tutorial **in your browser,** open this code in a new tab: **[Starter Code](https://codepen.io/gaearon/pen/oWWQNa?editors=0010)**. If you're going to work on the tutorial **locally,** instead open `src/index.js` in your project folder (you have already touched this file during the [setup](#setup-option-2-local-development-environment)).

This Starter Code is the base of what we're building. We've provided the CSS styling so that you only need to focus on learning React and programming the tic-tac-toe game.

By inspecting the code, you'll notice that we have three React components:

* Square
* Board
* Game

The Square component renders a single `<button>` and the Board renders 9 squares. The Game component renders a board with placeholder values which we'll modify later. There are currently no interactive components.

### Passing Data Through Props {#passing-data-through-props}

To get our feet wet, let's try passing some data from our Board component to our Square component.

We strongly recommend typing code by hand as you're working through the tutorial and not using copy/paste. This will help you develop muscle memory and a stronger understanding.

In Board's `renderSquare` method, change the code to pass a prop called `value` to the Square:

```js{3}
class Board extends React.Component {
  renderSquare(i) {
    return <Square value={i} />;
  }
```

Change Square's `render` method to show that value by replacing `{/* TODO */}` with `{this.props.value}`:

```js{5}
class Square extends React.Component {
  render() {
    return (
      <button className="square">
        {this.props.value}
      </button>
    );
  }
}
```

Before:

![React Devtools](../images/tutorial/tictac-empty.png)

After: You should see a number in each square in the rendered output.

![React Devtools](../images/tutorial/tictac-numbers.png)

**[View the full code at this point](https://codepen.io/gaearon/pen/aWWQOG?editors=0010)**

Congratulations! You've just "passed a prop" from a parent Board component to a child Square component. Passing props is how information flows in React apps, from parents to children.

### Making an Interactive Component {#making-an-interactive-component}

Let's fill the Square component with an "X" when we click it.
First, change the button tag that is returned from the Square component's `render()` function to this:

```javascript{4}
class Square extends React.Component {
  render() {
    return (
      <button className="square" onClick={function() { alert('click'); }}>
        {this.props.value}
      </button>
    );
  }
}
```

If you click on a Square now, you should see an alert in your browser.

>Note
>
>To save typing and avoid the [confusing behavior of `this`](https://yehudakatz.com/2011/08/11/understanding-javascript-function-invocation-and-this/), we will use the [arrow function syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) for event handlers here and further below:
>
>```javascript{4}
>class Square extends React.Component {
>  render() {
>    return (
>      <button className="square" onClick={() => alert('click')}>
>        {this.props.value}
>      </button>
>    );
>  }
>}
>```
>
>Notice how with `onClick={() => alert('click')}`, we're passing *a function* as the `onClick` prop. React will only call this function after a click. Forgetting `() =>` and writing `onClick={alert('click')}` is a common mistake, and would fire the alert every time the component re-renders.

As a next step, we want the Square component to "remember" that it got clicked, and fill it with an "X" mark. To "remember" things, components use **state**.

React components can have state by setting `this.state` in their constructors. `this.state` should be considered as private to a React component that it's defined in. Let's store the current value of the Square in `this.state`, and change it when the Square is clicked.

First, we'll add a constructor to the class to initialize the state:

```javascript{2-7}
class Square extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      value: null,
    };
  }

  render() {
    return (
      <button className="square" onClick={() => alert('click')}>
        {this.props.value}
      </button>
    );
  }
}
```

>Note
>
>In [JavaScript classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes), you need to always call `super` when defining the constructor of a subclass. All React component classes that have a `constructor` should start it with a `super(props)` call.

Now we'll change the Square's `render` method to display the current state's value when clicked:

* Replace `this.props.value` with `this.state.value` inside the `<button>` tag.
* Replace the `onClick={...}` event handler with `onClick={() => this.setState({value: 'X'})}`.
* Put the `className` and `onClick` props on separate lines for better readability.

After these changes, the `<button>` tag that is returned by the Square's `render` method looks like this:

```javascript{12-13,15}
class Square extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      value: null,
    };
  }

  render() {
    return (
      <button
        className="square"
        onClick={() => this.setState({value: 'X'})}
      >
        {this.state.value}
      </button>
    );
  }
}
```

By calling `this.setState` from an `onClick` handler in the Square's `render` method, we tell React to re-render that Square whenever its `<button>` is clicked. After the update, the Square's `this.state.value` will be `'X'`, so we'll see the `X` on the game board. If you click on any Square, an `X` should show up.

When you call `setState` in a component, React automatically updates the child components inside of it too.

**[View the full code at this point](https://codepen.io/gaearon/pen/VbbVLg?editors=0010)**

### Developer Tools {#developer-tools}

The React Devtools extension for [Chrome](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/) lets you inspect a React component tree with your browser's developer tools.

<img src="../images/tutorial/devtools.png" alt="React Devtools" style="max-width: 100%">

The React DevTools let you check the props and the state of your React components.

After installing React DevTools, you can right-click on any element on the page, click "Inspect" to open the developer tools, and the React tab will appear as the last tab to the right.

**However, note there are a few extra steps to get it working with CodePen:**

1. Log in or register and confirm your email (required to prevent spam).
2. Click the "Fork" button.
3. Click "Change View" and then choose "Debug mode".
4. In the new tab that opens, the devtools should now have a React tab.

## Completing the Game {#completing-the-game}

We now have the basic building blocks for our tic-tac-toe game. To have a complete game, we now need to alternate placing "X"s and "O"s on the board, and we need a way to determine a winner.

### Lifting State Up {#lifting-state-up}

Currently, each Square component maintains the game's state. To check for a winner, we'll maintain the value of each of the 9 squares in one location.

We may think that Board should just ask each Square for the Square's state. Although this approach is possible in React, we discourage it because the code becomes difficult to understand, susceptible to bugs, and hard to refactor. Instead, the best approach is to store the game's state in the parent Board component instead of in each Square. The Board component can tell each Square what to display by passing a prop, [just like we did when we passed a number to each Square](#passing-data-through-props).

**To collect data from multiple children, or to have two child components communicate with each other, you need to declare the shared state in their parent component instead. The parent component can pass the state back down to the children by using props; this keeps the child components in sync with each other and with the parent component.**

Lifting state into a parent component is common when React components are refactored -- let's take this opportunity to try it out.

Add a constructor to the Board and set the Board's initial state to contain an array of 9 nulls corresponding to the 9 squares:

```javascript{2-7}
class Board extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      squares: Array(9).fill(null),
    };
  }

  renderSquare(i) {
    return <Square value={i} />;
  }
```

When we fill the board in later, the `this.state.squares` array will look something like this:

```javascript
[
  'O', null, 'X',
  'X', 'X', 'O',
  'O', null, null,
]
```

The Board's `renderSquare` method currently looks like this:

```javascript
  renderSquare(i) {
    return <Square value={i} />;
  }
```

In the beginning, we [passed the `value` prop down](#passing-data-through-props) from the Board to show numbers from 0 to 8 in every Square. In a different previous step, we replaced the numbers with an "X" mark [determined by Square's own state](#making-an-interactive-component). This is why Square currently ignores the `value` prop passed to it by the Board.

We will now use the prop passing mechanism again. We will modify the Board to instruct each individual Square about its current value (`'X'`, `'O'`, or `null`). We have already defined the `squares` array in the Board's constructor, and we will modify the Board's `renderSquare` method to read from it:

```javascript{2}
  renderSquare(i) {
    return <Square value={this.state.squares[i]} />;
  }
```

**[View the full code at this point](https://codepen.io/gaearon/pen/gWWQPY?editors=0010)**

Each Square will now receive a `value` prop that will either be `'X'`, `'O'`, or `null` for empty squares.

Next, we need to change what happens when a Square is clicked. The Board component now maintains which squares are filled. We need to create a way for the Square to update the Board's state. Since state is considered to be private to a component that defines it, we cannot update the Board's state directly from Square.

Instead, we'll pass down a function from the Board to the Square, and we'll have Square call that function when a square is clicked. We'll change the `renderSquare` method in Board to:

```javascript{5}
  renderSquare(i) {
    return (
      <Square
        value={this.state.squares[i]}
        onClick={() => this.handleClick(i)}
      />
    );
  }
```

>Note
>
>We split the returned element into multiple lines for readability, and added parentheses so that JavaScript doesn't insert a semicolon after `return` and break our code.

Now we're passing down two props from Board to Square: `value` and `onClick`. The `onClick` prop is a function that Square can call when clicked. We'll make the following changes to Square:

* Replace `this.state.value` with `this.props.value` in Square's `render` method
* Replace `this.setState()` with `this.props.onClick()` in Square's `render` method
* Delete the `constructor` from Square because Square no longer keeps track of the game's state

After these changes, the Square component looks like this:

```javascript{1,2,6,8}
class Square extends React.Component {
  render() {
    return (
      <button
        className="square"
        onClick={() => this.props.onClick()}
      >
        {this.props.value}
      </button>
    );
  }
}
```

When a Square is clicked, the `onClick` function provided by the Board is called. Here's a review of how this is achieved:

1. The `onClick` prop on the built-in DOM `<button>` component tells React to set up a click event listener.
2. When the button is clicked, React will call the `onClick` event handler that is defined in Square's `render()` method.
3. This event handler calls `this.props.onClick()`. The Square's `onClick` prop was specified by the Board.
4. Since the Board passed `onClick={() => this.handleClick(i)}` to Square, the Square calls `this.handleClick(i)` when clicked.
5. We have not defined the `handleClick()` method yet, so our code crashes. If you click a square now, you should see a red error screen saying something like "this.handleClick is not a function".

>Note
>
>The DOM `<button>` element's `onClick` attribute has a special meaning to React because it is a built-in component. For custom components like Square, the naming is up to you. We could give any name to the Square's `onClick` prop or Board's `handleClick` method, and the code would work the same. In React, it's conventional to use `on[Event]` names for props which represent events and `handle[Event]` for the methods which handle the events.

When we try to click a Square, we should get an error because we haven't defined `handleClick` yet. We'll now add `handleClick` to the Board class:

```javascript{9-13}
class Board extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      squares: Array(9).fill(null),
    };
  }

  handleClick(i) {
    const squares = this.state.squares.slice();
    squares[i] = 'X';
    this.setState({squares: squares});
  }

  renderSquare(i) {
    return (
      <Square
        value={this.state.squares[i]}
        onClick={() => this.handleClick(i)}
      />
    );
  }

  render() {
    const status = 'Next player: X';

    return (
      <div>
        <div className="status">{status}</div>
        <div className="board-row">
          {this.renderSquare(0)}
          {this.renderSquare(1)}
          {this.renderSquare(2)}
        </div>
        <div className="board-row">
          {this.renderSquare(3)}
          {this.renderSquare(4)}
          {this.renderSquare(5)}
        </div>
        <div className="board-row">
          {this.renderSquare(6)}
          {this.renderSquare(7)}
          {this.renderSquare(8)}
        </div>
      </div>
    );
  }
}
```

**[View the full code at this point](https://codepen.io/gaearon/pen/ybbQJX?editors=0010)**

After these changes, we're again able to click on the Squares to fill them, the same as we had before. However, now the state is stored in the Board component instead of the individual Square components. When the Board's state changes, the Square components re-render automatically. Keeping the state of all squares in the Board component will allow it to determine the winner in the future.

Since the Square components no longer maintain state, the Square components receive values from the Board component and inform the Board component when they're clicked. In React terms, the Square components are now **controlled components**. The Board has full control over them.

Note how in `handleClick`, we call `.slice()` to create a copy of the `squares` array to modify instead of modifying the existing array. We will explain why we create a copy of the `squares` array in the next section.

### Why Immutability Is Important {#why-immutability-is-important}

In the previous code example, we suggested that you use the `.slice()` method to create a copy of the `squares` array to modify instead of modifying the existing array. We'll now discuss immutability and why immutability is important to learn.

There are generally two approaches to changing data. The first approach is to *mutate* the data by directly changing the data's values. The second approach is to replace the data with a new copy which has the desired changes.

#### Data Change with Mutation {#data-change-with-mutation}
```javascript
var player = {score: 1, name: 'Jeff'};
player.score = 2;
// Now player is {score: 2, name: 'Jeff'}
```

#### Data Change without Mutation {#data-change-without-mutation}
```javascript
var player = {score: 1, name: 'Jeff'};

var newPlayer = Object.assign({}, player, {score: 2});
// Now player is unchanged, but newPlayer is {score: 2, name: 'Jeff'}

// Or if you are using object spread syntax proposal, you can write:
// var newPlayer = {...player, score: 2};
```

The end result is the same but by not mutating (or changing the underlying data) directly, we gain several benefits described below.

#### Complex Features Become Simple {#complex-features-become-simple}

Immutability makes complex features much easier to implement. Later in this tutorial, we will implement a "time travel" feature that allows us to review the tic-tac-toe game's history and "jump back" to previous moves. This functionality isn't specific to games -- an ability to undo and redo certain actions is a common requirement in applications. Avoiding direct data mutation lets us keep previous versions of the game's history intact, and reuse them later.

#### Detecting Changes {#detecting-changes}

Detecting changes in mutable objects is difficult because they are modified directly. This detection requires the mutable object to be compared to previous copies of itself and the entire object tree to be traversed.

Detecting changes in immutable objects is considerably easier. If the immutable object that is being referenced is different than the previous one, then the object has changed.

#### Determining When to Re-Render in React {#determining-when-to-re-render-in-react}

The main benefit of immutability is that it helps you build _pure components_ in React. Immutable data can easily determine if changes have been made which helps to determine when a component requires re-rendering.

You can learn more about `shouldComponentUpdate()` and how you can build *pure components* by reading [Optimizing Performance](/docs/optimizing-performance.html#examples).

### Function Components {#function-components}

We'll now change the Square to be a **function component**.

In React, **function components** are a simpler way to write components that only contain a `render` method and don't have their own state. Instead of defining a class which extends `React.Component`, we can write a function that takes `props` as input and returns what should be rendered. Function components are less tedious to write than classes, and many components can be expressed this way.

Replace the Square class with this function:

```javascript
function Square(props) {
  return (
    <button className="square" onClick={props.onClick}>
      {props.value}
    </button>
  );
}
```

We have changed `this.props` to `props` both times it appears.

**[View the full code at this point](https://codepen.io/gaearon/pen/QvvJOv?editors=0010)**

>Note
>
>When we modified the Square to be a function component, we also changed `onClick={() => this.props.onClick()}` to a shorter `onClick={props.onClick}` (note the lack of parentheses on *both* sides).

### Taking Turns {#taking-turns}

We now need to fix an obvious defect in our tic-tac-toe game: the "O"s cannot be marked on the board.

We'll set the first move to be "X" by default. We can set this default by modifying the initial state in our Board constructor:

```javascript{6}
class Board extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      squares: Array(9).fill(null),
      xIsNext: true,
    };
  }
```

Each time a player moves, `xIsNext` (a boolean) will be flipped to determine which player goes next and the game's state will be saved. We'll update the Board's `handleClick` function to flip the value of `xIsNext`:

```javascript{3,6}
  handleClick(i) {
    const squares = this.state.squares.slice();
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      squares: squares,
      xIsNext: !this.state.xIsNext,
    });
  }
```

With this change, "X"s and "O"s can take turns. Try it!

Let's also change the "status" text in Board's `render` so that it displays which player has the next turn:

```javascript{2}
  render() {
    const status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');

    return (
      // the rest has not changed
```

After applying these changes, you should have this Board component:

```javascript{6,11-16,29}
class Board extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      squares: Array(9).fill(null),
      xIsNext: true,
    };
  }

  handleClick(i) {
    const squares = this.state.squares.slice();
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      squares: squares,
      xIsNext: !this.state.xIsNext,
    });
  }

  renderSquare(i) {
    return (
      <Square
        value={this.state.squares[i]}
        onClick={() => this.handleClick(i)}
      />
    );
  }

  render() {
    const status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');

    return (
      <div>
        <div className="status">{status}</div>
        <div className="board-row">
          {this.renderSquare(0)}
          {this.renderSquare(1)}
          {this.renderSquare(2)}
        </div>
        <div className="board-row">
          {this.renderSquare(3)}
          {this.renderSquare(4)}
          {this.renderSquare(5)}
        </div>
        <div className="board-row">
          {this.renderSquare(6)}
          {this.renderSquare(7)}
          {this.renderSquare(8)}
        </div>
      </div>
    );
  }
}
```

**[View the full code at this point](https://codepen.io/gaearon/pen/KmmrBy?editors=0010)**

### Declaring a Winner {#declaring-a-winner}

Now that we show which player's turn is next, we should also show when the game is won and there are no more turns to make. Copy this helper function and paste it at the end of the file:

```javascript
function calculateWinner(squares) {
  const lines = [
    [0, 1, 2],
    [3, 4, 5],
    [6, 7, 8],
    [0, 3, 6],
    [1, 4, 7],
    [2, 5, 8],
    [0, 4, 8],
    [2, 4, 6],
  ];
  for (let i = 0; i < lines.length; i++) {
    const [a, b, c] = lines[i];
    if (squares[a] && squares[a] === squares[b] && squares[a] === squares[c]) {
      return squares[a];
    }
  }
  return null;
}
```

Given an array of 9 squares, this function will check for a winner and return `'X'`, `'O'`, or `null` as appropriate.

We will call `calculateWinner(squares)` in the Board's `render` function to check if a player has won. If a player has won, we can display text such as "Winner: X" or "Winner: O". We'll replace the `status` declaration in Board's `render` function with this code:

```javascript{2-8}
  render() {
    const winner = calculateWinner(this.state.squares);
    let status;
    if (winner) {
      status = 'Winner: ' + winner;
    } else {
      status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');
    }

    return (
      // the rest has not changed
```

We can now change the Board's `handleClick` function to return early by ignoring a click if someone has won the game or if a Square is already filled:

```javascript{3-5}
  handleClick(i) {
    const squares = this.state.squares.slice();
    if (calculateWinner(squares) || squares[i]) {
      return;
    }
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      squares: squares,
      xIsNext: !this.state.xIsNext,
    });
  }
```

**[View the full code at this point](https://codepen.io/gaearon/pen/LyyXgK?editors=0010)**

Congratulations! You now have a working tic-tac-toe game. And you've just learned the basics of React too. So *you're* probably the real winner here.

## Adding Time Travel {#adding-time-travel}

As a final exercise, let's make it possible to "go back in time" to the previous moves in the game.

### Storing a History of Moves {#storing-a-history-of-moves}

If we mutated the `squares` array, implementing time travel would be very difficult.

However, we used `slice()` to create a new copy of the `squares` array after every move, and [treated it as immutable](#why-immutability-is-important). This will allow us to store every past version of the `squares` array, and navigate between the turns that have already happened.

We'll store the past `squares` arrays in another array called `history`. The `history` array represents all board states, from the first to the last move, and has a shape like this:

```javascript
history = [
  // Before first move
  {
    squares: [
      null, null, null,
      null, null, null,
      null, null, null,
    ]
  },
  // After first move
  {
    squares: [
      null, null, null,
      null, 'X', null,
      null, null, null,
    ]
  },
  // After second move
  {
    squares: [
      null, null, null,
      null, 'X', null,
      null, null, 'O',
    ]
  },
  // ...
]
```

Now we need to decide which component should own the `history` state.

### Lifting State Up, Again {#lifting-state-up-again}

We'll want the top-level Game component to display a list of past moves. It will need access to the `history` to do that, so we will place the `history` state in the top-level Game component.

Placing the `history` state into the Game component lets us remove the `squares` state from its child Board component. Just like we ["lifted state up"](#lifting-state-up) from the Square component into the Board component, we are now lifting it up from the Board into the top-level Game component. This gives the Game component full control over the Board's data, and lets it instruct the Board to render previous turns from the `history`.

First, we'll set up the initial state for the Game component within its constructor:

```javascript{2-10}
class Game extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      history: [{
        squares: Array(9).fill(null),
      }],
      xIsNext: true,
    };
  }

  render() {
    return (
      <div className="game">
        <div className="game-board">
          <Board />
        </div>
        <div className="game-info">
          <div>{/* status */}</div>
          <ol>{/* TODO */}</ol>
        </div>
      </div>
    );
  }
}
```

Next, we'll have the Board component receive `squares` and `onClick` props from the Game component. Since we now have a single click handler in Board for many Squares, we'll need to pass the location of each Square into the `onClick` handler to indicate which Square was clicked. Here are the required steps to transform the Board component:

* Delete the `constructor` in Board.
* Replace `this.state.squares[i]` with `this.props.squares[i]` in Board's `renderSquare`.
* Replace `this.handleClick(i)` with `this.props.onClick(i)` in Board's `renderSquare`.

The Board component now looks like this:

```javascript{17,18}
class Board extends React.Component {
  handleClick(i) {
    const squares = this.state.squares.slice();
    if (calculateWinner(squares) || squares[i]) {
      return;
    }
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      squares: squares,
      xIsNext: !this.state.xIsNext,
    });
  }

  renderSquare(i) {
    return (
      <Square
        value={this.props.squares[i]}
        onClick={() => this.props.onClick(i)}
      />
    );
  }

  render() {
    const winner = calculateWinner(this.state.squares);
    let status;
    if (winner) {
      status = 'Winner: ' + winner;
    } else {
      status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');
    }

    return (
      <div>
        <div className="status">{status}</div>
        <div className="board-row">
          {this.renderSquare(0)}
          {this.renderSquare(1)}
          {this.renderSquare(2)}
        </div>
        <div className="board-row">
          {this.renderSquare(3)}
          {this.renderSquare(4)}
          {this.renderSquare(5)}
        </div>
        <div className="board-row">
          {this.renderSquare(6)}
          {this.renderSquare(7)}
          {this.renderSquare(8)}
        </div>
      </div>
    );
  }
}
```

We'll update the Game component's `render` function to use the most recent history entry to determine and display the game's status:

```javascript{2-11,16-19,22}
  render() {
    const history = this.state.history;
    const current = history[history.length - 1];
    const winner = calculateWinner(current.squares);

    let status;
    if (winner) {
      status = 'Winner: ' + winner;
    } else {
      status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');
    }

    return (
      <div className="game">
        <div className="game-board">
          <Board
            squares={current.squares}
            onClick={(i) => this.handleClick(i)}
          />
        </div>
        <div className="game-info">
          <div>{status}</div>
          <ol>{/* TODO */}</ol>
        </div>
      </div>
    );
  }
```

Since the Game component is now rendering the game's status, we can remove the corresponding code from the Board's `render` method. After refactoring, the Board's `render` function looks like this:

```js{1-4}
  render() {
    return (
      <div>
        <div className="board-row">
          {this.renderSquare(0)}
          {this.renderSquare(1)}
          {this.renderSquare(2)}
        </div>
        <div className="board-row">
          {this.renderSquare(3)}
          {this.renderSquare(4)}
          {this.renderSquare(5)}
        </div>
        <div className="board-row">
          {this.renderSquare(6)}
          {this.renderSquare(7)}
          {this.renderSquare(8)}
        </div>
      </div>
    );
  }
```

Finally, we need to move the `handleClick` method from the Board component to the Game component. We also need to modify `handleClick` because the Game component's state is structured differently. Within the Game's `handleClick` method, we concatenate new history entries onto `history`.

```javascript{2-4,10-12}
  handleClick(i) {
    const history = this.state.history;
    const current = history[history.length - 1];
    const squares = current.squares.slice();
    if (calculateWinner(squares) || squares[i]) {
      return;
    }
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      history: history.concat([{
        squares: squares,
      }]),
      xIsNext: !this.state.xIsNext,
    });
  }
```

>Note
>
>Unlike the array `push()` method you might be more familiar with, the `concat()` method doesn't mutate the original array, so we prefer it.

At this point, the Board component only needs the `renderSquare` and `render` methods. The game's state and the `handleClick` method should be in the Game component.

**[View the full code at this point](https://codepen.io/gaearon/pen/EmmOqJ?editors=0010)**

### Showing the Past Moves {#showing-the-past-moves}

Since we are recording the tic-tac-toe game's history, we can now display it to the player as a list of past moves.

We learned earlier that React elements are first-class JavaScript objects; we can pass them around in our applications. To render multiple items in React, we can use an array of React elements.

In JavaScript, arrays have a [`map()` method](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) that is commonly used for mapping data to other data, for example:

```js
const numbers = [1, 2, 3];
const doubled = numbers.map(x => x * 2); // [2, 4, 6]
```

Using the `map` method, we can map our history of moves to React elements representing buttons on the screen, and display a list of buttons to "jump" to past moves.

Let's `map` over the `history` in the Game's `render` method:

```javascript{6-15,34}
  render() {
    const history = this.state.history;
    const current = history[history.length - 1];
    const winner = calculateWinner(current.squares);

    const moves = history.map((step, move) => {
      const desc = move ?
        'Go to move #' + move :
        'Go to game start';
      return (
        <li>
          <button onClick={() => this.jumpTo(move)}>{desc}</button>
        </li>
      );
    });

    let status;
    if (winner) {
      status = 'Winner: ' + winner;
    } else {
      status = 'Next player: ' + (this.state.xIsNext ? 'X' : 'O');
    }

    return (
      <div className="game">
        <div className="game-board">
          <Board
            squares={current.squares}
            onClick={(i) => this.handleClick(i)}
          />
        </div>
        <div className="game-info">
          <div>{status}</div>
          <ol>{moves}</ol>
        </div>
      </div>
    );
  }
```

**[View the full code at this point](https://codepen.io/gaearon/pen/EmmGEa?editors=0010)**

For each move in the tic-tac-toes's game's history, we create a list item `<li>` which contains a button `<button>`. The button has a `onClick` handler which calls a method called `this.jumpTo()`. We haven't implemented the `jumpTo()` method yet. For now, we should see a list of the moves that have occurred in the game and a warning in the developer tools console that says:

>  Warning:
>  Each child in an array or iterator should have a unique "key" prop. Check the render method of "Game".

Let's discuss what the above warning means.

### Picking a Key {#picking-a-key}

When we render a list, React stores some information about each rendered list item. When we update a list, React needs to determine what has changed. We could have added, removed, re-arranged, or updated the list's items.

Imagine transitioning from

```html
<li>Alexa: 7 tasks left</li>
<li>Ben: 5 tasks left</li>
```

to

```html
<li>Ben: 9 tasks left</li>
<li>Claudia: 8 tasks left</li>
<li>Alexa: 5 tasks left</li>
```

In addition to the updated counts, a human reading this would probably say that we swapped Alexa and Ben's ordering and inserted Claudia between Alexa and Ben. However, React is a computer program and does not know what we intended. Because React cannot know our intentions, we need to specify a *key* property for each list item to differentiate each list item from its siblings. One option would be to use the strings `alexa`, `ben`, `claudia`. If we were displaying data from a database, Alexa, Ben, and Claudia's database IDs could be used as keys.

```html
<li key={user.id}>{user.name}: {user.taskCount} tasks left</li>
```

When a list is re-rendered, React takes each list item's key and searches the previous list's items for a matching key. If the current list has a key that didn't exist before, React creates a component. If the current list is missing a key that existed in the previous list, React destroys the previous component. If two keys match, the corresponding component is moved. Keys tell React about the identity of each component which allows React to maintain state between re-renders. If a component's key changes, the component will be destroyed and re-created with a new state.

`key` is a special and reserved property in React (along with `ref`, a more advanced feature). When an element is created, React extracts the `key` property and stores the key directly on the returned element. Even though `key` may look like it belongs in `props`, `key` cannot be referenced using `this.props.key`. React automatically uses `key` to decide which components to update. A component cannot inquire about its `key`.

**It's strongly recommended that you assign proper keys whenever you build dynamic lists.** If you don't have an appropriate key, you may want to consider restructuring your data so that you do.

If no key is specified, React will present a warning and use the array index as a key by default. Using the array index as a key is problematic when trying to re-order a list's items or inserting/removing list items. Explicitly passing `key={i}` silences the warning but has the same problems as array indices and is not recommended in most cases.

Keys do not need to be globally unique; they only need to be unique between components and their siblings.


### Implementing Time Travel {#implementing-time-travel}

In the tic-tac-toe game's history, each past move has a unique ID associated with it: it's the sequential number of the move. The moves are never re-ordered, deleted, or inserted in the middle, so it's safe to use the move index as a key.

In the Game component's `render` method, we can add the key as `<li key={move}>` and React's warning about keys should disappear:

```js{6}
    const moves = history.map((step, move) => {
      const desc = move ?
        'Go to move #' + move :
        'Go to game start';
      return (
        <li key={move}>
          <button onClick={() => this.jumpTo(move)}>{desc}</button>
        </li>
      );
    });
```

**[View the full code at this point](https://codepen.io/gaearon/pen/PmmXRE?editors=0010)**

Clicking any of the list item's buttons throws an error because the `jumpTo` method is undefined. Before we implement `jumpTo`, we'll add `stepNumber` to the Game component's state to indicate which step we're currently viewing.

First, add `stepNumber: 0` to the initial state in Game's `constructor`:

```js{8}
class Game extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      history: [{
        squares: Array(9).fill(null),
      }],
      stepNumber: 0,
      xIsNext: true,
    };
  }
```

Next, we'll define the `jumpTo` method in Game to update that `stepNumber`. We also set `xIsNext` to true if the number that we're changing `stepNumber` to is even:

```javascript{5-10}
  handleClick(i) {
    // this method has not changed
  }

  jumpTo(step) {
    this.setState({
      stepNumber: step,
      xIsNext: (step % 2) === 0,
    });
  }

  render() {
    // this method has not changed
  }
```

We will now make a few changes to the Game's `handleClick` method which fires when you click on a square.

The `stepNumber` state we've added reflects the move displayed to the user now. After we make a new move, we need to update `stepNumber` by adding `stepNumber: history.length` as part of the `this.setState` argument. This ensures we don't get stuck showing the same move after a new one has been made.

We will also replace reading `this.state.history` with `this.state.history.slice(0, this.state.stepNumber + 1)`. This ensures that if we "go back in time" and then make a new move from that point, we throw away all the "future" history that would now become incorrect.

```javascript{2,13}
  handleClick(i) {
    const history = this.state.history.slice(0, this.state.stepNumber + 1);
    const current = history[history.length - 1];
    const squares = current.squares.slice();
    if (calculateWinner(squares) || squares[i]) {
      return;
    }
    squares[i] = this.state.xIsNext ? 'X' : 'O';
    this.setState({
      history: history.concat([{
        squares: squares
      }]),
      stepNumber: history.length,
      xIsNext: !this.state.xIsNext,
    });
  }
```

Finally, we will modify the Game component's `render` method from always rendering the last move to rendering the currently selected move according to `stepNumber`:

```javascript{3}
  render() {
    const history = this.state.history;
    const current = history[this.state.stepNumber];
    const winner = calculateWinner(current.squares);

    // the rest has not changed
```

If we click on any step in the game's history, the tic-tac-toe board should immediately update to show what the board looked like after that step occurred.

**[View the full code at this point](https://codepen.io/gaearon/pen/gWWZgR?editors=0010)**

### Wrapping Up {#wrapping-up}

Congratulations! You've created a tic-tac-toe game that:

* Lets you play tic-tac-toe,
* Indicates when a player has won the game,
* Stores a game's history as a game progresses,
* Allows players to review a game's history and see previous versions of a game's board.

Nice work! We hope you now feel like you have a decent grasp on how React works.

Check out the final result here: **[Final Result](https://codepen.io/gaearon/pen/gWWZgR?editors=0010)**.

If you have extra time or want to practice your new React skills, here are some ideas for improvements that you could make to the tic-tac-toe game which are listed in order of increasing difficulty:

1. Display the location for each move in the format (col, row) in the move history list.
2. Bold the currently selected item in the move list.
3. Rewrite Board to use two loops to make the squares instead of hardcoding them.
4. Add a toggle button that lets you sort the moves in either ascending or descending order.
5. When someone wins, highlight the three squares that caused the win.
6. When no one wins, display a message about the result being a draw.

Throughout this tutorial, we touched on React concepts including elements, components, props, and state. For a more detailed explanation of each of these topics, check out [the rest of the documentation](/docs/hello-world.html). To learn more about defining components, check out the [`React.Component` API reference](/docs/react-component.html).
