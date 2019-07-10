# Akademija FRI Website
Build with ❤️ using [Hugo](https://gohugo.io/).

[![Netlify Status](https://api.netlify.com/api/v1/badges/9bfc7cc9-c2f2-4918-820d-4ccc5b5942c8/deploy-status)](https://app.netlify.com/sites/akademija-fri/deploys)

Link: [akademijafri.si](https://akademijafri.si)

## How to Contribute
1. [Install dependencies](#dependencies)
2. Make changes check them out locally (Run `make` and visit `http://localhost:1313`)
3. Once satisfied create a pull request


## Development
### Dependencies
* [Hugo](https://gohugo.io/)
* [GNU Make](https://www.gnu.org/software/make/)
* [ImageMagick](https://imagemagick.org/index.php) - required for production builds

### Commands
#### Local development server
```bash
make
```

#### Builds
##### Development
```bash
make build-dev
```

##### Production
Production build will resize all build artifact .jpg images from `static/uploads` to a width of 1920px, preserving the aspect ratio. 
[ImageMagick](https://imagemagick.org/index.php) is required for this process.

```bash
# Replace "http://example.com" with the base url of the site
make build-prod url=http://example.com 
```

#### Other
```bash
make clean  # run after "make build-dev" or "make build-prod"
```
