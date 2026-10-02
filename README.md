# Hi, I'm Jonas Rønningen 👋

Software developer with a background in Computer Engineering and practical
experience developing user-focused applications and system integrations.

I primarily work with C#, .NET and WPF/MVVM, and I also have experience with
Java, JavaScript, Python, SQL, Angular and basic C++.

## About me

- Based in Vinstra, Norway
- Computer Engineering studies at Western Norway University of Applied Sciences
- Practical development experience through my own company
- Developed and continued working on a VR dashboard solution for
  Helse Vest IKT and Haukeland University Hospital
- Interested in software architecture, system integration and maintainable code
- Exchange semester at Griffith University in Australia

## Professional experience

Through my sole proprietorship, Rønningen Interactive, I collaborate with
Helse Vest IKT on the development and continued improvement of a VR dashboard
application for Energisenteret for barn og unge at Haukeland University Hospital.

My work includes:

- Development in C#, .NET and WPF
- MVVM architecture and application structure
- Integration with SteamVR and OpenVR
- Debugging and improvement of existing functionality
- Adapting the application to real user needs
- Communication and coordination with the client

## Technologies

**Languages**

C# · Java · JavaScript · Python · SQL · C++ fundamentals

**Frameworks and technologies**

.NET · WPF · MVVM · Angular · REST APIs · SteamVR · OpenVR

**Tools and practices**

Git · GitHub · Visual Studio · VS Code · Debugging · Testing · Documentation

## Featured project

### VR Dashboard for Helse Vest IKT Bergen

A desktop application designed to make VR systems easier to operate for
healthcare personnel without extensive technical experience.

The project included:

- Development with C#, .NET and WPF
- MVVM architecture and separation of responsibilities
- SteamVR and OpenVR integration
- Game library and profile management
- VR equipment and application status
- Error handling, debugging and usability improvements
- Continued development through a commercial assignment

<p align="center">
  <img src="/VRDashboard_Main.png" width="49%" />
</p>

## Personal projects

### [adsb-pipeline](https://github.com/h669791/adsb-pipeline)

A self-initiated project to learn the chain from a passive radio receiver to a live operator map,
using real-time aircraft positions from ADS-B signals.

**Stack:** TypeScript · Node.js · Fastify · WebSocket · React · Vite · MapLibre GL JS

**Next:** RTL-SDR · readsb · Raspberry Pi

- **Real-time pipeline:** the backend reads readsb's `aircraft.json` every second and pushes snapshots
  to the browser over WebSocket, with automatic reconnect and backoff.
- **Validation at the boundary:** raw data is treated as `unknown`, validated and normalized into a typed
  `Observation`. Unknown values stay `null` instead of becoming 0.
- **Honest about uncertainty:** markers fade and an uncertainty circle grows with position age
  (speed × age), so stale positions never look fresh.
- **Clock-aware timestamps:** sensor time and receive time are kept separate, and position age is
  measured on a single clock.

**Status:** Works end-to-end with test data. Next step is live reception with an RTL-SDR dongle on a
Raspberry Pi. readsb handles the signal processing; I built the rest of the chain.

### [DeviceHub](https://github.com/h669791/devicehub)
A backend platform for managing and monitoring simulated VR headsets. Inspired by my work on a VR dashboard for Helse Vest IKT, but written from scratch on my own time, using simulated data only.

**Stack:** C# · ASP.NET Core Web API · Entity Framework Core · PostgreSQL · Docker

**Built so far**
- REST API with full CRUD for headsets, using DTOs to separate the API contract from the database model
- Input validation, plus 404 and 409 Conflict handling for missing resources and duplicate serial numbers
- PostgreSQL running in Docker, with schema managed through EF Core migrations

**Roadmap**
- Sessions and experiences with business rules (e.g. a headset must be online to start a session)
- Live status updates with SignalR and a React/TypeScript frontend
- xUnit tests and CI with GitHub Actions
- A headset simulator in Kotlin/Spring Boot that sends status messages to the API through a message queue


## What I value

I aim to build software that is understandable, maintainable and useful.

## Currently learning

- Improving MVVM architecture and application structure
- C#
- Testing and maintainable software design
- Cloud technologies and deployment

## Contact

- LinkedIn: https://www.linkedin.com/in/jonas-r-a5428a132/
- Email: jonas-the@hotmail.com
