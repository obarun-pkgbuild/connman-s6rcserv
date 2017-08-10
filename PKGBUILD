# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=connmand-s6rcserv
pkgver=0.1
pkgrel=1
pkgdesc="connmand service for s6"
arch=(x86_64)
license=('beerware')
depends=('connman' 's6' 's6-rc' 's6-boot')
conflicts=()
install=connman-s6rcserv.install
source=('connmand.daemon.dependencies.s6'
		'connmand.daemon.pipeline-name.s6'
		'connmand.daemon.producer-for.s6'
		'connmand.daemon.run.s6'	
		'connmand.daemon.type.s6'		
		'connmand.log.consumer-for.s6'
		'connmand.log.dependencies.s6'
		'connmand.log.run.s6'
		'connmand.log.type.s6'
		'connman-vpnd.daemon.dependencies.s6'
		'connman-vpnd.daemon.pipeline-name.s6'
		'connman-vpnd.daemon.producer-for.s6'
		'connman-vpnd.daemon.run.s6'	
		'connman-vpnd.daemon.type.s6'		
		'connman-vpnd.log.consumer-for.s6'
		'connman-vpnd.log.dependencies.s6'
		'connman-vpnd.log.run.s6'
		'connman-vpnd.log.type.s6'
		'bundle.connman.contents.s6'
		'bundle.connman.type.s6'
		'LICENSE')
md5sums=('68b329da9893e34099c7d8ad5cb9c940'
         '1814bac8bf27060ec214d912b486ad33'
         '68290b3ae7c0e7b4c681f08e6aec2964'
         '0855f4616b4fcd62037acfbe35b2e1f9'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '5ba4b6c504b64f1eb73dae008089f448'
         '68b329da9893e34099c7d8ad5cb9c940'
         'f6bda00945d08fe7abf5555f203f92fc'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '68b329da9893e34099c7d8ad5cb9c940'
         'ca1e21037cfc26995b800edaafbf4d76'
         'b7b622cf29ee66326bc638b8c647b2b6'
         'de7a76844218eeba406ccdcf3ee71f9f'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         'eb79efce39ab665207574405f239f352'
         '68b329da9893e34099c7d8ad5cb9c940'
         '2a0d9b54e2d8ac882fae2c66836cd036'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '3e65fdd223cc419f219b6ed9e03615b1'
         '71abe97e2554d37f1d12c5bf4945297f'
         '191a37ae657aa17e37e75d0242865dba')

package() {
	
	# bundle , trouble here user-connmand need a maj at connmand e.g user-Base
	install -Dm 0644 "$srcdir/bundle.connman.contents.s6" "$pkgdir/etc/s6-serv/available/rc/bundle-Connman/contents"
	install -Dm 0644 "$srcdir/bundle.connman.type.s6" "$pkgdir/etc/s6-serv/available/rc/bundle-Connman/type"
	
	# daemon connmand
	install -Dm 0644 "$srcdir/connmand.daemon.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-daemon/dependencies"
	install -Dm 0644 "$srcdir/connmand.daemon.pipeline-name.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-daemon/pipeline-name"
	install -Dm 0644 "$srcdir/connmand.daemon.producer-for.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-daemon/producer-for"
	install -Dm 0644 "$srcdir/connmand.daemon.run.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-daemon/run"
	install -Dm 0644 "$srcdir/connmand.daemon.type.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-daemon/type"
	
	# daemon connman-vpnd
	install -Dm 0644 "$srcdir/connman-vpnd.daemon.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-daemon/dependencies"
	install -Dm 0644 "$srcdir/connman-vpnd.daemon.pipeline-name.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-daemon/pipeline-name"
	install -Dm 0644 "$srcdir/connman-vpnd.daemon.producer-for.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-daemon/producer-for"
	install -Dm 0644 "$srcdir/connman-vpnd.daemon.run.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-daemon/run"
	install -Dm 0644 "$srcdir/connman-vpnd.daemon.type.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-daemon/type"
	
	# log connmand
	install -Dm 0644 "$srcdir/connmand.log.consumer-for.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-log/consumer-for"
	install -Dm 0644 "$srcdir/connmand.log.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-log/dependencies"
	install -Dm 0644 "$srcdir/connmand.log.run.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-log/run"
	install -Dm 0644 "$srcdir/connmand.log.type.s6" "$pkgdir/etc/s6-serv/available/rc/connmand-log/type"
	
	# log connman-vpnd
	install -Dm 0644 "$srcdir/connman-vpnd.log.consumer-for.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/consumer-for"
	install -Dm 0644 "$srcdir/connman-vpnd.log.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/dependencies"
	install -Dm 0644 "$srcdir/connman-vpnd.log.run.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/run"
	install -Dm 0644 "$srcdir/connman-vpnd.log.type.s6" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/type"
	
	install -Dm 0644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/connmand-s6rcserv/LICENSE"
}
