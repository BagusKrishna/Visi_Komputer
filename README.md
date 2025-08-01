# Deteksi Penyakit Daun Tomat dengan YOLOv8 & YOLOv9

**Tugas Besar Visi Komputer**  
oleh  
Gede Bagus Krishnanditya Merta  
Raka Aditya Waluya  
Dody Adi Sancoko  

---

## 📌 Deskripsi Proyek  
Proyek ini membandingkan dua model deep learning terkini, yaitu **YOLOv8** dan **YOLOv9**, untuk mendeteksi 10 jenis penyakit pada daun tomat menggunakan citra dari lingkungan alami. Dataset terdiri dari **10.825 gambar** dan setelah augmentasi meningkat menjadi **15.154 gambar pelatihan**. Model dievaluasi menggunakan metrik seperti mAP, Precision, dan F1-score.  
📈 **Hasilnya:**
- **YOLOv9** unggul dalam akurasi, dengan precision 92.74% dan F1-score 92.81%
- **YOLOv8** unggul dalam efisiensi waktu pelatihan (hanya 77.11 menit vs 175.83 menit pada YOLOv9)

---

## 🧪 Implementasi Streamlit  
Aplikasi ini dibuat menggunakan **Streamlit** untuk menampilkan demo deteksi penyakit daun tomat. Pengguna cukup mengupload gambar daun tomat, lalu model akan memprediksi jenis penyakitnya secara visual.  
Deteksi dapat dilakukan menggunakan:
- **YOLOv8s** (versi ringan dan cepat)
- **YOLOv9s** (versi akurat dan stabil)

---

## 📂 Isi Repository
- `app.py` – Aplikasi Streamlit untuk demo deteksi penyakit daun tomat.
- `yolov8n.pt` – Model YOLOv8 (versi ringan) hasil pelatihan.
- `yolov8s.pt` – Model YOLOv8s terlatih.
- `yolov9s.pt` – Model YOLOv9s terlatih.
- `requirements.txt` – Dependensi Python.
- `apt.txt`, `runtime.txt` – Konfigurasi tambahan untuk deployment.
- `README.md` – Dokumentasi proyek ini.

---

## 📸 Kelas Penyakit Daun Tomat
Model dilatih untuk mengenali 10 kelas:
- Bacterial Spot  
- Early Blight  
- Late Blight  
- Leaf Mold  
- Septoria Leaf Spot  
- Spider Mites  
- Target Spot  
- Yellow Leaf Curl Virus  
- Mosaic Virus  
- Healthy (daun sehat)

---

## 🧰 Cara Menjalankan Aplikasi

1. **Clone repositori**  
   ```bash
   git clone https://github.com/BagusKrishna/Visi_Komputer.git
   cd Visi_Komputer

2. **Install dependensi**  
   ```bash
   pip install -r requirements.txt

2. **Jalankan Streamlit app**  
   ```bash
   streamlit run app.py
