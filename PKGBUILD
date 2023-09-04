# Maintainer: Leuc

pkgname=ffmpeg-omx
pkgver=4.4.4
pkgrel=1
pkgdesc='Complete solution to record, convert and stream audio and video with OMX patches for StarFive Vision Five 2 SBC'
arch=('riscv64')
url=https://ffmpeg.org/
prefix=/opt/ffmpeg-omx
install=ffmpeg-omx.install
license=(GPL3)
depends=(
  alsa-lib
  aom
  bzip2
  fontconfig
  fribidi
  gmp
  gnutls
  gsm
  jack
  lame
  libass.so
  libavc1394
  libbluray.so
  libdav1d.so
  libdrm
  libfreetype.so
  libiec61883
  libmodplug
  libpulse
  librav1e.so
  libraw1394
  librsvg-2.so
  libsoxr
  libssh
  libtheora
  libva.so
  libva-drm.so
  libva-x11.so
  libvdpau
  libvidstab.so
  libvorbisenc.so
  libvorbis.so
  libvpx.so
  libwebp
  libx11
  libx264.so
  libx265.so
  libxcb
  libxext
  libxml2
  libxv
  libxvidcore.so
  libzimg.so
  opencore-amr
  openjpeg2
  opus
  sdl2
  speex
  srt
  svt-av1
  v4l-utils
  xz
  zlib
  libOMX_Core.so
)
makedepends=(
  amf-headers
  clang
  git
  patch
)
provides=(
  libavcodec.so
  libavdevice.so
  libavfilter.so
  libavformat.so
  libavutil.so
  libpostproc.so
  libswresample.so
  libswscale.so
)
_tag=71fb6132637a2a430375c24afc381fff8b854fe7
source=(
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0001-swscale-x86-yuv2rgb-Fix-build-without-SSSE3.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0002-avcodec-vaapi_h264-skip-decode-if-pic-has-no-slices.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0003-libavutil-Fix-mips-build.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0004-configure-add-extralibs-to-extralibs_xxx.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0005-avcodec-add-omx-decoder-support.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0006-add-hevc-decoder-and-encoder-support.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0007-avcoder-fix-decoder-bug.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0008-fix-omx-decoder-setting-pix-fmt-bug.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0009-ffmpeg-add-mjpeg-decoder-support-and-fix-some-bug.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0010-ffmpeg-support-to-change-gop.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0011-ffmpeg-add-delay-for-decoding.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0012-ffmpeg-add-omx_pix_fmt.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0013-ffmpeg-replace-the-indent-with-space.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0014-ffmpeg-add-pixel-foramt.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0015-ffmpeg-remove-delay.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0016-FFmpeg-omx-add-scale-option-for-omx.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0017-FFmpeg-omxdec-add-mirror-rotation-and-crop-option.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0018-FFmpeg-omx-gop-parameter-of-hevc-encoder.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0019-FFmpeg-omcdec-fix-mjpeg_omx-decoder-scale-option-bug.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0020-FFmpeg-omxdec-modify-the-range-of-width-and-height-o.patch"
  "https://github.com/starfive-tech/Debian/raw/v0.9.0-engineering-release-wayland/multimedia/patch/ffmpeg/0021-FFmpeg-omxdec-set-pts-of-avframe-and-fix-some-compil.patch"
  "git+https://git.ffmpeg.org/ffmpeg.git#tag=${_tag}"
)
md5sums=(
  7ccec04db2c458b7b29109fa4223935d
  59c6098207203b8366e4bb35d899a32c
  15c3db0366ed40b685b78ed571e161dd
  ff895a30e22151ade3850f9d3e5c043d
  8cacfd45691e47bfff3a7bea8055b072
  6ae455aada902b0bdf68b14beb6e9248
  a59f157db51c06e43865ee207ff8f966
  4a344c5afc07355c057796b2dd554257
  a67b17d52837483507e1553962acc848
  b387aa021064aa1f00ee6c0f1441a217
  50f1f3675296f6ce50951bda71bd0eb6
  9b725a3fd82f8d7606ec0beebddb41a9
  a6af1c12d137f12cf54860c515d9de42
  f8e0bfa2040805538af1cb1f980f5109
  848d3f63316256af72da5c1400ba3892
  0fdefb146c46a1acc5967b023b6fa68a
  3e33479e89a88d711093e79cfb75a3b1
  d946a935b83ec6b68f4ab55b63fd9cbc
  f25d606e06567a94cbf8c19e29c70907
  74391b65719cc1652675f89739d307b0
  88bc6012019dcaed3c464325a03fa21a
  SKIP
)

pkgver() {
  cd ffmpeg
  git describe --tags | sed 's/^n//'
}

prepare() {
  cd ffmpeg
  git cherry-pick -n 988f2e9eb063db7c1a678729f58aab6eba59a55b # fix nvenc on older gpus
  git cherry-pick -n 031f1561cd286596cdb374da32f8aa816ce3b135 # remove compressed_ten_bit_format
  for patchfile in ${srcdir}/*.patch; do
    patch -g0 -p1 --remove-empty-files --no-backup-if-mismatch --batch --forward --directory=${srcdir}/ffmpeg --input="${patchfile}"
  done
}

build() {
  cd ffmpeg

  ./configure \
    --prefix=$prefix \
    --disable-debug \
    --disable-doc \
    --enable-programs \
    --disable-static \
    --disable-stripping \
    --enable-amf \
    --enable-cuda-llvm \
    --enable-lto \
    --enable-fontconfig \
    --enable-gmp \
    --enable-gnutls \
    --enable-gpl \
    --enable-libaom \
    --enable-libass \
    --enable-libbluray \
    --enable-libdav1d \
    --enable-libdrm \
    --enable-libfreetype \
    --enable-libfribidi \
    --enable-libgsm \
    --enable-libiec61883 \
    --enable-libjack \
    --enable-libmodplug \
    --enable-libmp3lame \
    --enable-libopencore_amrnb \
    --enable-libopencore_amrwb \
    --enable-libopenjpeg \
    --enable-libopus \
    --enable-libpulse \
    --enable-librav1e \
    --enable-librsvg \
    --enable-libsoxr \
    --enable-libspeex \
    --enable-libsrt \
    --enable-libssh \
    --enable-libsvtav1 \
    --enable-libtheora \
    --enable-libv4l2 \
    --enable-libvidstab \
    --enable-libvorbis \
    --enable-libvpx \
    --enable-libwebp \
    --enable-libx264 \
    --enable-libx265 \
    --enable-libxcb \
    --enable-libxml2 \
    --enable-libxvid \
    --enable-libzimg \
    --enable-shared \
    --enable-version3 \
    --enable-omx \
    --extra-cflags="-I/usr/include/omx-il" \
    --extra-libs="-lOMX_Core"

  make
  make tools/qt-faststart
}

package() {
  make DESTDIR="${pkgdir}" -C ffmpeg install

  install -dm0755 "$pkgdir/etc/ld.so.conf.d/"
  echo "$prefix/lib" > "$pkgdir/etc/ld.so.conf.d/ffmpeg-omx.conf"
}

# vim:set sw=2 ts=2 et:
