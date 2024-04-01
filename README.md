# Face recognition app using Streamlit

Ini adalah aplikasi pengenalan wajah yang dibuat menggunakan Python, [Face-Recognition API](https://github.com/ageitgey/face_recognition) dan kerangka kerja Streamlit. Aplikasi ini memungkinkan pengguna mengunggah gambar yang berisi wajah dan melakukan pengenalan wajah menggunakan perpustakaan pengenalan wajah.

## Features

- Deteksi dan pengenalan wajah
- Pengenalan multi-wajah
- Pilihan untuk menampilkan wajah yang dikenali
- Antarmuka yang ramah pengguna

## Requirements 
- Python 3.9
- Streamlit 1.22.0
- face_recognition 

## Repository structure
```bash
├───dataset
│   │───ID_Name.jpg
│   │───...
├───pages
│   ├───1_🔧_Updating.py
│   └───2_💾_Database
├───Tracking.py
│───utils.py
├───config.yaml 
├───requirements.txt
├───packages.txt
└───README.md
```

## Description
- **kumpulan data**: berisi gambar orang yang akan dikenali. Format nama file adalah ID_Name.jpg. `Misalnya, 1_Elon_Musk.jpg, 2_Jenna_Ortega.jpg  3_Bill_Gates.jpg, dll.` Bebas menggunakan format jpg, jpeg, atau png.
- **halaman**: berisi kode untuk setiap halaman aplikasi. Jika Anda ingin menambahkan lebih banyak halaman, Anda dapat membuat file baru dengan format `Order_Icon_Pagename` di folder ini, atau hanya halaman tanpa ikon dengan format `Order_Pagename`.
- **Tracking.py**: beranda aplikasi, digunakan untuk melacak secara real-time menggunakan webcam dan gambar.
- **utils.py**: berisi fungsi yang digunakan oleh aplikasi.
- **config.yaml**: berisi konfigurasi untuk aplikasi seperti jalur direktori kumpulan data dan pesan prompt.
- **requirements.txt**: berisi dependensi untuk aplikasi.
- **packages.txt**: berisi paket untuk aplikasi yang digunakan untuk diterapkan di Streamlit Cloud.



## Installation
1. Clone the repository
```bash
cd Face-recognition-app-using-Streamlit
```

2. Install the dependencies
```bash
pip install -r requirements.txt
```

3. Run the app
```bash
streamlit run Tracking.py
```

## Usage
1. Melacak secara real-time menggunakan webcam
2. Pelacakan menggunakan file gambar
3. Memperbarui database (menambah, menghapus dan memperbarui)
4. Melihat database


## Demo

1.  Tracking using camera
![Tracking using webcam](assets/webcam.gif) 

2. Tracking using picture 
![Tracking using picture](assets/tracking.png)

3. Adding new person to database
![Adding new person to database](assets/adding.png)



