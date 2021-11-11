# Gofi nightly build

this repo will auto build gofi by GitHub Actions at 00:00 every day.

## Docker Usage (Nightly Build)

```bash
docker run -d \
              --name=gofi \
              -p 80:8080 \
              -v ~/gofi:/app \
              -v ~/gofi/storage:/app/storage \
              --restart unless-stopped \
              sloaix/gofi:nightly-prod-latest
```
