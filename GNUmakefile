export ARCH=powerpc
export CROSS_COMPILE=/opt/OSELAS.Toolchain-2012.12.1/powerpc-603e-linux-gnu/gcc-4.7.2-glibc-2.16.0-binutils-2.22-kernel-3.6-sanitized/bin/powerpc-603e-linux-gnu-


all := $(filter-out Makefile,$(MAKECMDGOALS))

_all:
	$(MAKE) --no-print-directory -j$(nproc) -f Makefile $(all)

$(all): _all
	@:

%/: _all
	@:
