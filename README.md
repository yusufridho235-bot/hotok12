// 1. Membuat array berisi angka acak
let angka = [];

for (let i = 0; i < 10; i++) {
    angka.push(Math.floor(Math.random() * 100) + 1);
}

console.log("1. Angka acak:");
console.log(angka);

// 2. Mengurutkan dari terbesar ke terkecil
let terbesar = [...angka].sort((a, b) => b - a);

console.log("2. Terbesar ke terkecil:");
console.log(terbesar);

// 3. Mengurutkan dari terkecil ke terbesar
let terkecil = [...angka].sort((a, b) => a - b);

console.log("3. Terkecil ke terbesar:");
console.log(terkecil);

// 4. Menjumlahkan semua angka
let jumlah = angka.reduce((total, nilai) => total + nilai, 0);

console.log("4. Jumlah semua angka:");
console.log(jumlah);

// 5. Menampilkan angka genap saja
let genap = angka.filter(nilai => nilai % 2 === 0);

console.log("5. Angka genap saja:");
console.log(genap);
