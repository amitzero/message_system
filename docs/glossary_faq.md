# Glossary & FAQ

## Glossary

| **Term**                | **Definition**                                                                                                   |
|--------------------------|-----------------------------------------------------------------------------------------------------------------|
| **API**                 | Application Programming Interface, allows communication between software components.                           |
| **JWT**                 | JSON Web Token, a compact token format used for securely transmitting information between parties.              |
| **WebSocket**           | A protocol for real-time, full-duplex communication over a single TCP connection.                              |
| **Kubernetes (K8s)**    | An open-source platform for automating deployment, scaling, and management of containerized applications.       |
| **PostgreSQL**          | An open-source, object-relational database known for its robustness and SQL compliance.                        |
| **Redis**               | An in-memory data structure store used for caching and session management.                                     |
| **S3 (Simple Storage)** | Scalable object storage service, often used for storing files like images, videos, and backups.                |
| **CI/CD**               | Continuous Integration and Continuous Deployment, automates building, testing, and deploying applications.     |
| **TLS/SSL**             | Transport Layer Security / Secure Sockets Layer, ensures secure communication over networks using encryption.  |
| **Flutter**             | An open-source UI software development kit by Google for building natively compiled applications.              |
| **NestJS**              | A progressive Node.js framework for building efficient and scalable server-side applications.                  |
| **Firestore**           | A cloud-hosted NoSQL database by Firebase for scalable, real-time applications.                               |
| **RBAC**                | Role-Based Access Control, a method for regulating access to resources based on roles assigned to users.       |

---

## FAQ

### General

**Q1: What is the purpose of this messaging app?**  
A1: The app is designed for secure, email-based messaging without the need for phone numbers or status updates. It prioritizes privacy, encryption, and a clean user experience.

**Q2: What platforms will the app support?**  
A2: The app will be available for Android, iOS, and as a web application.

**Q3: Why is it email-based?**  
A3: To ensure accessibility for users without requiring a phone number and to enhance privacy.

---

### Technical

**Q4: How is user data secured?**  
A4: Data is encrypted using AES-256 for storage and TLS for transmission. Messages are end-to-end encrypted with a unique key for each conversation.

**Q5: What happens to media files?**  
A5: Media files (e.g., images, videos) are stored in an S3-compatible storage solution. Only authorized users can access these files via pre-signed URLs.

**Q6: How does real-time messaging work?**  
A6: WebSocket servers are used for instant message delivery. The app also uses fallback mechanisms like polling for less capable networks.

**Q7: How are backups handled?**  
A7: Automated daily backups are taken for the database and stored in separate secure regions. Backups are encrypted for safety.

---

### UI/UX

**Q8: What guidelines should UI/UX designers follow?**  
A8: Designers should ensure simplicity and intuitiveness. Follow Material Design principles for mobile apps and provide seamless navigation.

**Q9: Can users customize the interface?**  
A9: Yes, users can enable dark mode, customize chat themes, and adjust notification settings.

---

### Development

**Q10: What technologies are used in the project?**  
A10: Key technologies include:
- **Frontend**: Flutter for Android, iOS, and Web.
- **Backend**: NestJS with Node.js.
- **Database**: PostgreSQL and Firestore.
- **Real-Time Messaging**: WebSocket protocols.
- **Caching**: Redis.

**Q11: How is the CI/CD pipeline implemented?**  
A11: GitHub Actions are used for continuous integration, Docker for containerization, and Kubernetes for orchestration.

---

### Troubleshooting

**Q12: What to do if a message fails to send?**  
A12: The app automatically retries sending messages in case of a failure. If it persists, check the network connection or app logs.

**Q13: How to handle login issues?**  
A13: Users can reset their passwords via the email-based recovery process. For further assistance, contact support.

**Q14: What if a user's email is compromised?**  
A14: Recommend the user update their email credentials and enable multi-factor authentication if available.

---

### Future Enhancements

**Q15: What features might be added later?**  
A15: Planned features include:
- Multi-device support.
- Scheduled message delivery.
- Voice and video calling.
- Team collaboration

**Q16: Can the app support custom emojis or stickers?**  
A16: Yes, custom emoji and sticker packs are planned for a future release.

---
