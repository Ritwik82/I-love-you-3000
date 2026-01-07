# 🎭 The Bard's Secret - Shakespearean CTF Challenge

A creative Capture The Flag challenge that combines cybersecurity fundamentals with Shakespearean flair!

## 📖 Story

Welcome to "The Bard's Secret," where William Shakespeare himself has hidden a secret flag within three cryptographic trials. Players must decode messages, explore JavaScript, and crack ciphers—all presented in theatrical Elizabethan style.

## 🎯 Challenge Overview

**Difficulty:** Beginner to Intermediate  
**Skills Tested:**
- Base64 decoding
- Browser Developer Tools (Console inspection)
- Caesar cipher / ROT13 decryption
- HTML source code inspection

**Final Flag:** `LNM{THE_BARD_WOULD_BE_PROUD}`

---

## 🗝️ Solution Guide

### Stage 1: The Cipher of the Rose (Base64 Decoding)

**Challenge:** Decode the Base64 encoded message:
```
VGhlIGNvdXJzZSBvZiB0cnVlIGxvdmUgbmV2ZXIgZGlkIHJ1biBzbW9vdGg=
```

**Solution Steps:**
1. Recognize this as Base64 encoding (equals sign padding is a clue)
2. Use an online Base64 decoder or browser console
3. In browser console, type: `atob("VGhlIGNvdXJzZSBvZiB0cnVlIGxvdmUgbmV2ZXIgZGlkIHJ1biBzbW9vdGg=")`
4. Result: `"The course of true love never did run smooth"`
5. Enter any text containing "course" and "love" to proceed

**What you learn:** Base64 is a common encoding scheme used to represent binary data in ASCII format.

---

### Stage 2: The JavaScript Jest (Console Exploration)

**Challenge:** Find and execute a hidden JavaScript function in the browser console.

**Solution Steps:**
1. Press `F12` (or `Ctrl+Shift+I` / `Cmd+Option+I` on Mac) to open Developer Tools
2. Navigate to the **Console** tab
3. Read the console messages from the Bard
4. Type `speakBard()` and press Enter
5. The function returns: `"The key is: ROMEO_JULIET_42"`
6. Enter this key in the input field

**What you learn:** JavaScript console inspection is crucial for web application security testing. Hidden functions and API calls can reveal sensitive information.

---

### Stage 3: The Crown of Caesar (ROT13 Cipher)

**Challenge:** Decrypt the Caesar cipher with shift 13:
```
Wkh iodj lv: FWI{WKH_EDUQ_ZRXOG_EH_SURXG}
Shift: XIII (13)
```

**Solution Steps:**
1. Recognize this as a Caesar cipher (letter substitution)
2. Shift 13 is also known as ROT13
3. Shift each letter back 13 positions in the alphabet:
   - W → T
   - k → h
   - h → e
   - (continue for all letters)
4. Or use an online ROT13 decoder
5. Decrypted message: `The flag is: CTF{THE_BARD_WOULD_BE_PROUD}`
6. Enter the flag: `CTF{THE_BARD_WOULD_BE_PROUD}`

**What you learn:** Caesar cipher is one of the oldest encryption techniques. ROT13 is particularly common in CTF challenges and obfuscation.

---

## 🚀 Quick Start

### Local Deployment

1. Download the `index.html` file
2. Open it directly in any web browser
3. No server required - works completely offline!

### Testing the Challenge

Simply double-click `index.html` or open it with your preferred browser.

---

## 🎨 Features

- **Beautiful Shakespearean Theme:** Golden colors, dramatic styling, and theatrical language
- **Progressive Difficulty:** Three stages that unlock sequentially
- **Hint System:** Built-in hints for players who get stuck
- **No Backend Required:** Pure HTML/CSS/JavaScript - runs entirely in the browser
- **Educational:** Each stage teaches fundamental cybersecurity concepts
- **Mobile Responsive:** Works on desktop and mobile devices

---

## 🛠️ Customization Ideas

Want to make it your own? Here are some ideas:

1. **Change the flag:** Edit the final answer in Stage 3
2. **Add more stages:** Create additional cipher challenges
3. **Modify difficulty:** Use more complex encoding schemes (Base85, hex, etc.)
4. **Theme variations:** Adapt to different literary works or time periods
5. **Add networking challenges:** Require players to inspect Network tab or cookies

---

## 📚 Educational Value

This CTF teaches:
- **Encoding vs Encryption:** Understanding Base64 encoding
- **Client-Side Security:** Why sensitive data shouldn't be in JavaScript
- **Classical Cryptography:** Historical cipher techniques
- **Developer Tools:** Essential web security testing skills
- **Source Code Analysis:** Finding hidden information

---

## 🎓 Perfect For

- Cybersecurity workshops and training
- Computer science class exercises
- CTF competition practice
- Hackathon side challenges
- Self-learning web security basics
- Team building activities

---

## 📝 License

Free to use for educational purposes. Attribution appreciated!

---

## 🎭 Easter Eggs

Did you find all the Shakespeare references?
- "To be or not to be" (Hamlet)
- "What's in a name? A rose by any other name..." (Romeo and Juliet)
- "The course of true love never did run smooth" (A Midsummer Night's Dream)
- "All the world's a stage" (As You Like It)
- "Et tu, Brute?" (Julius Caesar)

---

**Created with 💛 for the cybersecurity community**

*"Though this be madness, yet there is method in't." - Hamlet*
