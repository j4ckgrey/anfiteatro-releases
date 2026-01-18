<div align="center">
  <img src="Anfiteatro_name_below.png" alt="Anfiteatro Logo" width="200" />
  <p>
    <b>A media streaming client compatible with Jellyfin and Remux Server.</b>
  </p>
  <p>
    Anfiteatro is a modern client focused on direct play and remux performance, optimized for Android TV and Mobile.
  </p>
</div>

## Releases

This repository tracks the public releases of Anfiteatro.

## Installation Options

### Android Client
Download the latest `.apk` from the Releases section.

### Samsung Tizen TV
To install on a Samsung Smart TV (Tizen OS):

**Method 1: Using the Installer (Recommended)**
1. Download the **Anfiteatro2Samsung Installer** for your computer (Windows, Linux, or macOS) from the Releases section.
2. Enable **Developer Mode** on your TV:
   - Go to "Apps" on your TV.
   - Press `12345` on your remote.
   - Toggle "Developer Mode" to **On**.
   - Enter your computer's IP address and restart the TV.
3. Run the installer, select your TV, choose "Anfiteatro" from the list, and click **Download & Install**.

**Method 2: Manual WGT Installation**
1. Download the `.wgt` file from the Releases section.
2. Use the Tizen CLI to install:
   ```bash
   tizen install -n Anfiteatro-1.0.0-beta.2.wgt -t <TV_IP_ADDRESS>
   ```

### Docker (Self-Hosted)
The recommended public image is on Docker Hub:
```bash
docker pull j4ckgrey/anfiteatro_releases:latest
```

#### Docker Compose
```yaml
services:
  anfiteatro:
    image: j4ckgrey/anfiteatro_releases:latest
    container_name: anfiteatro
    ports:
      - "6661:80"
    restart: unless-stopped
```

### Web Browser
You can access the latest beta version directly in your browser:
https://anfiteatro-web.vercel.app/
## Community & Support

- **Bugs & Issues:** [GitHub Issues](https://github.com/j4ckgrey/anfiteatro_releases/issues)  
- **Discussions:** [Discord](https://discordapp.com/channels/1433689453158862943/1441378427239137300)  
- **Support:** If you like my work and want to support development, consider buying me a coffee: https://ko-fi.com/j4ckgrey
---