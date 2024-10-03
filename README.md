# Tmux Temel Kullanım Rehberi

## İçindekiler

1. [Tmux Nedir?](#tmux-nedir)
2. [Kurulum](#kurulum)
3. [Temel Komutlar](#temel-komutlar)
4. [Oturumlar (Sessions)](#oturumlar-sessions)
5. [Pencereler (Windows)](#pencereler-windows)
6. [Bölmeler (Panes)](#bölmeler-panes)
7. [Kaydırma-Kopyalama Modu](#kopyalama-modu)

## Tmux Nedir?

Tek bir terminal penceresinde birden fazla terminal oturumu oluşturmanıza, bunlar arasında geçiş yapmanıza ve bunları yönetmenize olanak tanıyan bir araçtır. Screen kullanımından sonra tmux'un pratik yapısına çok kısa sürede alışacaksınız.
Basitçe anlamak için 3 katmandan bahsedebiliriz.
<br>Oturumlar > Pencereler > Bölmeler

## Kurulum

- Ubuntu/Debian: `sudo apt-get install tmux`

## Temel Komutlar

- Tmux'u başlatmak: `tmux`  (Oturum başlatır.)
- Son Tmux'a geri dönmek: `tmux a`  (Son oturuma girer.)
- Her tuşlama öncesi (Prefix): `Ctrl+b` bas ve bırak, işlev tuşuna basabilirsin.
- Tmux'tan çıkmak (Oturum Detach): `Ctrl+b  d`

## Pencereler (Windows)

- Yeni pencere oluşturmak: `Ctrl+b  c`
- Pencereler arası geçiş: `Ctrl+b  0-9` veya `Ctrl+b  n` (sonraki) / `Ctrl+b  p` (önceki)
- Pencereyi yeniden adlandırmak: `Ctrl+b  ,`
- Oturum ve pencerelerin tümüne kolay erişim: `Ctrl+b  w`

## Bölmeler (Panes)

- Dikey bölme: `Ctrl+b  %`
- Yatay bölme: `Ctrl+b  "`
- Bölmeler arası geçiş: `Ctrl+b  Yön Tuşları`
- Bölmeleri boyutlandırma: `Ctrl+b  Ctrl+Yön Tuşları` veya daha uzun adımlarla boyutlandırmak için `Alt+Yön Tuşları`
- Bölmeleri standart boyutlara oranla:  `Ctrl+b  Space`
- Bölmeyi yok et: `Ctrl+b  x` y veya n sorar.

 ## Oturumlar (Sessions)
### Bu adım basitçe "tmux" yazıp başlatmak ve "tmux a" ile son başlatılmış oturuma dönme pratikliğine ters. Katmanları anlamak için kalabilir.
- Yeni oturum oluşturmak: `tmux new -s oturum_adı`
- Oturumları listelemek: `tmux ls`
- Oturumdan ayrılmak: `Ctrl+b  d`

## Kaydırma-Kopyalama Modu

- Kaydırma ve kopyalama moduna girmek: `Ctrl+b  [`  (Tekerlek ve Page Up/Down)


