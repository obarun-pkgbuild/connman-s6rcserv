# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=connmand-s6rcserv
pkgver=0.1
pkgrel=2
pkgdesc="connmand service for"
arch=(x86_64)
license=('beerware')
depends=('connman' 's6' 's6-rc' 's6-boot')
conflicts=()
source=('connmand.longrun.dependencies'
		'connmand.longrun.pipeline-name'
		'connmand.longrun.producer-for'
		'connmand.longrun.run'	
		'connmand.longrun.type'		
		'connmand.log.consumer-for'
		'connmand.log.dependencies'
		'connmand.log.run'
		'connmand.log.type'
		'connman-vpnd.longrun.dependencies'
		'connman-vpnd.longrun.pipeline-name'
		'connman-vpnd.longrun.producer-for'
		'connman-vpnd.longrun.run'	
		'connman-vpnd.longrun.type'		
		'connman-vpnd.log.consumer-for'
		'connman-vpnd.log.dependencies'
		'connman-vpnd.log.run'
		'connman-vpnd.log.type'
		'bundle.connman.contents'
		'bundle.connman.type'
		'connmand.logd'
		'LICENSE')
md5sums=('68b329da9893e34099c7d8ad5cb9c940'
         '1814bac8bf27060ec214d912b486ad33'
         '68290b3ae7c0e7b4c681f08e6aec2964'
         '0855f4616b4fcd62037acfbe35b2e1f9'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         'bd3505d7df3aeadcd29a17b56125ab1c'
         '68b329da9893e34099c7d8ad5cb9c940'
         'f6bda00945d08fe7abf5555f203f92fc'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '68b329da9893e34099c7d8ad5cb9c940'
         'ca1e21037cfc26995b800edaafbf4d76'
         'b7b622cf29ee66326bc638b8c647b2b6'
         'de7a76844218eeba406ccdcf3ee71f9f'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         'bfc022bcf77ac8eedc430b22f3ea6059'
         '68b329da9893e34099c7d8ad5cb9c940'
         '2a0d9b54e2d8ac882fae2c66836cd036'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '3617965975f8d2b3a3c49b9f6298d48f'
         '71abe97e2554d37f1d12c5bf4945297f'
         '47910c2c6d7376793219166010fe43fa'
         '191a37ae657aa17e37e75d0242865dba')

package() {
	
	# bundle , trouble here user-connmand need a maj at connmand e.g user-Base
	install -Dm 0644 "$srcdir/bundle.connman.contents" "$pkgdir/etc/s6-serv/available/rc/bundle-Connman/contents"
	install -Dm 0644 "$srcdir/bundle.connman.type" "$pkgdir/etc/s6-serv/available/rc/bundle-Connman/type"
	
	# longrun connmand
	install -Dm 0644 "$srcdir/connmand.longrun.dependencies" "$pkgdir/etc/s6-serv/available/rc/connmand-longrun/dependencies"
	install -Dm 0644 "$srcdir/connmand.longrun.pipeline-name" "$pkgdir/etc/s6-serv/available/rc/connmand-longrun/pipeline-name"
	install -Dm 0644 "$srcdir/connmand.longrun.producer-for" "$pkgdir/etc/s6-serv/available/rc/connmand-longrun/producer-for"
	install -Dm 0644 "$srcdir/connmand.longrun.run" "$pkgdir/etc/s6-serv/available/rc/connmand-longrun/run"
	install -Dm 0644 "$srcdir/connmand.longrun.type" "$pkgdir/etc/s6-serv/available/rc/connmand-longrun/type"
	
	# longrun connman-vpnd
	install -Dm 0644 "$srcdir/connman-vpnd.longrun.dependencies" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-longrun/dependencies"
	install -Dm 0644 "$srcdir/connman-vpnd.longrun.pipeline-name" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-longrun/pipeline-name"
	install -Dm 0644 "$srcdir/connman-vpnd.longrun.producer-for" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-longrun/producer-for"
	install -Dm 0644 "$srcdir/connman-vpnd.longrun.run" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-longrun/run"
	install -Dm 0644 "$srcdir/connman-vpnd.longrun.type" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-longrun/type"
	
	# log connmand
	install -Dm 0644 "$srcdir/connmand.log.consumer-for" "$pkgdir/etc/s6-serv/available/rc/connmand-log/consumer-for"
	install -Dm 0644 "$srcdir/connmand.log.dependencies" "$pkgdir/etc/s6-serv/available/rc/connmand-log/dependencies"
	install -Dm 0644 "$srcdir/connmand.log.run" "$pkgdir/etc/s6-serv/available/rc/connmand-log/run"
	install -Dm 0644 "$srcdir/connmand.log.type" "$pkgdir/etc/s6-serv/available/rc/connmand-log/type"
	
	# log connman-vpnd
	install -Dm 0644 "$srcdir/connman-vpnd.log.consumer-for" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/consumer-for"
	install -Dm 0644 "$srcdir/connman-vpnd.log.dependencies" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/dependencies"
	install -Dm 0644 "$srcdir/connman-vpnd.log.run" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/run"
	install -Dm 0644 "$srcdir/connman-vpnd.log.type" "$pkgdir/etc/s6-serv/available/rc/connman-vpnd-log/type"
	
	# hook
	install -Dm 0644 "$srcdir/connmand.logd" "$pkgdir/etc/s6-serv/log.d/connmand-rc"
	
	install -Dm 0644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/connmand-s6rcserv/LICENSE"
}
