# netics-deployment

| Nama           | NRP        | 
| ---            | ---        | 
|Nathanael Oliver Amadhika Yuswana|5025241109|

## Penjelasan
### Soal 1
Pada soal nomor 1, saya memahami dan mempelajari mengenai API publik melalui AI Gemini. Saya mempelajari cara membuat struktur kode untuk API dengan NodeJS melalui bantuan Gemini. Saya memodifikasi yang diberikan oleh Gemini menyesuaikan kebutuhan pada soal 1, di mana API-nya akan memiliki endpoint /health. Untuk kode dari API-nya adalah sebagai berikut:
`app.js`
```
const express = require('express');
const app = express();
const port = 32;

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
