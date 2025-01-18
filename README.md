# FallPose
## Overview
Proyek ini bertujuan untuk mengembangkan sistem deteksi pose yang mampu mengidentifikasi orang dalam kondisi terjatuh dan tidak terjatuh secara real-time. Sistem ini dirancang untuk mendukung pengawasan keselamatan, terutama di lingkungan dengan risiko tinggi seperti rumah sakit, fasilitas perawatan lanjut usia, atau area kerja yang rawan kecelakaan.

## Dataset
Dataset didapatkan dari gabungan dataset [yolov8-pose Computer Vision Project](https://universe.roboflow.com/yolo-xvnzo/yolov8-pose-utovc/dataset/3) yang memiliki gambar pose jatuh yang bervariasi. Persebaran data yang digunakan adalah sebagai berikut:  
| Folder  | Image Count | 
| ------------- | ------------- |
| Train  | 332 | 
| Validation | 95 | 
| Test | 47 |

## Model 
Proyek ini menggunakan model YOLOv11 sebagai algoritma deteksi objek utama, yang telah diimplementasikan dengan melakukan hyperparameter tuning untuk mengoptimalkan performa deteksi.

### Environment
- Quadro RTX 5000
- Python 3.12.1
- Pytorch 2.5.1
- Torchvision 0.20.1
- Torchaudio 2.5.1
- Ultralytics 8.3.39

### Metrik Evaluasi
![results](https://github.com/user-attachments/assets/c2dc71ac-7fcc-48b6-bd17-aecb9fe5ff7e)

| Model | epoch  | Imgsz | lr0  | lrf | Recall  | Precision | mAP50  | mAP50-95 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Baseline | 100  | 640  | 0.01  | 0.01 | 0.88649  | 0.9412  | 0.90595 | 0.6018  |

### Hasil
![val_batch2_pred](https://github.com/user-attachments/assets/f90b10f3-448e-4a89-985f-3c678b5f0bab)
