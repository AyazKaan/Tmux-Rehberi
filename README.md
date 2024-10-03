# Tmux Kullanım Rehberi

Tmux, terminal multiplexer olarak bilinen güçlü bir araçtır. Bu rehber, tmux'un temel kullanımını ve bazı yararlı ipuçlarını içermektedir.

## İçindekiler

1. [Tmux Nedir?](#tmux-nedir)
2. [Kurulum](#kurulum)
3. [Temel Komutlar](#temel-komutlar)
4. [Oturumlar (Sessions)](#oturumlar-sessions)
5. [Pencereler (Windows)](#pencereler-windows)
6. [Bölmeler (Panes)](#bölmeler-panes)
7. [Kopyalama Modu](#kopyalama-modu)
8. [Tmux Yapılandırması](#tmux-yapılandırması)
9. [İpuçları ve Püf Noktaları](#ipuçları-ve-püf-noktaları)

## Tmux Nedir?

Tmux, tek bir terminal penceresinde birden fazla terminal oturumu oluşturmanıza, bunlar arasında geçiş yapmanıza ve bunları yönetmenize olanak tanıyan bir araçtır.

## Kurulum

Tmux'u kurmak için:

- Ubuntu/Debian: `sudo apt-get install tmux`
- macOS (Homebrew): `brew install tmux`
- Fedora: `sudo dnf install tmux`

## Temel Komutlar

- Tmux'u başlatmak: `tmux`
- Prefix tuşu: `Ctrl+b` (varsayılan)
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

## Tmux Yapılandırması

Tmux'u özelleştirmek için `~/.tmux.conf` dosyasını kullanabilirsiniz. Örnek:
