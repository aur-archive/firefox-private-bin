# Maintainer  : Fernando "Firef0x" G.P. da Silva <firefgx { aT ) gmail [ d0t } com>
# Contributor : Fernando "Firef0x" G.P. da Silva <firefgx { aT ) gmail [ d0t } com>
# Contributor : Kyro <chris-bos-lee@hotmail.com>

_majorver=38
_pkgver=${_majorver}.x
# Only use when the version is different from the package 'firefox' in [community]
# _pkgver2=34.0.5

pkgname=firefox-private-bin
pkgver="${_majorver}.0"
pkgrel=1
pkgdesc="Standalone web browser from mozilla.org, built with GCC -O3 with graphite optimization, media-libs/gstreamer, Unity global menu and environment variable MOZILLA_DISABLE_PLUGINS support."
arch=('x86_64')
license=('MPL' 'GPL' 'LGPL')
url="http://sourceforge.net/projects/libportable/files/Firefox/"
depends=('gtk2'
         'mozilla-common'
         'libxt'
         'startup-notification'
         'mime-types'
         'dbus-glib'
         'alsa-lib'
         'desktop-file-utils'
         'hicolor-icon-theme'
         'libvpx'
         'icu'
         'libevent'
         'nss'
         'hunspell'
         'sqlite')
optdepends=('networkmanager: Location detection via available WiFi networks'
            'gstreamer0.10-base-plugins: vorbis decoding, ogg demuxing'
            'gstreamer0.10-good-plugins: webm and mp4 demuxing'
            'gstreamer0.10-bad-plugins: aac, vp8 and opus decoding'
            'gstreamer0.10-ugly-plugins: h.264 and mp3 decoding'
            'gstreamer0.10-ffmpeg: more decoders'
            'upower: Battery API')
provides=("firefox=${pkgver}" "firefox-i18n-zh-cn=${pkgver}")
conflicts=('firefox')
replaces=('firefox-private' 'firefox-private-zh-cn')
options=('!emptydirs')

# If you couldn't get the first source file, replace the first item in array 'source' with the following link
# 如果您不能下载source里的第一个文件，请用以下链接替换source数组的第一项(如果还是不行，请番,羽,土,啬)
# "http://jaist.dl.sourceforge.net/project/libportable/Firefox/${CARCH}/${_pkgver}/firefox-private-${pkgver}.zh-CN.linux-${CARCH}.tar.bz2"
source=("http://downloads.sourceforge.net/project/libportable/Firefox/${CARCH}/${_pkgver}/firefox-private-${pkgver}.zh-CN.linux-${CARCH}.tar.bz2"
        "vendor.js::https://projects.archlinux.org/svntogit/packages.git/plain/trunk/vendor.js?h=packages/firefox"
        "firefox.desktop::https://projects.archlinux.org/svntogit/packages.git/plain/trunk/firefox.desktop?h=packages/firefox"
        "16.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default16.png"
        "22.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default22.png"
        "24.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default24.png"
        "32.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default32.png"
        "48.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default48.png"
        "64.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/content/icon64.png"
        "128.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/mozicon128.png"
        "192.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/content/about-logo.png"
        "256.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/default256.png"
        "384.png::https://hg.mozilla.org/mozilla-central/raw-file/f0d1677cc3e8/browser/branding/official/content/about-logo@2x.png")
md5sums=('2f5573c23b50071d4602cd4b6fc1bc88'
         '0d053487907de4376d67d8f499c5502b'
         '9b02198df96be08f2a0a323ac2e6c2a2'
         'ccf618ebec94f98741cbf99ff5c89af6'
         '534778117755231290b5892165b2257b'
         'f11dcb54897188bb7cddc2a10bca048f'
         '1549dc3f6c0d0e0b0dc74b0955bf218c'
         '29e9295bf32d16560103327cbdacbe45'
         'e8dc544804a3e5033e9f5f18c9e7c2d4'
         '2c33a28d0fd6b94bffe717df9ca6a236'
         'bc3a02fbde6efb2c2bf8c28399345e23'
         '4b51c1ede396f37409b7b00bca1e366f'
         'b24fd5bc7acbf051c80cecf97b1929ba')
sha1sums=('3d4af5e741fdc9d8aefafc6279db18685b4c24a2'
          '7739fbea2838cb9148a1d77090ace46eeb397f79'
          'e3a2f893df8d462f7025bb2da57d3ce74979f192'
          '077c7737036af790eb9ee80102d082facf299606'
          'b74f9a7b72cf6295ebf7dd08734c6797500290aa'
          '345f4b9a9618ff3221f5c725073da1467057ea41'
          '5e933ab86483b449d7c5faeeb9bca496bb695703'
          '6209703d3cd18aede02bd945695095b2a5699c89'
          'a293ac493192e4a93d5360086785b0402f09c385'
          '2270a28c1d8f4aaf865cdd9bfa029a3db8f2ce51'
          '3e314c006819e0553841e0ebffb097e1632d278f'
          'e387bc1179f0551ca9ce308778c51e6632dd7dec'
          'acc9dd95a755d0ecf0f4854b708d6ac92f4f1ceb')

install=${pkgname}.install

changelog=README.md

# Set to 0 if you don't need the default searchplugins
# 如果您不需要默认的搜索引擎插件，请设置为0
_keep_searchplugins=1

package(){
  cd "${srcdir}"/firefox/

  install -d "${pkgdir}/usr/lib/firefox"
  mv * "${pkgdir}/usr/lib/firefox"

  # Install missing resource files
  install -Dm644 "${srcdir}/vendor.js" "${pkgdir}/usr/lib/firefox/browser/defaults/preferences/vendor.js"

  install -Dm644 "${srcdir}/firefox.desktop" "${pkgdir}/usr/share/applications/firefox.desktop"

  for i in 16 22 24 32 48 64 128 192 256 384; do
    install -d "${pkgdir}/usr/share/icons/hicolor/${i}x${i}/apps"
    install -Dm644 "${srcdir}/$i.png" "${pkgdir}/usr/share/icons/hicolor/${i}x${i}/apps/firefox.png"
  done

  # Use system-provided dictionaries
  ln -s /usr/share/hunspell "${pkgdir}/usr/lib/firefox/dictionaries"
  ln -s /usr/share/hyphen "${pkgdir}/usr/lib/firefox/hyphenation"

  # Remove default searchplugins if _keep_searchplugins=0
  if [ ${_keep_searchplugins} -eq 0 ]; then
    rm -f "${pkgdir}"/usr/lib/firefox/browser/searchplugins/*
  fi

  # Make symbolic links
  install -d "${pkgdir}/usr/bin"
  ln -sf /usr/lib/firefox/firefox "${pkgdir}"/usr/bin/firefox
  # Workaround for bug #658850
  # https://bugzilla.mozilla.org/show_bug.cgi?id=658850
  ln -sf /usr/lib/firefox/firefox "${pkgdir}"/usr/lib/firefox/firefox-bin
}

# vim:set sts=2 ts=2 sw=2 et:
