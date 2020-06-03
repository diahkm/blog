+++
author = "Diah Komala"
title = "Dukungan Emoji"
date = "2020-05-25"
description = "Panduan untuk penggunaan emoji di Hugo"
tags = [
    "emoji",
	"hugo",
]
+++

Emoji dapat diaktifkan dalam proyek Hugo dalam beberapa cara.
<!--more-->
Fungsi [`emojify`](https://gohugo.io/functions/emojify/) dapat dipanggil langsung di templat atau dengan [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

Untuk mengaktifkan emoji secara global, setel `enableEmoji` ke `true` dalam [konfigurasi situs](https://gohugo.io/getting-started/configuration/) anda dan kemudian anda bisa mengetikkan kode emoji secara langsung dalam file konten, misalnya :

:see_no_evil : :see_no_evil: :speak_no_evil : :speak_no_evil: :hear_no_evil : :hear_no_evil:

[Lembar cheat Emoji](http://www.emoji-cheat-sheet.com/) adalah referensi yang berguna untuk kode emoji.

***

**N.B.** Langkah-langkah di atas memungkinkan karakter dan urutan emoji Unicode Standard dalam Hugo, namun rendering `glyphs` ini tergantung pada browser dan platform. Untuk gaya emoji Anda dapat menggunakan font emoji pihak ketiga atau font stack, misalnya : 

{{< highlight html >}}
.emoji {
	font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
}
{{< /highlight >}}
