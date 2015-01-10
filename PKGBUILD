pkgver='20131028'
url='https://github.com/seebi/tmux-colors-solarized'
license=('MIT')
depends=('tmux')
conflicts=('tmux-solarized-git')
source=('git+https://github.com/seebi/tmux-colors-solarized#commit=8d9edb6')

build() {
	cd 'tmux-colors-solarized'
	mv 'tmuxcolors-256.conf' 'solarized-256.conf'
	mv 'tmuxcolors-light.conf' 'solarized-light.conf'
	mv 'tmuxcolors-dark.conf' 'solarized-dark.conf'
}

package() {
	cd 'tmux-colors-solarized'
	install -Dm644 -t "$pkgdir/usr/share/tmux" *.conf
}
