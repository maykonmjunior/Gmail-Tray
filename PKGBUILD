# Maintainer: Maykon Marcos Junior <maykonmjunior@gmail.com>
pkgname=gmail-tray
pkgver=1.0
pkgrel=1
pkgdesc="Minimal Gmail tray notifier with unread counter"
arch=('any')
url="https://github.com/maykonmjunior/gmail-tray"
license=('MIT')
depends=('dunst' 'fetchmail' 'gtk3' 'libappindicator-gtk3' 'libnotify' 'python' 'python-gobject')
source=('gmail-tray.py' 'gmail-tray.desktop' 'gmail-tray.service' 'gmail.png')
sha256sums=('SKIP'  # gmail-tray.py
            'SKIP'  # gmail-tray.desktop
            'SKIP'  # gmail-tray.service
            'SKIP') # gmail.png
install=
package() {
  install -Dm755 "$srcdir/gmail-tray.py" "$pkgdir/usr/bin/gmail-tray"
  install -Dm644 "$srcdir/gmail-tray.desktop" "$pkgdir/usr/share/applications/gmail-tray.desktop"
  install -Dm644 "$srcdir/gmail-tray.service" "$pkgdir/usr/lib/systemd/user/gmail-tray.service"
  install -Dm644 "$srcdir/gmail.png" "$pkgdir/usr/share/icons/hicolor/48x48/apps/gmail-tray.png"
}
