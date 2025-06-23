# 🕵️‍♂️ Steganography using LSB and XOR Encryption

This project demonstrates how to hide and retrieve secret messages in images using **Least Significant Bit (LSB) steganography** combined with **XOR encryption**.

![Demo](images/stego_output.jpg)

---

## 🔐 Features

- Hide messages inside images without visible change.
- XOR encryption for added security.
- Pixel-level decryption with debug output.
- End-of-message detection using a marker (`~`).
- Written in Python using Jupyter Notebook.

---

## 🛠️ Technologies Used

- Python 3
- OpenCV (`cv2`)
- Jupyter Notebook

---

## 🚀 How to Run

### 1. Install Requirements
```bash
pip install opencv-python
````

### 2. Open the Notebook

Run the notebook file:

```
Steganography_XOR_LSB.ipynb
```

Use Jupyter or any IDE like VSCode that supports `.ipynb` files.

---

## 🧪 Example Usage

### ➕ To Embed a Message:

```python
embed_encrypted_data('input.png', 'stego.png', 'secret', 'key123')
```

### 🔓 To Decode the Message:

```python
xor_decrypt('stego.png', 'key123')
```

---

## 📷 Image Guide

Place a sample input image in the root or `images/` folder.
Preferably use **PNG** format for lossless quality.

To show results in GitHub, add your output image to:

```
images/stego_output.png
```

---

## 📝 Sample Output

```
Decrypting pixel (0,0,0): 66 XOR 49 = 115 -> 's'
Decrypting pixel (1,2,1): 87 XOR 50 = 101 -> 'e'
Decrypting pixel (2,1,2): 80 XOR 51 = 99 -> 'c'
Decrypting pixel (3,0,0): 67 XOR 49 = 114 -> 'r'
Decrypting pixel (4,2,1): 87 XOR 50 = 101 -> 'e'
Decrypting pixel (5,1,2): 71 XOR 51 = 116 -> 't'

Decrypted message: secret
```

---

## 📂 Project Structure

```
steganography-xor-lsb/
├── Steganography_XOR_LSB.ipynb
├── README.md
└── images/
    └── stego_output.png
```

---

## 🔮 Future Scope

* Add a GUI (Tkinter or PyQt).
* Support steganography in audio/video files.
* Combine with AES encryption or other stronger methods.
* Add integrity check for message verification.

---

## 📃 License

This project is open-source and available for educational and research use.

```


