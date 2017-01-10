# Docker for Craft CMS

A MySQL container suitable for Craft CMS 2.x.

See the related [Stack Exchange issue](https://craftcms.stackexchange.com/questions/12084/getting-this-sql-error-group-by-incompatible-with-sql-mode-only-full-group-by/12106) to learn why the latest MySQL version's default config is incompatible with Craft version 2.

The instructions below are for the Able development team. This repo remains public in the spirit of sharing.

## Build

After making changes, rebuild the image with the `latest` tag.

```bash
docker build -f Dockerfile -t ablelending/craftcms-mysql:latest ./
```

## Push to Docker Hub

After rebuilding the image, be sure to push it to Docker Hub.

```bash
docker push ablelending/craftcms-mysql
```

## License

[MIT License](/LICENSE).
