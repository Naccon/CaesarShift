# CaesarShift CLI Tool 🕵️‍♂️🔐

A simple Python-based command line Caesar Cipher tool that allows users to encrypt or decrypt messages using a character shift technique.

---

## 🔧 Features

- Encrypt (`encode`) your message with a shift value.
- Decrypt (`decode`) any encoded message using the same shift.
- Preserves special characters, spaces, and punctuation.
- Automatically wraps around the alphabet.
- ASCII art logo at startup.

---

## 🚀 How It Works

Caesar Cipher is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet.

For example, with a shift of `3`:
```
original:   a b c d e
encrypted:  d e f g h
```

---

## 🧠 Example Usage

```
Type 'encode' to encrypt, type 'decode' to decrypt:
> encode

Type your message:
> hello world!

Type the shift number:
> 5

Here is the encoded result: mjqqt btwqi!
```

---

## 📁 Files

- `main.py`: Main Caesar Cipher logic and interactive loop.
- `art.py`: Contains the ASCII logo as a string variable `logo`.

---

## ✅ Requirements

- Python 3.x

---

## 🔄 Run the Program

```bash
python main.py
```

---


## 📜 License

This project is open-source and free to use.
