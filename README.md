# Tmux Kullanım Rehberi

## İçindekiler

1. [Tmux Nedir?](#tmux-nedir)
2. [Kurulum](#kurulum)
3. [Temel Komutlar](#temel-komutlar)
4. [Oturumlar (Sessions)](#oturumlar-sessions)
5. [Pencereler (Windows)](#pencereler-windows)
6. [Bölmeler (Panes)](#bölmeler-panes)
7. [Kaydırma-Kopyalama Modu](#kopyalama-modu)

## Tmux Nedir?

Tmux, tek bir terminal penceresinde birden fazla terminal oturumu oluşturmanıza, bunlar arasında geçiş yapmanıza ve bunları yönetmenize olanak tanıyan bir araçtır. Screen kullanımından sonra tmux'un pratik yapısına çok kısa sürede alışacaksınız.

## Kurulum

- Ubuntu/Debian: `sudo apt-get install tmux`

## Temel Komutlar

- Tmux'u başlatmak: `tmux`
- Son Tmux'a geri dönmek: `tmux a`
- Her tuşlama öncesi: `Ctrl+b` tuşları bırak. 
- Tmux'tan çıkmak: `exit` veya `Ctrl+d`

## Oturumlar (Sessions)

- Yeni oturum oluşturmak: `tmux new -s oturum_adı`
- Oturumları listelemek: `tmux ls`
- Oturuma bağlanmak: `tmux attach -t oturum_adı`
- Oturumdan ayrılmak: `Prefix d`

## Pencereler (Windows)

- Yeni pencere oluşturmak: `Prefix c`
- Pencereler arası geçiş: `Prefix 0-9` veya `Prefix n` (sonraki) / `Prefix p` (önceki)
- Pencereyi yeniden adlandırmak: `Prefix ,`

## Bölmeler (Panes)

- Dikey bölme: `Prefix %`
- Yatay bölme: `Prefix "`
- Bölmeler arası geçiş: `Prefix ok tuşları`
- Bölmeyi kapatmak: `Prefix x`

## Kopyalama Modu

- Kopyalama moduna girmek: `Prefix [`
- Metin seçmek: `Space` ile başla, `Enter` ile bitir
- Yapıştırmak: `Prefix ]`

