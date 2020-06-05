+++
author = "Diah Komala"
title = "Panduan Sintaks Markdown"
date = "2020-06-03"
description = "Sintaks dasar markdown dan format elemen HTML."
tags = [
    "markdown",
    "css",
    "html",
	  "hugo",
]
+++

Contoh sintaks Markdown dasar yang dapat digunakan dalam file konten Hugo, juga menunjukkan apakah elemen HTML dasar didekorasi dengan CSS dalam tema Hugo.
<!--more-->

## Headings

Elemen HTML `<h1>` —` <h6> `berikut ini mewakili enam tingkat judul bagian. `<h1>` adalah tingkat bagian tertinggi sedangkan `<h6>` adalah yang terendah.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Paragraf

Jangan membenci siapapun, tidak peduli berapa banyak mereka bersalah padamu. Hiduplah dengan rendah hati, tidak peduli seberapa kekayaanmu. Berpikirlah positif, tidak peduli seberapa keras kehidupanmu. Berikanlah banyak, meskipun menerima sedikit. Tetaplah berhubungan dengan orang-orang yang telah melupakanmu, dan ampuni yang bersalah padamu. Jangan berhenti berdoa untuk yang terbaik bagi orang yang kau cintai.

Tiada kekayaan lebih utama daripada akal. Tiada kepapaan lebih menyedihkan daripada kebodohan. Tiada warisan yang lebih baik daripada pendidikan. Dan tiada pembantu yang lebih baik daripada musyawarah.

Lidah orang yang berakal berada di belakang hatinya, sedangkan hati orang bodoh berada di belakang lidahnya.

## Blockquotes

Elemen blockquote mewakili konten yang dikutip dari sumber lain, secara opsional dengan kutipan yang harus berada di dalam elemen `footer` atau` cite`, dan secara opsional dengan perubahan sebaris seperti anotasi dan singkatan.

#### Blockquote tanpa atribusi

> Nafas itu lebih pendek dari rindu, rindu lebih purba dari nafas. Maka, rindu tidak pernah berakhir bila nafas behenti.
> **Catatan** bahwa anda dapat menggunakan *sintaks Markdown* dalam blockquote.

#### Blockquote dengan atribusi

> Rindu bukanlah persoalan, ia adalah jawaban yang belum selesai, bahkan tak harus.
> — <cite>Rocky Gerung[^1]</cite>


[^1]: Kutipan di atas dikutip dari [twitter](https://twitter.com/rockygerung/status/941337724849496064?lang=en) Rocky Gerung pada tanggal 14 Desember 2017.

## Tabel

Tabel bukan bagian dari core Markdown spec, tetapi dukungan Hugo mendukung itu out-of-the-box.

   Name | Age
--------|------
   Mala | 27
  Fuady | 23

#### Inline Markdown di dalam tabel

| Inline&nbsp;&nbsp;&nbsp;     | Markdown&nbsp;&nbsp;&nbsp;  | In&nbsp;&nbsp;&nbsp;                | Table      |
| ---------- | --------- | ----------------- | ---------- |
| *italics*  | **bold**  | ~~strikethrough~~&nbsp;&nbsp;&nbsp; | `code`     |

## Blok kode

#### Blok kode dengan backticks

```
html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```
#### Blok kode indentasi dengan empat spasi

    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Blok kode dengan Hugo shortcode 
{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## Tipe List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Elemen lainya — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> format gambar bitmap.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.