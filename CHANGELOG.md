# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]


## [v2.0.0] - 2019-10-25

### Added
- Added OpenSSL, which is used to compile versions of Python 3.7+, it is not packaged in GeoLambda Layer
- OPENSSL_VERSION=1.0.2

### Changed
- Updated GDAL, PROJ, and Geotiff libraries.
- GDAL_VERSION=3.0.1
- PROJ_VERSION=6.2.0
- GEOTIFF_VERSION=1.5.1


## [v1.2.0] - 2019-10-24

### Added
- A Python GeoLambda Layer is now published, along with the base Lambda Layer. The base layer *must* be included in any Lambda that uses the Python GeoLambda layer. It includes the Python libraries GDAL, rasterio, pyproj, and shapely.
- Base geolambda includes OpenSSL 1.0.2, as this is required for compiling Python 3.7+. It is not included in the Lambda layer, just the base layer for ease of creating different versions of Python child images.


### Changed
- The python diectory, and the new Lambda layer, now uses Python 3.7.4
- GDAL_VERSION=2.4.2
- GEOS_VERSION=3.8.0
- NETCDF_VERSION=4.7.1
- NGHTTP2_VERSION=1.39.2
- OPENJPEG_VERSION=2.3.1
- CURL_VERSION=7.66.0
- LIBJPEG_TURBO_VERSION=2.0.3
- WEBP_VERSION=1.0.3
- ZSTD_VERSION=1.4.3


## [v1.1.0] - 2018-03-22

### Added
- Make compatible with Lambda Layers
- Python example
- Improve documentation
- More libraries (CURL with http2, webp, zstd, libjpegturbo)
- GeoTIFF now compiled from scratch rather than GGDAL builtin
- Published public lambda layers - see README for ARNs
- GEOTIFF_VERSION=1.4.3
- OPENJPEG_VERSION=2.3.0
- LIBJPEG_TURBO_VERSION=2.0.1
- CURL_VERSION=7.59.0
- NGHTTP2_VERSION=1.35.1
- WEBP_VERSION=1.0.1
- ZSTD_VERSION=1.3.8

### Changed
- Major refactor, GeoLambda base now runtime agnostic contains system libraries only
- GDAL_VERSION=2.4.1
- GEOS_VERSION=3.7.1
- HDF4_VERSION=4.2.14
- HDF5_VERSION=1.10.5
- NETCDF_VERSION=4.6.2

### Removed
- Removed Python codes to make geolambda system libraries only


## [v1.0.0] - 2018-07-27

Initial release

Package Versions
- PROJ_VERSION=5.2.0
- GEOS_VERSION=3.6.2
- HDF4_VERSION=4.2.12
- SZIP_VERSION=2.1.1
- HDF5_VERSION=1.10.1
- NETCDF_VERSION=4.6.1
- OPENJPEG_VERSION=2.3.0
- PKGCONFIG_VERSION=0.29.2
- GDAL_VERSION=2.3.1

[Unreleased]: https://github.com/sat-utils/sat-stac/compare/master...develop
[v2.0.0]: https://github.com/developmentseed/geolambda/compare/1.2.0...2.0.0
[v1.2.0]: https://github.com/developmentseed/geolambda/compare/1.1.0...1.2.0
[v1.1.0]: https://github.com/developmentseed/geolambda/compare/1.0.0...1.1.0
[v1.0.0]: https://github.com/developmentseed/geolambda/tree/1.0.0
