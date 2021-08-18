# Antora UI

Reference tutorial: https://fedoramagazine.org/using-antora-for-your-open-source-documentation

## Prerequisite

Having the documentation repo pushed and configured in antora-playbook.yml

## Usage

```bash
docker pull antora/antora
docker run --rm -it -v $(pwd):/antora:z antora/antora antora-playbook.yml --stacktrace
cd build/site
python3 -m http.server 8080
# Open your browers on localhost:8080 to view your documentation site
```
