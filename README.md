# App Dashboard
Dockerised configuration for the app dashboard based on [Homer](https://github.com/bastienwirtz/homer).

## Screenshots

### Dark theme
<img src="https://raw.githubusercontent.com/JorgeAnzola/homer-dashboard/master/assets/readme/dark.jpg">

### Light theme
<img src="https://raw.githubusercontent.com/JorgeAnzola/homer-dashboard/master/assets/readme/light.jpg">

## Installing

```
cd ~
git clone https://github.com/JorgeAnzola/homer-dashboard homer
cd homer
docker-compose up -d
```

### Starting Home on reboot
```
crontab -e
```

Add the following line to the cronjob file
```
@reboot docker-compose -f ~/homer/docker-compose.yaml up -d
```

## Icons
Most of them from [NX221's repo](https://github.com/NX211/homer-icons).

## Roadmap
- Get Sonarr and Radarr working. Probably [#254](https://github.com/bastienwirtz/homer/pull/254) this is merge.
- Get `Ping` service type working