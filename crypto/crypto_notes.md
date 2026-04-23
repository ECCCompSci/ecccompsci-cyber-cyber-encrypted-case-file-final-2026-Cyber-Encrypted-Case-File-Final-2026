# 🔐 Cryptography Background — For Analysts

This file gives context on the cipher types used in this case. It does NOT give you the keys — you must figure those out yourself.

---

## Message 1 — Cipher Type
**Category:** Substitution cipher (classical)  
**Subcategory:** Caesar / ROT cipher  
**How it works:** Every letter in the plaintext is shifted a fixed number of positions forward in the alphabet. For example, with a shift of 3, A→D, B→E, C→F, and so on.  
**Weakness:** Only 25 possible keys. Frequency analysis easily breaks it — the most common letter in English text is E, so the most frequent letter in the ciphertext is likely the encrypted version of E.

**Your job:** Determine the shift value. Try common shifts first (3, 13). Count the most frequent letters in the ciphertext.

---

## Message 2 — Cipher Type
**Category:** Polyalphabetic substitution cipher  
**Subcategory:** Vigenère cipher  
**How it works:** Uses a keyword where each letter of the keyword determines the Caesar shift for the corresponding letter of the plaintext. The keyword repeats throughout the message. Example: keyword=CAT means letter 1 shifts by 2 (C), letter 2 shifts by 0 (A), letter 3 shifts by 19 (T), then repeats.  
**Weakness:** Harder than Caesar but crackable if the keyword length can be guessed (Kasiski examination or index of coincidence). If the keyword is known, decryption is straightforward.

**Your job:** A hint about the keyword appears in the message file itself. Use a Vigenère decryption table or an online Vigenère decoder to confirm.

---

## Why These Ciphers Are Not Used Today
Modern systems use symmetric encryption (AES-256) and asymmetric encryption (RSA, ECC) because classical ciphers can be broken in seconds by a computer. Classical ciphers have tiny key spaces and predictable patterns that frequency analysis exploits.

---

## Vocabulary Review
| Term | Definition |
|---|---|
| Plaintext | The original readable message |
| Ciphertext | The encrypted, unreadable message |
| Key | The value used to encrypt/decrypt |
| Caesar cipher | Fixed-shift substitution cipher |
| Vigenère cipher | Keyword-based polyalphabetic cipher |
| Frequency analysis | Exploiting letter frequency patterns to break ciphers |
| Symmetric encryption | Same key for encrypt and decrypt (e.g., AES) |
| Asymmetric encryption | Public/private key pair (e.g., RSA) |
