# Kindlegen Buildpack
This is a Kindlegen buildpack for Heroku. It installs the Kindlegen command line tool for generating mobi files. It downloads a Kindlegen tarball from S3, extracts and moves the binary and sets the path environment variable. The binary will be located in `/app/vendor/kindlegen/bin`.

## Usage
Add the buildpack:
```
heroku buildpacks:add --index 1 https://github.com/benmel/kindlegen-buildpack.git
```
Kindlegen will be installed at the next deployment.
