Gravatar - Mencari email aktif melalui gambar.

Deteksi warna gambar : https://github.com/humanmade/Colors-Of-Image

```
include_once( 'colorsofimage.class.php' );
$image = new ColorsOfImage( 'https://www.gravatar.com/avatar/'.md5('users@example.com') );
$colors = $image->getProminentColors(); 
print_r($colors);

hasil email tidak terdaftar : 

Array
(
    [0] => #0066CC
)

hasil email yang terdaftar :

Array
(
    [0] => #CCCCCC
    [1] => #424153
    [2] => #000000
)
```

kita anggap #0066CC sebagai warna email yang tidak terdaftar di Gravatar. sedangkan jika muncul lebih dari 1 hasil maka kita Anggap pengguna terdaftar di Gravatar.
perlu diperhatikan bahwa tidak semua pengguna Gravatar Mengganti avatar.
