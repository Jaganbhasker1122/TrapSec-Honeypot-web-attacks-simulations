# TrapSec

An interactive web-based educational simulation demonstrating common web attack vectors and their mitigation techniques.

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Project Type](https://img.shields.io/badge/type-Educational%20Simulation-blue)]()
[![Status](https://img.shields.io/badge/status-stable-brightgreen)]()

---

## Table of Contents

1. [Problem Statement](#problem-statement)
2. [What is TrapSec](#what-is-trapsec)
3. [Simulated Attacks](#simulated-attacks)
4. [Features](#features)
5. [Quick Start](#quick-start)
6. [How to Use](#how-to-use)
7. [Architecture](#architecture)
8. [Educational Use Cases](#educational-use-cases)
9. [Limitations](#limitations)
10. [Future Scope](#future-scope)
11. [Contributing](#contributing)
12. [License](#license)
13. [Author](#author)

---

## Problem Statement

Cybersecurity education requires hands-on practice with attack scenarios. However, setting up real attack environments is complex, risky, and resource-intensive. Many students and professionals learn security theory without understanding how attacks actually manifest in practice.

**Key challenges in security education:**
- Real attack environments are difficult to set up safely
- Learning from theory alone doesn't build practical understanding
- Observing attack behavior firsthand improves retention and awareness
- Interactive demonstrations help bridge the gap between textbook knowledge and real-world threats

TrapSec addresses this by providing a safe, browser-based platform to observe and understand common web attacks without deploying actual malicious code or infrastructure.

---

## What is TrapSec

TrapSec is an interactive, web-based **educational simulation** that demonstrates how common web attacks work. It provides visual and interactive representations of attacks like SQL injection, XSS, and phishing—allowing learners to see attack mechanics without actual compromise or data breach.

**Important:** TrapSec is **not a real honeypot**. It does not detect actual attacks, monitor live systems, or perform threat analysis. Instead, it simulates attack behavior for educational purposes.

**Use TrapSec to:**
- Understand attack vectors and methodologies
- Learn how vulnerabilities are exploited
- Recognize warning signs and defensive patterns
- Build security awareness through interactive learning

---

## Simulated Attacks

### SQL Injection
Demonstrates how malicious SQL code can be injected into input fields to manipulate database queries. Shows how attackers can bypass authentication, extract data, or modify records.

### Cross-Site Scripting (XSS)
Illustrates how malicious JavaScript code can be injected into web pages. Shows how attackers can steal session cookies, perform unauthorized actions, or redirect users to malicious sites.

### Denial of Service (DoS)
Simulates flooding a server with excessive requests to exhaust resources and make services unavailable. Educational simulation only; no actual network traffic generated.

### Keylogger
Demonstrates how keystrokes can be intercepted and logged. Shows the attack flow and impact on user privacy and security. Simulation only; no actual keystroke capture occurs.

### Adware
Displays simulated malicious advertisements and pop-ups. Illustrates how unwanted software can be bundled with legitimate applications and negatively impact user experience.

### Malicious File Download
Simulates scenarios where users download files that appear legitimate but contain malware. Educates on file type spoofing and social engineering techniques.

### Phishing
Shows how fake login forms and fraudulent emails can trick users into revealing credentials. Demonstrates visual similarities to legitimate sites and common phishing patterns.

---

## Features

### Interactive Demonstrations
- Visual, hands-on demonstrations of each attack vector
- Step-by-step simulation of attack execution
- Real-time feedback and interaction

### Educational Content
- Detailed explanations of each attack mechanism
- Information about real-world implications
- Countermeasures and defensive strategies for each attack

### User-Friendly Design
- Centralized navigation hub
- Clear visual organization
- Responsive interface suitable for different screen sizes

### Mitigation Guidance
- Best practices for preventing each type of attack
- Security recommendations for developers and users
- Defense-in-depth strategies

---

## Quick Start

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or backend setup required

### Running Locally

1. Clone the repository:
```bash
git clone https://github.com/Jaganbhasker1122/TrapSec.git
cd TrapSec
```

2. Open `index.html` in your web browser:
```bash
# Option 1: Direct file open
open index.html

# Option 2: Using a local web server (recommended)
python -m http.server 8000
# Then navigate to http://localhost:8000
```

3. Explore the available simulations from the home page.

### Live Demo
Access the deployed version: [TrapSec Live Demo](https://honeypot-web-simulation.netlify.app/index.html)

---

## How to Use

1. **Start at Home**: Open `index.html` to access the main navigation hub
2. **Select an Attack**: Choose a simulation from the available options
3. **Interact with Simulation**: Follow the on-screen instructions to observe the attack
4. **Read Explanations**: Review the detailed information cards explaining:
   - How the attack works
   - Real-world impact
   - Detection methods
   - Prevention techniques
5. **Learn Defenses**: Understand countermeasures and security best practices
6. **Explore Others**: Navigate back to try other attack simulations

---

## Architecture

### Project Structure

```
TrapSec/
├── index.html                 # Main home page and navigation hub
├── style.css                  # Global styling
├── try-now.css               # Specific styling for demos
│
├── Simulations/
│   ├── sqlinjection.html      # SQL injection demonstration
│   ├── xss.html              # XSS attack demonstration
│   ├── DOS.html              # Denial of Service simulation
│   ├── keylogger.html        # Keylogger behavior demonstration
│   ├── adware.html           # Adware simulation
│   ├── maliciousfile.html    # File download attack simulation
│   └── phishing.html         # Phishing form demonstration
│
├── Educational Pages/
│   ├── simulated-attacks.html # Overview of all attacks
│   ├── learn-more.html        # Detailed learning resources
│   ├── protect-yourself.html  # Defense and protection guide
│   └── try-now.html          # Getting started guide
│
├── assets/
│   └── images/                # Screenshots and visual assets
│
└── package-lock.json         # Dependency metadata

```

### Design Approach

**Frontend-Only:** All simulations run in the browser using HTML, CSS, and JavaScript. No backend server is required.

**Self-Contained:** Each simulation is an independent HTML file that can be viewed in isolation.

**Educational Focus:** Simulations prioritize clear demonstration over technical realism.

**Static Content:** No persistent data storage, logging, or dynamic content generation.

---

## Educational Use Cases

### For Computer Science Students
Understand practical attack mechanisms and security concepts covered in coursework. Build intuition about vulnerability exploitation and defense strategies.

### For Cybersecurity Role Preparation
Prepare for interviews and entry-level security positions by demonstrating knowledge of common attack vectors and defensive techniques.

### For Awareness Training
Use in security awareness programs to educate non-technical staff about phishing, social engineering, and safe computing practices.

### For Instructors
Incorporate into classroom lessons as interactive demonstrations of security concepts. Help students visualize attack flows and understand real-world implications.

### For Self-Paced Learning
Independent study resource for building foundational security knowledge without requiring access to lab environments or real systems.

---

## Limitations

TrapSec is an **educational simulation only**. The following limitations should be clearly understood:

### Not a Real Honeypot
- Does not detect actual attacks or monitor live systems
- Does not interact with real networks or services
- Does not generate actual malicious traffic or payloads
- Cannot be used for production threat monitoring

### Simulations Are Simplified
- Attack demonstrations are educational representations, not exact replicas
- User interactions trigger predefined simulated responses
- No actual code execution or system compromise occurs
- Visual effects and flow are designed for learning, not technical accuracy

### No Actual Attack Mechanics
- SQL injection simulation does not execute real SQL queries against databases
- XSS demonstrations do not inject scripts into actual web pages
- DoS simulation does not generate network requests or flood servers
- Keylogger simulation does not capture actual keystroke data
- Phishing simulation uses forms that do not transmit credentials

### Scope Boundaries
- Focuses on common web attacks; network, infrastructure, and advanced attack vectors not covered
- Educational only; not suitable for research, penetration testing, or production security work
- No threat intelligence integration or attack analysis
- No logging or audit trail functionality

### Technical Constraints
- Browser-based only; requires JavaScript enabled
- No persistence or data storage between sessions
- Static content; cannot adapt to user input or real-world scenarios
- No authentication or access control mechanisms

---

## Future Scope

### Short-Term Enhancements
- Additional attack simulations (CSRF, XXE, NoSQL injection)
- Interactive quizzes to test understanding
- Video explanations of attack concepts
- Downloadable study guides and reference materials

### Medium-Term Improvements
- Interactive flow diagrams showing attack progression
- Side-by-side code examples showing vulnerable vs. secure implementations
- Glossary of security terminology
- Progress tracking for learners

### Long-Term Additions
- Expanded coverage of emerging threats and attack patterns
- Internationalization for global audience
- Offline version for environments without internet access
- Integration with security certification study materials

---

## Contributing

Contributions are welcome. Please follow these guidelines:

### Areas for Contribution
- New attack simulations (with educational focus)
- Improved explanations and defensive strategies
- Enhanced visual design and user experience
- Documentation and learning materials
- Bug reports and usability feedback

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/description`)
3. Commit your changes with clear messages
4. Push to the branch and open a pull request
5. Include descriptions of your changes and educational value

### Code Standards
- Maintain focus on educational clarity
- Keep simulations browser-compatible
- Use clear, commented code
- Test across multiple browsers before submitting

---

## License

TrapSec is released under the MIT License. See the LICENSE file for details.

---

## Author

**Gurram Jagan Bhasker**  
B.Tech Cyber Security (3rd Year) | India

Cybersecurity enthusiast focused on building educational tools and practical security projects. Interested in application security, threat analysis, and helping others learn cybersecurity concepts.

### Contact and Profiles

- GitHub: [github.com/Jaganbhasker1122](https://github.com/Jaganbhasker1122)
- LinkedIn: [linkedin.com/in/gurram-jagan-bhasker-a0906b29a](https://www.linkedin.com/in/gurram-jagan-bhasker-a0906b29a/)
- Email: jaganbhaskergurram@gmail.com

---

*TrapSec: Learning security through interactive simulation.*
