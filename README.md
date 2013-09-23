# Updated GDAL library for CentOS 6.x

Originally ~~butchered and slaughtered~~ sourced from a SuSe SRPM that works
with the SuSe RPM naming conventions, so I just abruptly removed as many
possible dependencies as possible just to get a compile working. Among the
curiosities of such a hasty amputation is that there's a python-gdal that
builds, but even though we have Java bindings also built there is no java-gdal
that is produced. Maybe a kind soul will change this mishapen SPEC file to be a
better citizen of the CentOS world than what we have here. The updated version
dependencies of every other library in here will make this a much bigger task
than it appears. Not a surprise that RedHat stopped trying to support a lot of
these libraries.

Currently up to GDAL 1.10.1
