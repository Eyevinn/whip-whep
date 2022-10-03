# WHIP / WHEP 

Docker compose file to setup a local [WHIP](https://www.ietf.org/archive/id/draft-ietf-wish-whip-01.html) and [WHEP](https://www.ietf.org/id/draft-murillo-whep-00.html) development environment. Helpful when building either WHIP- or WHEP-clients.

When started it will start the following containers:

- Ingest Endpoint: [WHIP Endoint](https://www.npmjs.com/package/@eyevinn/whip-endpoint)
- Origin SFU: [Symphony Media Bridge](https://github.com/finos/SymphonyMediaBridge)
- Edge SFU: [Symphony Media Bridge](https://github.com/finos/SymphonyMediaBridge)
- Egress Endpoint: [WHEP Endpoint](https://www.npmjs.com/package/@eyevinn/wrtc-egress)

## Usage

Start

```bash
curl -SL https://github.com/Eyevinn/whip-whep/releases/v0.0.1/docker-compose.yml | docker-compose up
```

Stop

```bash
curl -SL https://github.com/Eyevinn/whip-whep/releases/v0.0.1/docker-compose.yml | docker-compose down
```

Once everything is up and running you will have a WHIP/WHEP endpoints available at:
- WHIP: [http://localhost:8200/api/v2/whip/sfu-broadcaster?channelId=test](https://web.whip.eyevinn.technology/?endpoint=http%3A%2F%2Flocalhost%3A8200%2Fapi%2Fv2%2Fwhip%2Fsfu-broadcaster%3FchannelId%3Dtest)
- WHEP: http://localhost:8300/whep/channel/test

## Support

Join our [community on Slack](http://slack.streamingtech.se) where you can post any questions regarding any of our open source projects. Eyevinn's consulting business can also offer you:

- Further development of this component
- Customization and integration of this component into your platform
- Support and maintenance agreement

Contact [sales@eyevinn.se](mailto:sales@eyevinn.se) if you are interested.

## About Eyevinn Technology

Eyevinn Technology is an independent consultant firm specialized in video and streaming. Independent in a way that we are not commercially tied to any platform or technology vendor.

At Eyevinn, every software developer consultant has a dedicated budget reserved for open source development and contribution to the open source community. This give us room for innovation, team building and personal competence development. And also gives us as a company a way to contribute back to the open source community.

Want to know more about Eyevinn and how it is to work here. Contact us at work@eyevinn.se!
