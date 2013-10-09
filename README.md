# GDAL v 1.10+ library for CentOS 6.x

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

# Currency

Currently up to GDAL 1.10.1

# Effective Dependencies

libgeotiff and libgeotiff-devel 1.2.5+ are required to install the gdal RPM. Following is what gets pulled
down with a minimal CentOS6 install that has EPEL repo enabled:

    ===============================================================================================================================================
     Package                          Arch                Version                            Repository                                       Size
    ===============================================================================================================================================
    Installing: 
     gdal                             x86_64              1.10.1-1.tst.1                     /gdal-1.10.1-1.tst.1.x86_64                     3.8 M
     gdal-devel                       x86_64              1.10.1-1.tst.1                     /gdal-devel-1.10.1-1.tst.1.x86_64                14 M
     libgdal                          x86_64              1.10.1-1.tst.1                     /libgdal-1.10.1-1.tst.1.x86_64                   62 M
     python-gdal                      x86_64              1.10.1-1.tst.1                     /python-gdal-1.10.1-1.tst.1.x86_64              3.5 M
    Installing for dependencies:
     expat-devel                      x86_64              2.0.1-11.el6_2                     base                                            120 k
     geos                             x86_64              3.3.2-1.el6                        epel                                            505 k
     geos-devel                       x86_64              3.3.2-1.el6                        epel                                            1.3 M
     giflib-devel                     x86_64              4.1.6-3.1.el6                      base                                             85 k
     keyutils-libs-devel              x86_64              1.4-4.el6                          base                                             28 k
     krb5-devel                       x86_64              1.10.3-10.el6_4.6                  updates                                         495 k
     libcom_err-devel                 x86_64              1.41.12-14.el6_4.2                 updates                                          32 k
     libcurl-devel                    x86_64              7.19.7-37.el6_4                    updates                                         244 k
     libidn-devel                     x86_64              1.18-2.el6                         base                                            137 k
     libjpeg-turbo-devel              x86_64              1.2.1-1.el6                        base                                             96 k
     libpng-devel                     x86_64              2:1.2.49-1.el6_2                   base                                            112 k
     libselinux-devel                 x86_64              2.0.94-5.3.el6_4.1                 updates                                         136 k
     libsepol-devel                   x86_64              2.0.41-4.el6                       base                                             64 k
     openssl-devel                    x86_64              1.0.0-27.el6_4.2                   updates                                         1.1 M
     postgresql-libs                  x86_64              8.4.13-1.el6_3                     base                                            200 k
     unixODBC                         x86_64              2.2.14-12.el6_3                    base                                            378 k
     xerces-c                         x86_64              3.0.1-20.el6                       base                                            866 k
     xerces-c-devel                   x86_64              3.0.1-20.el6                       base                                            520 k
     zlib-devel                       x86_64              1.2.3-29.el6                       base                                             44 k
    Updating for dependencies:
     curl                             x86_64              7.19.7-37.el6_4                    updates                                         193 k
     e2fsprogs                        x86_64              1.41.12-14.el6_4.2                 updates                                         552 k
     e2fsprogs-libs                   x86_64              1.41.12-14.el6_4.2                 updates                                         120 k
     krb5-libs                        x86_64              1.10.3-10.el6_4.6                  updates                                         761 k
     krb5-workstation                 x86_64              1.10.3-10.el6_4.6                  updates                                         805 k
     libcom_err                       x86_64              1.41.12-14.el6_4.2                 updates                                          36 k
     libcurl                          x86_64              7.19.7-37.el6_4                    updates                                         165 k
     libselinux                       x86_64              2.0.94-5.3.el6_4.1                 updates                                         108 k
     libselinux-python                x86_64              2.0.94-5.3.el6_4.1                 updates                                         202 k
     libselinux-utils                 x86_64              2.0.94-5.3.el6_4.1                 updates                                          81 k
     libss                            x86_64              1.41.12-14.el6_4.2                 updates                                          41 k
     openssl                          x86_64              1.0.0-27.el6_4.2                   updates                                         1.4 M
