
pkgname=stormos-installer
pkgver=1.0.1
pkgrel=1
pkgdesc="Command line installer for StormOS for expert users."
arch=('any')
url="https://github.com/bfitzgit23/stormos-installer"
license=('GPL3')
depends=('alacritty' 'dialog' 'wipe')
source=(
		abif
		abif.desktop
		alacritty.toml
		dutch.trans
		english.trans
		french.trans
		hungarian.trans
		italian.trans
		portuguese.trans
		portuguese_brasil.trans
		russian.trans
		spanish.trans)
sha256sums=('a75d908ed5ad1e0059791e42dff440d92ef02741f273118d2a3f765e47ef06d8'
            '9fdb1fcab922486d72ad3f6110c65a83952c75e09fe2de98618a6fe2b0fd3df7'
            '376cf5e4e10db59cb8c2c799c651d6cee756d16451c34e410ef50034bea2210a'
            '62fbb7fa46bc724bf1a2de88361e8257503551ab0b472643ce9cdddd1079185f'
            '4881e9576968070ace22d20aa2773d59997a3ab847e66824858dfe3d3dc88596'
            'ba58c00b7b026fa1cee1fdcf592549a6ad88e795d0120cd67861c0dddfd2aff1'
            '28f59663beaa55e166e0849a0b4564322fc5c82f39e59665a0bb40cb9d3a59f9'
            'a3c0c8c8ca304912e65ece7f00cbf9f41fa441db1b24d8862744a95cf594b8a5'
            '3f4a0c4ad0901767279c8f43fc6bc42f771edc15fe999059da6e96537b091c8b'
            '2d5732b753d3e438171b2a4699fea0eb579b7e2a529ebf3380c438b90d2a4935'
            '5b4965a3f012f32445318dd1ba59bc3a7b245557a6692f08d168162f751cfe34'
            '0eef8929f34731c00fd77cc21063379715ba8f456e224b99f5dc463cd147df3f')

package() {
	local _idir="${pkgdir}/abif-master"
	mkdir -p "$_idir"

	install -Dm 755 abif 					"$_idir"/abif
	install -Dm 644 alacritty.toml 			"$_idir"/alacritty.toml
	install -Dm 644 dutch.trans 			"$_idir"/dutch.trans
	install -Dm 644 english.trans 			"$_idir"/english.trans
	install -Dm 644 french.trans 			"$_idir"/french.trans
	install -Dm 644 hungarian.trans 		"$_idir"/hungarian.trans
	install -Dm 644 italian.trans 			"$_idir"/italian.trans
	install -Dm 644 portuguese.trans 		"$_idir"/portuguese.trans
	install -Dm 644 portuguese_brasil.trans "$_idir"/portuguese_brasil.trans
	install -Dm 644 russian.trans 			"$_idir"/russian.trans
	install -Dm 644 spanish.trans 			"$_idir"/spanish.trans

	install -Dm 644 abif.desktop 			-t "$pkgdir"/usr/share/applications
}
