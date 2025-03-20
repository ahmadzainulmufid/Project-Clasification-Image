# Model Klasifikasi Gambar

Proyek ini berisi model deep learning untuk klasifikasi gambar menggunakan TensorFlow. Model telah dikonversi ke format TensorFlow Lite (TFLite) dan TensorFlow.js (TFJS) agar dapat digunakan di berbagai platform.

## Struktur Folder
- `tfjs_model/`  → Model dalam format TensorFlow.js  
- `tflite/`  → Model dalam format TFLite dan file label  
- `saved_model/`  → Model asli dalam format TensorFlow SavedModel  
- `notebook.ipynb`  → Notebook untuk pelatihan dan konversi model  
- `README.md`  → Dokumentasi proyek  
- `requirements.txt`  → Daftar dependensi  

## Menjalankan Inferensi
### TensorFlow Lite
Gunakan Python:
```python
import tensorflow.lite as tflite
interpreter = tflite.Interpreter(model_path="tflite/model.tflite")
interpreter.allocate_tensors()
