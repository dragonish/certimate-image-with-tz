# certimate-image-with-tz

Build certimate image and introduce support for TZ.

## Usage

```bash
# pull
docker pull giterhub/certimate:latest

# run
docker run -d \
    --name certimate \
    --restart unless-stopped \
    -e TZ="your_timezone" \
    -p 8090:8090 \
    -v ./data:/app/pb_data \
    giterhub/certimate:latest
```

## Credits

- [certimate-go/certimate](https://github.com/certimate-go/certimate)
