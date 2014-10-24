FROM scratch
MAINTAINER Bilge <bilge@scriptfusion.com>

ADD	rootfs.tar.xz	/

# Copy crude env emulator for Composer invocation support.
COPY	env							/usr/bin/

# Copy getcomposer.org CA certificate.
COPY	DigiCert_Global_Root_CA.pem	/etc/ssl/certs/ca-certificates.crt

# Install Composer.
RUN	[\
	"php", "-r", "eval('?>'.file_get_contents('https://getcomposer.org/installer'));", \
	"--", "--filename=composer", "--install-dir=/usr/bin" \
]

CMD	["php", "-a"]
