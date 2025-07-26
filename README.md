
# Caesar Cipher

A simple Python program that encrypts and decrypts messages using the Caesar Cipher technique.

---

## Description

This program allows you to encode (encrypt) or decode (decrypt) a text message by shifting each letter by a specified number in the alphabet. It supports looping the shift around the alphabet and leaves non-alphabet characters unchanged.

The program repeatedly asks the user if they want to continue encoding or decoding messages until the user chooses to exit.

---

## Features

- Encode text by shifting letters forward in the alphabet.
- Decode text by shifting letters backward in the alphabet.
- Handles both uppercase and lowercase input (converts to lowercase internally).
- Non-alphabet characters (like spaces, punctuation) remain unchanged.
- Continuous operation until user decides to stop.

---

## Usage

1. Run the Python script.
2. Type `encode` to encrypt a message or `decode` to decrypt.
3. Enter the message you want to process.
4. Enter the shift number (integer).
5. View the result.
6. Choose whether to continue or exit.

---

## Example

```
Type 'encode' to encrypt, type 'decode' to decrypt:
encode
Type your message:
hello world
Type the shift number:
3
Here is the encoded result: khoor zruog

Type 'yes' if you want to go again. Otherwise, type 'no':
no
Thank you for choosing me
Goodbye!!
```

---

## Requirements

- Python 3.x

---

## Code Snippet

```python
alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 
            'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

def caesar(original_text, shift_amount, encode_or_decode):
    output_text = ""

    if encode_or_decode == "decode":
        shift_amount *= -1

    for letter in original_text:
        if letter not in alphabet:
            output_text += letter
        else:
            shifted_position = alphabet.index(letter) + shift_amount
            shifted_position %= len(alphabet)
            output_text += alphabet[shifted_position]
    print(f"Here is the {encode_or_decode}d result: {output_text}")
```

---

## Author

Naim Ibne Nasir  
Electrical and Electronics Engineering student  
Bangladesh Army University of Science and Technology (BAUST)

---

## License

This project is free to use and modify.

