# Ridemama 

<div align="center">
  <img src="assets/images/ridemama-logo.png" alt="Ridemama Logo" width="300px">
  <p><em>Connecting Campus Commuters</em></p>
</div>

Ridemama is a student-focused ride-sharing platform built to make daily commutes easier for students whose colleges are far from city centers. It aims to solve the challenges of finding instant rides, reducing daily bus struggles, and enabling smoother, more affordable transportation options.

## 📋 What is the Purpose of this Repository?

This repository serves as a technical walkthrough of the Ridemama platform, providing insights into the architecture, design decisions, and technical challenges faced during its development. Since the actual codebase is private, this repo is meant to demonstrate the engineering skills, problem-solving approaches, and collaborative effort behind the project without exposing sensitive logic.

## 🚀 Key Features

- **Host your own car**: Share your vehicle with fellow students
- **Find rides at your preferred time**: Flexible scheduling that fits your timetable
- **Affordable, constant prices**: No surge pricing regardless of traffic conditions
- **Route selection flexibility**: Choose the best path for your journey
- **Direct payments**: Seamless transactions between riders and hosts
- **Simple, student-friendly interface**: Designed with campus commuters in mind

## 🏗️ System Architecture

<div align="center">
  <img src="assets/images/system-architecture.png" alt="Ridemama System Architecture" width="700px">
</div>

Our architecture follows a microservices approach with these key components:
- Frontend client application
- Backend API services
- Database layer
- Third-party integrations (Maps, Payments, Messaging)

## 🗂️ Database Schema

<div align="center">
  <img src="assets/images/database-erd.png" alt="Ridemama Database ERD" width="700px">
</div>

Our MongoDB schema includes these primary collections:
- Users (riders and hosts)
- Rides (scheduling, routing)
- Payments (transactions)
- Messages (in-app communication)
- Reviews (ratings and feedback)

## ⚙️ Tech Stack

| Component | Technologies |
|-----------|-------------|
| **Frontend** | TypeScript, Next.js, Tailwind CSS |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB (Atlas) |
| **Maps** | Ola Maps by Krutrim |
| **Payments** | Razorpay |
| **Messaging** | Twilio WhatsApp Messaging |
| **Authentication** | JWT |
| **Hosting** | DigitalOcean Droplets |
| **Image Storage** | AWS S3 |
| **Other Tools** | Zod, Docker, GitHub Actions for CI/CD |

## 🚀 Future Improvements

| Feature | Priority | Notes |
|---------|----------|-------|
| WebSocket Integration | High | Real-time ride updates |
| TypeScript Backend Migration | Medium | Better type safety and maintainability |
| RC and DL API Integration | High | For automated vehicle verification |
| Cross-Platform App | Low | Mobile-first approach |
| Bike Registration | Low | Pending insurance and regulatory approval |

## 📸 Screenshots and Visuals

<div align="center">
  <h3>Home Screen</h3>
  <img src="assets/screenshots/home-screen.png" alt="Ridemama Home Screen" width="300px">
  
  <h3>Ride Booking Flow</h3>
  <img src="assets/screenshots/booking-flow.png" alt="Ride Booking Process" width="700px">
  
  <h3>Host Dashboard</h3>
  <img src="assets/screenshots/host-dashboard.png" alt="Host Dashboard" width="500px">
  
  <h3>Payment Interface</h3>
  <img src="assets/screenshots/payment-screen.png" alt="Payment Interface" width="300px">
</div>

## 🛠️ Challenges and Solutions

### Handling real-time updates
*Details to be added*

### Ensuring secure payments
*Details to be added*

### Optimizing ride matching algorithms
*Details to be added*

### Scaling the platform for peak traffic
*Details to be added*

## 📚 Lessons Learned

- **Importance of data consistency**: Maintaining accurate ride information across all system components
- **Balancing speed and security**: Implementing efficient authentication without compromising user experience
- **Managing real-time communication at scale**: Strategies for handling peak-time ride requests

## 👥 Contributors

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/SuryatejPonnapalli">
        <img src="https://github.com/SuryatejPonnapalli.png" width="100px;" alt="Surya's profile picture" style="border-radius:50%;"/><br />
        <sub><b>Surya</b></sub>
      </a><br />
      <sub>Full-stack Developer</sub>
    </td>
     <td align="center">
      <a href="https://github.com/harshith-1008">
        <img src="https://github.com/harshith-1008.png" width="100px;" alt="Harshith's profile picture" style="border-radius:50%;"/><br />
        <sub><b>Harshith</b></sub>
      </a><br />
      <sub>Full-stack Developer</sub>
    </td>
    <td align="center">
      <a href="https://github.com/KDDhanush25">
        <img src="https://github.com/KDDhanush25.png" width="100px;" alt="Dhanush's profile picture" style="border-radius:50%;"/><br />
        <sub><b>Dhanush</b></sub>
      </a><br />
      <sub>Operations and Strategy</sub>
    </td>
    <td align="center">
      <a href="https://github.com/BJVPavan">
        <img src="https://github.com/BJVPavan.png" width="100px;" alt="Pavan's profile picture" style="border-radius:50%;"/><br />
        <sub><b>Pavan</b></sub>
      </a><br />
      <sub>Operations and Market Research</sub>
    </td>
  </tr>
</table>


## 📜 License

MIT License - See [LICENSE](LICENSE) file for details.

## 🔗 Links and References

- [Project Management Tools](#)
- [Relevant Tech Blogs](#)
- [API Documentation](#)

## 🌱 Stay Connected

<div align="center">
  <a href="https://www.linkedin.com/company/ridemama/" target="#">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://www.instagram.com/ridemama_/"  target="#">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
</div>

Follow the journey as we continue to improve Ridemama and expand its reach.

---

<div align="center">
  <img src="assets/images/ridemama-footer.png" alt="Ridemama Footer" width="200px">
  <p><em>Ridemama - Connecting Campus Commuters</em></p>
</div>
