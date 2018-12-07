FROM archlinux/base

RUN pacman -Syu --noconfirm
RUN pacman -S --noconfirm gcc make cmake git openssh vim wget curl python
RUN pacman -S --noconfirm boost cfitsio gsl swig dirmngr lsb-release doxygen
RUN pacman -S --noconfirm fftw openal gpsd dcraw gtest gmock
RUN pacman -S --noconfirm libnova libraw libdc1394 libftdi-compat libftdi
RUN pacman -S --noconfirm libusb rtl-sdr limesuite ffmpeg libcurl-gnutls libgphoto2
RUN pacman -S --noconfirm libjpeg6-turbo libtiff confuse

WORKDIR /home

ADD https://raw.githubusercontent.com/jochym/indi/master/docker/run-build.sh /home/
RUN chmod a+x /home/run-build.sh
