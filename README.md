# netics-deployment

| Nama           | NRP        | 
| ---            | ---        | 
|Nathanael Oliver Amadhika Yuswana|5025241109|

## Penjelasan
### Soal 1
Pada soal nomor 1, saya memahami dan mempelajari mengenai API publik melalui AI Gemini. Saya mempelajari cara membuat struktur kode untuk API dengan NodeJS melalui bantuan Gemini. Saya memodifikasi kode yang diberikan oleh Gemini menyesuaikan kebutuhan pada soal 1, di mana API-nya akan memiliki endpoint /health. Untuk kode dari API-nya adalah sebagai berikut:

`api.js`
```
const express = require('express');
const app = express();
const port = 3000;

app.use(express.json());

app.get('/health', (req, res) => {
    res.status(200).json({
        "nama": "Nathanael Oliver Amadhika Yuswana",
        "nrp": "5025241109",
        "status": "UP",
        "timestamp": new Date(),
        "uptime": process.uptime()
    });
});

app.listen(port);
```

- Di awal kode, program mengimport library express dan memastikan server bisa membaca file berformat JSON. Port yang digunakan pada program adalah port 3000. Seperti yang diminta pada soal, data API yang berisi nama, nrp, dan lain-lain dimasukkan pada endpoint /health. Terakhir, server akan melakukan _listen_ pada koneksi yang masuk untuk memberikan respons yang berisi data API-nya jika koneksi berhasil terhubung. 

Untuk history chat dengan Gemini dapat diakses pada link berikut: https://gemini.google.com/share/79b5e33514d1
