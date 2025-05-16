# RideMama

<div align="center">
  <img src="public/logo.jpeg" alt="Ridemama Logo" width="300px">
  <p><em>Simplifying Campus Commutes - One Ride at a Time.</em></p>
  <a href="https://ridemama.in">
  <img
    src="https://img.shields.io/badge/Live%20Site-ridemama.in-6f52ea?style=for-the-badge"
    alt="Live Site"
  />
</a>
</div>

Ridemama is a student-focused ride-sharing platform built to make daily commutes easier for students whose colleges are far from city centers. It aims to solve the challenges of finding instant rides, reducing daily bus struggles, and enabling smoother, more affordable transportation options.

## 📋 What's this repo for?

Because the main codebase is private, this repo serves as a technical walkthrough—showing architecture, build decisions, and the roadblocks we hit—without exposing source code.

## 🚀 Key Features

- **Host your own car**: Share your ride with fellow students
- **Find rides at your preferred time**: Flexible scheduling that fits your timetable
- **Affordable, constant prices**: No surge pricing regardless of traffic conditions
- **Route selection flexibility**: Choose the best route for your journey
- **Direct payments**: Seamless transactions between riders and hosts
- **Simple, student-friendly interface**: Designed with campus commuters in mind

## 🏗️ System Architecture

High-level architecture for RideMama

<div align="center">
  <img src="public/tech-architecture.jpeg" alt="Ridemama System Architecture" width="700px">
</div>

The platform is broken into separate services to keep things modular and easy to scale. Key parts include:

- Frontend client application
- Backend API services
- Database layer
- Third-party integrations (Maps, Payments, Messaging)

## 🗂️ High-Level DB Schema

<div align="center">
  <img src="public/erd.jpeg" alt="Ridemama Database ERD" width="700px">
</div>

Our MongoDB schema includes these primary collections:

- Users (riders and hosts)
- Rides (scheduling, routing)
- Payments (transactions)
- Vehicles (Registered vehicles)
- Report (reports and feedback)

## ⚙️ Tech Stack

| Component          | Technologies                          |
| ------------------ | ------------------------------------- |
| **Frontend**       | TypeScript, Next.js, Tailwind CSS     |
| **Backend**        | Node.js, Express.js                   |
| **Database**       | MongoDB (Atlas)                       |
| **Maps**           | Ola Maps by Krutrim                   |
| **Payments**       | Razorpay                              |
| **Messaging**      | Twilio WhatsApp Messaging             |
| **Authentication** | JWT                                   |
| **Hosting**        | DigitalOcean Droplets                 |
| **Image Storage**  | AWS S3                                |
| **Tooling and CI** | Zod, Docker, GitHub Actions for CI/CD |

## 🔭 Future Improvements

| Feature                      | Priority | Notes                                     |
| ---------------------------- | -------- | ----------------------------------------- |
| WebSocket Integration        | High     | Real-time ride updates                    |
| TypeScript Backend Migration | Medium   | Better type safety and maintainability    |
| RC and DL API Integration    | High     | For automated vehicle verification        |
| Cross-Platform App           | Low      | Mobile-first approach                     |
| Bike Registration            | Low      | Pending insurance and regulatory approval |

## 📸 Screenshots

<div align="center">
  <h3>Home Screen</h3>
  <img src="public/home.png" alt="Ridemama Home Screen" width="400px" height="800px">
  
  <h3>Settings</h3>
  <img src="public/settings.png" alt="Settings Screen" width="400px" height="800px">

  <h3>Host route Selection</h3>
  <img src="public/select-route.png" alt="Host Route Selection" width="400px" height="800px">
  
  <h3>Host Dashboard</h3>
  <img src="public/host-ride.jpeg" alt="Host Dashboard" width="400px" height="800px">

  <h3>Available rides</h3>
  <img src="public/avl-rides.jpeg" alt="Available Rides" width="400px" height="800px">
  
  <h3>Active rider page</h3>
  <img src="public/active-rider.jpeg" alt="Active Rider Page" width="400px" height="800px">

  <h3>Payment Interface</h3>
  <img src="public/payment.jpeg" alt="Payment Interface" width="400px" height="800px">
</div>

## 🛠️ Things We Had to Figure Out

### Handling real-time updates

Ridemama started as a simple side project, so we initially built it on a basic HTTP server. However, as the platform grew, we needed real-time features like live ride statuses and instant booking updates for a better user experience.

Integrating WebSockets turned out to be more complex than expected, given our current architecture. As a quick workaround, we opted for polling, which, while not the most efficient, handles our current traffic levels reasonably well.

That said, we plan to revisit this as the platform scales, potentially integrating WebSockets, server-sent events (SSE), or WebRTC for a more robust solution.

### Deployments

Initially, we handled Docker builds and deployments on our DigitalOcean droplet manually, which involved resizing droplets, managing SSH keys, and restarting services — a slow and error-prone process.

We solved this by implementing a CI/CD pipeline using GitHub Actions, automating the entire process. This reduced manual steps, minimized errors, and significantly sped up deployments, making the whole workflow much smoother and more reliable.

## 📚 Lessons Learned

- Simplify first, optimise later — early over-engineering would have stalled us.
- Automating deploys early saved us a ton of time later. CI/CD felt like overkill at first, but it helped avoid a lot of small mistakes.
- Real-time features are harder than they look — we’re holding off on WebSockets until we have a clearer use case.

## 👥 Contributors

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/SuryatejPonnapalli" target="#">
        <img src="https://github.com/SuryatejPonnapalli.png" width="100px" alt="Suryatej"/>
        <br />
        <b>Suryatej</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/harshith-1008" target="#">
        <img src="https://github.com/harshith-1008.png" width="100px" alt="Harshith"/>
        <br />
        <b>Harshith</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/KDDhanush25" target="#">
        <img src="https://github.com/KDDhanush25.png" width="100px" alt="Dhanush"/>
        <br />
        <b>Dhanush</b>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/BJVPavan" target="#">
        <img src="https://github.com/BJVPavan.png" width="100px" alt="Pavan"/>
        <br />
        <b>Pavan</b>
      </a>
    </td>
  </tr>
</table>

## 📜 License

MIT License - See [LICENSE](LICENSE) file for details.

## 🔗 Links and References

- [Our First CI/CD Pipeline for Ridemama](https://www.saiharshith.in/blog/first-cicd-pipeline)

## 🧩 Contributing

This repo is read-only for now, but we’re open to ideas, suggestions, or collabs — feel free to raise issues or reach out via LinkedIn.

## 🌱 Stay Connected

Join the Ridemama journey and connect with us

<div align="center">
  <a href="https://www.linkedin.com/company/ridemama/" target="#">
    <img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://www.instagram.com/ridemama_/" target="#">
    <img src="https://img.shields.io/badge/-Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
</div>

Follow the journey as we continue to improve Ridemama and expand its reach.

---
