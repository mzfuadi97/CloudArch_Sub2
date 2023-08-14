# Submission2: Transformasi Skalabilitas E-commerce: Dari On-Premise ke Google Cloud Platform

**Username dicoding:** mzfuadi97

## Masalah
Aplikasi e-commerce dari perusahaan multinasional telah sukses beroperasi di pusat data on-premise. Namun, dengan bertambahnya jumlah pelanggan, muncul masalah skalabilitas terutama saat ada acara diskon flash sale yang menyebabkan tantangan pada kapasitas server dan bahkan mengakibatkan aplikasi mengalami downtime. Lambatnya waktu akses juga mengakibatkan ketidakpuasan pelanggan. Untuk mengatasi masalah ini, perusahaan memutuskan untuk memindahkan beban kerja ke Google Cloud Platform, dengan harapan mendapatkan arsitektur yang handal dan elastis, serta mampu memberikan kinerja yang optimal dan latensi rendah kepada pelanggan di seluruh dunia, terutama di Asia Tenggara dan Eropa. Sebagai Arsitek Google Cloud berpengalaman, saya ditugaskan untuk merancang dan mengimplementasikan arsitektur cloud baru ini.


## Solusi
Solusi arsitektur cloud meliputi skalabilitas otomatis untuk melayani pelanggan dengan latensi rendah dari Asia Tenggara dan Eropa, pemantauan infrastruktur oleh tim IT dengan akses audit eksternal, dan efisiensi biaya yang tetap mengikuti praktik terbaik dalam cloud computing.


Saya menerapkan autoscaling untuk menjamin high availability dan fault tolerance dengan arsitektur dual-region. Traffic didistribusikan melalui HTTP(S) load balancing, mencakup berbagai region. Autoscaling didukung oleh VPC yang aman dan fleksibel. Menggunakan region europe-west dan southeast asia, log dipantau melalui dashboard, termasuk CPU utilization dan traffic. Menggunakan n1-standard karena keseimbangan kinerja dan skalabilitas, dengan region yang dipilih untuk mengurangi latensi dan meningkatkan ketersediaan. Load balancer HTTP(S) global dipilih untuk mengakomodasi pengguna dari seluruh dunia.

## Arsitektur Cloud
Berikut adalah arsitektur cloud pada GCP untuk mendeploy aplikasi:
![Diagram Arsitektur Cloud](https://github.com/mzfuadi97/CloudArch_Sub1/assets/70827786/698b1280-db29-456e-b4a3-f93acb1d58b5)


## Dokumentasi Deploy Aplikasi
### Template-Instance
![Template Instance](https://github.com/mzfuadi97/CloudArch_Sub1/assets/70827786/33c4eb1f-9144-4344-a6c5-f93dd7e68f31)


### Autoscalling
![Autoscalling Instance Group](https://github.com/mzfuadi97/CloudArch_Sub1/assets/70827786/517fb593-8235-48f8-a1d4-504dd0079620)


### Monitoring-Instaces
![Template Instance](https://github.com/mzfuadi97/CloudArch_Sub1/assets/70827786/89a5a621-2e39-4ad3-98d9-623ca38a333f)


### Kalkulator-GCP
![Kalkulator Biaya Architect](https://github.com/mzfuadi97/CloudArch_Sub1/assets/70827786/f5d5c778-0839-4c6d-8a1b-74704506ecc7)

