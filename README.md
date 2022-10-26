Coding hitung php
 
 
<form method="GET" action="hasil_hitung.php">
Nilai y : <input type="text" name="a"><br><br>
Nilai x : <input type="text" name="b"><br><br>
Operasi : <br>
<input type="radio" name="operasi" value="jumlah">Penjumlahan<br>
<input type="radio" name="operasi" value="kurang">Pengurangan<br>
<input type="radio" name="operasi" value="kali">Perkalian<br>
<input type="radio" name="operasi" value="bagi">Pembagian<br><br>
<input type="submit" value="Hitung">
</form>
 
 
Coding hasil hitung php
 
<?php
$a       = $_GET['a'];
$b       = $_GET['b'];
$operasi = $_GET['operasi'];
 
echo "Nilai y : $a<br>";
echo "Nilai x : $b<br><br>";
 
if ($operasi=="jumlah"){
  $c = $a + $b; // rumus penjumlahan
  echo "Penjumlahan $a + $b = $c";
}
elseif ($operasi=="kurang"){
  $c = $a - $b; // rumus pengurangan
  echo "Pengurangan $a - $b = $c";
}
elseif ($operasi=="kali"){
  $c = $a * $b; // rumus perkalian
  echo "Perkalian $a x $b = $c";
}
elseif ($operasi=="bagi"){
  $c = $a / $b; // rumus pembagian
  echo "Pembagian $a / $b = $c";
}
// apabila operasi perhitungan belum dipilih
else{
  echo "Anda belum memilih operasi perhitungan";
}
?>
 
Coding hitung python
 
n= int(input('ketik jumlah obyek: '))
r= int(input('ketik jumlah urutan: '))
kombinasi=1
for x in range (kombinasi,n-1):
 kombinasi=kombinasi*x
a=kombinasi
b=n-r
kombinasi=1
for x in range (kombinasi,b-1):
 kombinasi=kombinasi*x
 c=kombinasi
 permutasi=a/c
 print('permutasi dari sejumlah ',n,' obyek dengan urutan sebanyak ',r,' adalah:',permutasi)
