# **Execution — Portofolio Rizki R.**

## **Step 1: Initial Build & Architecture**

### **Prompt**

kamu adalah seorang senior front end engineer yang sudah berpengalaman dalam mengembangkan sebuah awwards standard, tugas kamu adalah bantu saya dalam membuat website portofolio berdasarkan brainstorm.md dan juga harus mengikuti details.md. output harus dalam bentuk html, jika memungkinkan css juga dipisah. penggunaan javascript bisa di dalam file html. tapi untuk css, jika bisa dipisah saja.

### **RTCC-O Check**

- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### **AI Response**

Menghasilkan struktur dasar menggunakan font Plus Jakarta Sans & Inter. Implementasi section "API Status" dan "Logic Breakdown" untuk menonjolkan sisi Backend Engineer. Menggunakan CSS Custom Properties untuk manajemen warna Slate Navy & Ghost White.

### **Review**

- \[✅\] Sesuai constraints?
- \[✅\] Format sesuai?
- \[✅\] Bisa dipahami?
- Changes: Menggunakan clamp() untuk fluid typography agar responsif tanpa banyak media queries.

## **Step 2: Error Correction (Compiler Issue)**

### **Prompt**

There's an error in the code that you generated... \[Error: Expected identifier but found "\!"\]

### **RTCC-O Check**

- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### **AI Response**

Memperbaiki identifikasi file agar compiler tidak membaca \<\!DOCTYPE html\> sebagai sintaks JavaScript. Memastikan file output didefinisikan sebagai file HTML murni.

### **Review**

- \[✅\] Sesuai constraints?
- \[✅\] Format sesuai?
- \[✅\] Bisa dipahami?
- Changes: Penyesuaian tag file block menjadi html untuk memastikan integrasi preview yang tepat.

## **Step 3: Smooth Scroll Implementation**

### **Prompt**

tambahkan smooth scrool seperti efek locomotive smooth scroll versi css.

### **RTCC-O Check**

- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### **AI Response**

Menambahkan scroll-behavior: smooth pada level HTML dan mengoptimalkan transisi cubic-bezier(0.16, 1, 0.3, 1\) pada elemen kartu untuk mensimulasikan efek inersia. Menambahkan custom scrollbar minimalis.

### **Review**

- \[✅\] Sesuai constraints?
- \[✅\] Format sesuai?
- \[✅\] Bisa dipahami?
- Changes: Penggunaan will-change: transform untuk optimasi performa rendering saat scrolling.

## **Step 4: Sticky Navbar & ID Navigation**

### **Prompt**

buatkan navbar dan lakukan scrool behavior berupa smooth scrools ketika klik navbar atau side bar tersebut.

### **RTCC-O Check**

- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### **AI Response**

Implementasi \<nav\> dengan efek glassmorphism. Menambahkan scroll-margin-top pada setiap section agar judul tidak terpotong oleh navbar saat melakukan navigasi internal (anchor links).

### **Review**

- \[✅\] Sesuai constraints?
- \[✅\] Format sesuai?
- \[✅\] Bisa dipahami?
- Changes: Menambahkan padding pada body untuk mengompensasi tinggi fixed navbar.
