<p align="center">
  <a href="#">
    <img src="assets/images/Honeypot.png" alt="Honeypot Simulation Logo" width="200" height="165">
  </a>
</p>

<h3 align="center">Honeypot Web Simulation</h3>

<p align="center">
  A comprehensive web-based honeypot simulation to demonstrate various cybersecurity attack scenarios and educate users about security vulnerabilities.
  <br>
  <a href="https://honeypot-web-simulation.netlify.app/index.html"><strong>Explore the Simulation »</strong></a>
  <br>
  <br>
  <a href="#features">Features</a>
  ·
  <a href="#how-to-use">How to Use</a>
  ·
  <a href="#demo">Demo</a>
  ·
  <a href="#contact">Contact</a>
  <br>
</p>

[![Honeypot Web Simulation](assets/images/simulated-attacks.jpg)](https://honeypot-web-simulation.netlify.app/index.html)

## Features

- **Simulated Attacks**:
  - **SQL Injection**: Demonstrates how malicious SQL queries can compromise databases.
  - **Cross-Site Scripting (XSS)**: Explains how attackers can inject malicious scripts into web pages.
  - **Denial of Service (DoS)**: Simulates flooding a server with excessive requests.
  - **Keylogger Simulation**: Showcases how keystrokes can be captured.
  - **Adware**: Displays simulated malicious ads to mimic real-world adware behavior.
  - **Malicious File Downloading**: Warns users about downloading potentially harmful files.
  - **Phishing Simulation**: Demonstrates fake login forms to mimic credential theft.
- **Interactive UI**: User-friendly design with detailed information cards for each attack.
- **Learning Focus**: Explains how each attack works and its real-world implications.
- **Home Navigation**: A central hub to explore different attack simulations.
- **Secure Practices**: Highlights mitigation techniques and best practices for each attack.

## How to Use

1. Navigate to the homepage: [index.html](https://honeypot-web-simulation.netlify.app/index.html).
2. Choose an attack simulation from the menu.
3. Follow the instructions provided in the simulation.
4. Read the detailed explanation and mitigation techniques in the info card.

## Demo

Live Demo: [Honeypot Web Simulation](https://honeypot-web-simulation.netlify.app/index.html)

### Screenshots

**Home Page**

![Home Page](assets/images/Honeypot.png)

**SQL Injection Simulation**

![SQL Injection](assets/images/sqlinjection.png)

**DoS Attack Simulation**

![DoS Attack](assets/images/DOS.png)

**Keylogger Simulation**

![Keylogger](assets/images/keylogger.png)

## Technologies Used

- **HTML5**: For creating the structure.
- **CSS3**: For styling and responsive design.
- **JavaScript**: For implementing attack logic and interactive features.

## Goals and Objectives

- To educate users about cybersecurity threats through hands-on demonstrations.
- To provide detailed insights into attack methodologies and their countermeasures.
- To create an engaging platform for cybersecurity awareness.

## Development

### File Structure

```plaintext
Honeypot-Web-Simulation/
│
├── index.html
├── style.css
├── try-now.css
├── adware.html
├── DOS.html
├── FakeForm.html
├── keylogger.html
├── learn-more.html
├── maliciousfile.html
├── phishing.html
├── protect-yourself.html
├── simulated-attacks.html
├── sqlinjection.html
├── try-now.html
├── xss.html
├── assets/
│   ├── images/
│   │   ├── adware.png
│   │   ├── DOS.png
│   │   ├── fakeform.png
│   │   ├── filedownload.jpg
│   │   ├── Honeypot.png
│   │   ├── keylogger.png
│   │   ├── learn-more.svg
│   │   ├── phishing.png
│   │   ├── protect-yourself.jpg
│   │   ├── simulated-attacks.jpg
│   │   ├── sqlinjection.png
│   │   ├── try-now.png
│   │   ├── xss.png
│
└── .package-lock.json
