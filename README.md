<h1 align="center">Teerasak Mairoddee</h1>

<p align="center">
  <b>Software. Security. Hardware. Built into one system.</b><br>
  UK-based engineer building resilient, security-first technology for defence and edge environments.
</p>

---

## The mission

I started out writing software. Then I learned how software breaks, and moved into security. Then I wanted to build things you can hold, so I added hardware.

Now I combine all three. Writing code is no longer the hard part. The hard part is building something that works in the real world: it runs when the network is down, holds up when someone attacks it, and gives the person using it the information they need when it counts.

That is why I'm drawn to **defence technology**. It is the one field that needs everything at once. Embedded hardware, radio links, computer vision, secure architecture and software that cannot fail quietly. Every skill I have has a place there.

> I don't build demos. I build working systems, test them, and record what they can and cannot do.

---

## Current build: ENTITY (Edge Node To TAK)

An offline person-detection system that sends alerts from the edge to a common operational picture, with no internet and no cloud.

```
 Camera ─▶ YOLO on the node ─▶ Encrypted LoRa (868 MHz) ─▶ Gateway ─▶ TAK server (mutual TLS) ─▶ iTAK / ATAK
```

- **Sense:** a camera node runs YOLO person detection locally on CPU.
- **Transmit:** a compact event (180 bytes or less) goes over Meshtastic LoRa on a private, keyed channel.
- **Deliver:** the gateway checks each event, converts it to Cursor-on-Target and pushes it through a local TAK server to a phone over mutual TLS.
- **Ship:** one-click setup for each side, an operator console, automated tests, and tagged releases built and tested in CI that refuse to package anything that looks like a secret.

**Bench results so far:** 20 of 20 events delivered with no losses and no duplicates. Median delay from detection to gateway is 1.85 seconds (p95 2.21 s). Live webcam detections appear as markers in iTAK.

Next: range and outdoor testing, several nodes at once, battery life and detection accuracy. It is a prototype, and the record says exactly what has been proven so far.

---

## Capabilities

**Offensive and defensive security**
Level 4 Cyber Security trained, focused on practical penetration testing: reconnaissance and enumeration, web app testing, SQL injection, OAuth and JWT attacks, Linux privilege escalation, traffic analysis, and physical / USB HID attack research.

`Kali` `Nmap` `Burp Suite` `Metasploit` `Wireshark` `SQLMap` `Hydra` `Gobuster` `LinPEAS`

**Secure delivery (DevSecOps)**
Security belongs in the pipeline from the first commit, not added at the end.

`GitHub Actions` `Docker` `CodeQL` `Semgrep` `Trivy` `Gitleaks` `Secret detection` `Checksummed releases`

**Hardware and edge**
Systems that sense, decide and communicate without the cloud.

`ESP32` `Raspberry Pi` `Heltec LoRa` `Meshtastic` `OpenCV` `YOLO` `TAK / CoT` `I²C sensors`

**Software engineering**
From embedded C++ to full-stack web apps and AI tooling.

`Python` `TypeScript` `JavaScript` `C++ (Arduino)` `PHP` `Bash` `React` `Node.js` `Express` `Linux`

---

## Selected work

| Project | What it shows |
|---|---|
| **ENTITY** | Edge AI, LoRa mesh, TAK integration, mutual TLS, release engineering. Defence-oriented, built end to end. |
| [**P4wnP1 HID Scripting**](https://github.com/Teerasak-Mairoddee/P4wnp1_HID_Scripting) | Physical attack research: a library of USB HID payloads on a Raspberry Pi, run in controlled labs to understand detection and defence. |
| [**ESP32-C3 Desk Buddy**](https://github.com/Teerasak-Mairoddee/esp32-c3-oled-animations) | Embedded firmware: a BMI160 motion sensor triggers animations drawn frame by frame on an SSD1306 OLED. |
| [**Mobile Conversion Assistant**](https://github.com/Teerasak-Mairoddee/mobile_conversion_assistant) | A real operational problem solved in React + TypeScript, built on the tools the business already uses with almost no infrastructure. |
| [**Cover Letter AI**](https://github.com/Teerasak-Mairoddee/cover-letter-ai) | CV parsing and AI generation on a self-hosted Node/Express stack behind a reverse proxy. |

---

## Operating principles

1. **Works offline.** If it needs the cloud to function, it isn't resilient.
2. **Secure by design.** I attack my own systems before anyone else gets the chance.
3. **Tested, not claimed.** Every claim is backed by a test result.
4. **Built to be used.** One-click setup, clear consoles and documentation that someone else can follow.

---

## Open to

Roles in **defence technology, security engineering, embedded and edge systems, and DevSecOps**, where software, security and hardware come together.

[GitHub](https://github.com/Teerasak-Mairoddee)

---

<p align="center"><i>Build it. Break it. Secure it. Deploy it.</i></p>
