# get_open_graph_facebook
Mengambil data facebook graph berdasarkan url web dengan php



## Apa itu openGraph atau yang sering dikenal dengan OG Facebook :

OpenGraph merupakan OG meta yang dibuat oleh facebook untuk keperluan share artikel melalui facebook, dengan kata lain ketika kamu melakukan share link maka akan terlihat gambar, judul, description dan lainnya, data itu semua umumnya bisa hanya dengan menggunakan meta biasa, namun lebih baik lagi jika kita menggunakan OpenGraph dari Facebook dalam meta web yang kita gunakan.



![OpenGraph](https://www.dropbox.com/s/glzsnl6xxa3n4ov/opengraph_facebook.PNG?raw=1)



Seperti gambar diatas yang saya berikan lingkaran merah merupakan data yang didapat dari OpenGraph Facebook yang telah kita setting pada meta web kita.



## Lalu bagaimana cara memasangnya ?

Mungkin disini teman-teman bisa mencarinya melalui Google dengan Keyword "Cara Memasang OG Meta Facebook Pada Web"



Cara mendapatkan data opengraph facebook dengan php

Nah dengan adanya opengraph kita juga bisa mengambil data yang ada pada opengraph facebook dengan cara seperti yang ada pada file berikut ini :

[get_data_facebook_open_graph](https://github.com/kangyasin/get_open_graph_facebook/blob/master/get_data_facebook_open_graph.md)



Hasil akhirnya akan berbentuk array(); dan kalian hanya tinggal menyusun hasil array tersebut sesuai dengan kebutuhan yang dibutuhkan.



```markdown
Array
(
    [locale] => en_US
    [type] => article
    [title] => Kang Yasin - Fotografi: Memilih "Kamera" Handphone untuk Fotografi
    [description] => Kang Yasin - Fotografi: Memilih "Kamera" Handphone untuk Fotografi
    [url] => http://www.kangyasin.com/2017/12/memilih-kamera-handphone-untuk-fotografi.html
    [site_name] => kangyasin.com
    [updated_time] => 2018-03-21T1506:54:44+07:00
    [image] => https://3.bp.blogspot.com/-M8Slu_ZO8h0/Wi6GKTYyruI/AAAAAAAAMic/kjgDDP7ltGYPdJU7As33u2-iiWMTtOiowCEwYBhgL/s320/iphone5s%2Bkangyasincom%2Bbliblicom.PNG
    [image:secure_url] => https://3.bp.blogspot.com/-M8Slu_ZO8h0/Wi6GKTYyruI/AAAAAAAAMic/kjgDDP7ltGYPdJU7As33u2-iiWMTtOiowCEwYBhgL/s320/iphone5s%2Bkangyasincom%2Bbliblicom.PNG
    [image:width] => 320
    [image:height] => 320
)
```



Terima kasih.

[^]: Jurnal Web http://www.jurnalweb.com/demo/php/og.php

