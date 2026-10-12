Tugas 05 — Transfer Learning untuk Klasifikasi Citra dengan Data Terbatas
Dataset: Oxford-IIIT Pet (10 kelas: Abyssinian, Bengal, Birman, Persian, Siamese, beagle, boxer, chihuahua, pug, samoyed), split stratified 70/15/15, seed = 42. Arsitektur utama: ResNet-18 (ImageNet1K_V1). Pembanding (B5): efficientnet_b0.

Cara menjalankan
Buka Tugas05_Transfer_Learning.ipynb di Google Colab (Runtime GPU T4).
pip install -r requirements.txt (opsional; Colab sudah memuat library utama).
Run all cells. Dataset diunduh otomatis oleh torchvision.
Berkas luaran
training_log_per_epoch.csv — log loss/akurasi per epoch untuk semua kondisi
results_summary.csv|json — ringkasan metrik akhir per kondisi (sumber angka laporan)
fig_*.png — grafik kurva pembelajaran, failure analysis, confusion matrix, Grad-CAM
failure_cases.csv — daftar sampel misklasifikasi
Catatan
Pengujian memakai single seed (42). Seleksi model/strategi memakai validation set, bukan test set.
