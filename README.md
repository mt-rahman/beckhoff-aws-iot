<!-- [![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url] -->
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<!-- <br /> -->
<div align="center">
  <a href="https://github.com/mt-rahman/beckhoff-aws-iot">
  </a>

<h3 align="center">Beckhoff Embedded PC | IoT | AWS | Fleet Monitoring</h3>

  <p align="center">
    A TwinCAT Project for an IoT monitoring system for fleet monitoring using Beckhoff's embedded PCs
</div>

<!-- ABOUT THE PROJECT -->
## About The Project

<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->

### Features:

* Read data with a sampling rate of 1 Hz & 100 Hz from analog sensors, RS-232 serial, and GPS
* Periodically send data to AWS IoT Core using MQTT
* Buffers data to SQLite database in case of network connection loss
* Saves sent data to SQLite database for local data storage

## Project Tree
```bash
.
├── FullSystem
│   ├── Database
│   │   ├── Database.tcconnproj
│   │   └── TcDbServer.tcdbsrv
│   ├── FullSystem.sln
│   └── Plc
│       ├── App
│       │   ├── DUTs
│       │   │   ├── ST_SelectStructData.TcDUT
│       │   │   ├── ST_SelectStructData.xml
│       │   │   ├── ST_SelectStructIMU.TcDUT
│       │   │   └── ST_SelectStructIMU.xml
│       │   ├── GVLs
│       │   │   └── GVL.TcGVL
│       │   ├── PlcTask_Background.TcTTO
│       │   ├── PlcTask_Buffer.TcTTO
│       │   ├── PlcTask_Read.TcTTO
│       │   ├── PlcTask_Send.TcTTO
│       │   ├── PlcTask_Vacuum.TcTTO
│       │   ├── POUs
│       │   │   ├── Background_FatigueCam.TcPOU
│       │   │   ├── Background_GPS.TcPOU
│       │   │   ├── Background_IMU.TcPOU
│       │   │   ├── Background_Time.TcPOU
│       │   │   ├── Buffer_Data.TcPOU
│       │   │   ├── Buffer_IMU.TcPOU
│       │   │   ├── DRAFT_Buffer_Data.TcPOU
│       │   │   ├── DRAFT_Get_Data.TcPOU
│       │   │   ├── FB_FatigueCam_Receive.TcPOU
│       │   │   ├── Get_Data.TcPOU
│       │   │   ├── Get_IMU.TcPOU
│       │   │   ├── Main_Background.TcPOU
│       │   │   ├── Main_Buffer.TcPOU
│       │   │   ├── Main_Read.TcPOU
│       │   │   ├── Main_Send.TcPOU
│       │   │   ├── Main_Vacuum.TcPOU
│       │   │   ├── Read_FatigueCam.TcPOU
│       │   │   ├── Read_GPS.TcPOU
│       │   │   ├── Read_ID.TcPOU
│       │   │   ├── Read_IMU.TcPOU
│       │   │   ├── Read_Payload.TcPOU
│       │   │   ├── Read_Pressure.TcPOU
│       │   │   ├── Save_Data.TcPOU
│       │   │   ├── Save_IMU.TcPOU
│       │   │   ├── Send_IMU.TcPOU
│       │   │   ├── Send.TcPOU
│       │   │   ├── Vacuum_Buffer_Data_2.TcPOU
│       │   │   ├── Vacuum_Buffer_Data.TcPOU
│       │   │   ├── Vacuum_Buffer_IMU_2.TcPOU
│       │   │   ├── Vacuum_Buffer_IMU.TcPOU
│       │   │   ├── Vacuum_Data.TcPOU
│       │   │   └── Vacuum_IMU.TcPOU
│       │   └── App.plcproj
│       └── FullSystem.tsproj
├── LICENSE
└── README.md
```

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact

Muhammad Taufik Rahman - mtaufikrahman@ymail.com

Project Link: [https://github.com/mt-rahman/beckhoff-aws-iot](https://github.com/mt-rahman/beckhoff-aws-iot)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
<!-- [contributors-shield]: https://img.shields.io/github/contributors/mt-rahman/beckhoff-aws-iot.svg?style=for-the-badge
[contributors-url]: https://github.com/mt-rahman/beckhoff-aws-iot/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/mt-rahman/beckhoff-aws-iot.svg?style=for-the-badge
[forks-url]: https://github.com/mt-rahman/beckhoff-aws-iot/network/members
[stars-shield]: https://img.shields.io/github/stars/mt-rahman/beckhoff-aws-iot.svg?style=for-the-badge
[stars-url]: https://github.com/mt-rahman/beckhoff-aws-iot/stargazers
[issues-shield]: https://img.shields.io/github/issues/mt-rahman/beckhoff-aws-iot.svg?style=for-the-badge
[issues-url]: https://github.com/mt-rahman/beckhoff-aws-iot/issues -->
[license-shield]: https://img.shields.io/github/license/mt-rahman/beckhoff-aws-iot.svg?style=for-the-badge
[license-url]: LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/mtaufikrahman
<!-- [product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com -->