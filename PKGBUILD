# Maintainer: Daniel Spies <daniel dot spies at fuceekay dot com>

pkgname=google-gson
pkgver=2.2.4
pkgrel=1
pkgdesc='Java library to convert Java Objects into JSON and back'
arch=('i686' 'x86_64')
url='http://code.google.com/p/google-gson/'
license=('APACHE')
depends=('java-runtime')
source=("http://google-gson.googlecode.com/files/${pkgname}-${pkgver}-release.zip")
#md5sums=('046bbaa4779cdcf47f332bfdfdea7ad7')
sha1sums=('1e8d308e075683d8f963cf5ea6aef7b9d3763cb2')

package() {
    install -d -m755 ${pkgdir}/usr/share/java/${pkgname}/
    install -m755 \
        ${srcdir}/${pkgname}-${pkgver}/gson-${pkgver}.jar \
        ${pkgdir}/usr/share/java/${pkgname}/${pkgname}-${pkgver}.jar
    install -m755 \
        ${srcdir}/${pkgname}-${pkgver}/gson-${pkgver}-sources.jar \
        ${pkgdir}/usr/share/java/${pkgname}/${pkgname}-${pkgver}-sources.jar
    install -m755 \
        ${srcdir}/${pkgname}-${pkgver}/gson-${pkgver}-javadoc.jar \
        ${pkgdir}/usr/share/java/${pkgname}/${pkgname}-${pkgver}-javadoc.jar
    ln -s /usr/share/java/${pkgname}/${pkgname}-${pkgver}.jar ${pkgdir}/usr/share/java/${pkgname}/${pkgname}.jar
    ln -s /usr/share/java/${pkgname}/${pkgname}-${pkgver}-sources.jar ${pkgdir}/usr/share/java/${pkgname}/${pkgname}-sources.jar
    ln -s /usr/share/java/${pkgname}/${pkgname}-${pkgver}-javadoc.jar ${pkgdir}/usr/share/java/${pkgname}/${pkgname}-javadoc.jar
}

