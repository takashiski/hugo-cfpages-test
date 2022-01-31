# Hugo(with asciidoc) + Cloudflare Pages

```sh
docker run --name hugo --mount type=bind,source="$(pwd)",target=/src klakegg/hugo:asciidoctor new site $THIS_REPOSITORY
cd $THIS_REPOSITORY
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
# edit config.toml and set "theme=ananke"
```
