# Golang Modules

## Sebelum Ada Go Modules

- Saat kita membuat aplikasi, biasanya kita akan menggunakan library atau dependency dari project lain.
- Sebelum ada Go Modules, management untuk dependency sangat sulit dilakukan di Go-Lang.
- Biasanya kita akan meng-copy semua source code library atau dependency lain ke project kita, hal ini membuat project kita menjadi bengkak karena penuh dengan library orang lain.
- Atau biasanya library orang lain akan kita save di GOPATH directory, namun hal ini akan sulit jika ternyata beberapa aplikasi butuh library yang sama dengan versi yang berbeda

## Go-modules

- Go-Modules mulai dikenalkan di Go-lang 1.11 and 1.12
- Dengan Go-Modules, kita bisa membuat project dengan mudah dan dependency management yang sangat mudah

### Membuat modules

**Teringegrasi oleh git :**

```
go mod init namamodule
```

**Jalankan perintah berikut di terminal :**

```
go mod init github.com/ilhambonardoo/golang-modules
```

**Kalo mau melakukan major update jalankan perintah berikut :**

```
go mod init github.com/ilhambonardoo/golang-modules/v2
```

### Membuat rilis

**Jalankan perintah berikut di terminal :**

```
git tag v1.0.0
git push origin v1.0.0
```
