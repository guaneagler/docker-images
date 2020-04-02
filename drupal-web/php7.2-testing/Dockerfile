FROM ciandtchina/drupal-web:php7.2-apache

LABEL maintainer="guaneagler@gmail.com"


# Install wkhtmltopdf
RUN apt-get update; \
	apt install -y xfonts-75dpi xfonts-base gvfs colord glew-utils libvisual-0.4-plugins gstreamer1.0-tools opus-tools qt5-image-formats-plugins qtwayland5 qt5-qmltooling-plugins librsvg2-bin lm-sensors
COPY pkg/wkhtmltox_0.12.5-1.stretch_amd64.deb /tmp/wkhtmltox_0.12.5-1.stretch_amd64.deb
RUN dpkg -i /tmp/wkhtmltox_0.12.5-1.stretch_amd64.deb

# Chinese font support
RUN apt install -y fonts-arphic-gbsn00lp
