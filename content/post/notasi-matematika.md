---
author: Diah Komala
title: Notasi Matematika
date: 2020-06-01
description: Panduan singkat untuk mengatur KaTeX
tags : ["matematika","hugo"]
math: true
---

Notasi matematika dalam web proyek Hugo dapat diaktifkan dengan menggunakan JavaScript libraries pihak ketiga.
<!--more-->

Dalam contoh ini kita akan menggunakan [KaTeX](https://katex.org/)

- Buatlah sebuah file parisal di dalam `/layouts/partials/math.html`;
- Dengan file parisal ini merujuk ke [Auto-render Extension](https://katex.org/docs/autorender.html) atau host skrip ini secara lokal;
- Sertakan parsial dalam template anda seperti ini :  

```
{{ if or .Params.math .Site.Params.math }}
{{ partial "math.html" . }}
{{ end }}
```  
- Untuk mengaktifkan KaTex secara global, atur parameter `math` ke` true` dalam konfigurasi proyek;
- Untuk mengaktifkan KaTex pada basis per halaman sertakan parameter `math: true` dalam file konten.

**Catatan:** Gunakan referensi online dari [Supported TeX Functions](https://katex.org/docs/supported.html)


### Contoh
{{< math.inline >}}
<p>
Baris simbol matematika: \(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\)
</p>
{{</ math.inline >}}

Baris simbol matematika :
$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$

