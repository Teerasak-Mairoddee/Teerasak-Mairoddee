<h1 align="center">TEERASAK MAIRODDEE</h1>

<p align="center">
  <b>I build systems that work when everything else fails.</b><br>
  Software · Security · Hardware · Defence Technology
</p>

---

## Origin

I started out writing software.
I learned how to break it, so I moved into security.
I wanted to build things you can pick up and deploy, so I added hardware.

Now all three are one discipline.

Coding has changed. Writing code is no longer the hard part. What matters now is **impact**: systems that run with no network, survive an attacker, and put the right information in front of the right person when it counts.

That is why I build for **defence**. It is the one field that demands everything at once: embedded hardware, radio, computer vision, hardened architecture, and software that cannot be allowed to fail quietly. Every skill I have is useful there.

---

## Current build: ENTITY

**Edge Node To TAK.** Offline person detection, from sensor to operator. No cloud. No internet. No single point of failure.

```
 [ CAMERA ] ──▶ [ YOLO, on the node ] ──▶ [ ENCRYPTED LoRa 868 MHz ] ──▶ [ GATEWAY ] ──▶ [ TAK, mutual TLS ] ──▶ [ iTAK / ATAK ]
```

| | |
|---|---|
| **Detect** | YOLO person detection runs locally on the node. Nothing leaves the device but the alert. |
| **Transmit** | A compact event of 180 bytes or less goes over Meshtastic LoRa on a private, keyed channel. |
| **Deliver** | The gateway validates each event, converts it to Cursor-on-Target and pushes it through a local TAK server over mutual TLS. |
| **Deploy** | One-click setup for each side, an operator console, automated tests, and CI-built releases that refuse to ship anything that looks like a secret. |

**Bench record:** 20 of 20 events delivered. Zero lost, zero duplicated. Median 1.85 s from detection to gateway (p95 2.21 s). Live detections land as markers on the operator's phone.

**Next:** range, multi-node, endurance and accuracy trials. Nothing is claimed until it has been tested.

---

## Arsenal

**Offence and defence.** Level 4 Cyber Security trained. Reconnaissance, web app exploitation, SQL injection, OAuth and JWT attacks, Linux privilege escalation, traffic analysis, and physical USB HID attacks.
`Kali` `Nmap` `Burp Suite` `Metasploit` `Wireshark` `SQLMap` `Hydra` `Gobuster` `LinPEAS`

**Hardened delivery.** Security goes into the pipeline from the first commit.
`GitHub Actions` `Docker` `CodeQL` `Semgrep` `Trivy` `Gitleaks` `Secret detection` `Checksummed releases`

**Hardware and edge.** Sense, decide and communicate without the cloud.
`ESP32` `Raspberry Pi` `Heltec LoRa` `Meshtastic` `OpenCV` `YOLO` `TAK / CoT` `I²C sensors`

**Software.** From embedded C++ to full-stack web and AI tooling.
`Python` `TypeScript` `JavaScript` `C++` `PHP` `Bash` `React` `Node.js` `Express` `Linux`

---

## Field record

| Build | Capability proven |
|---|---|
| **ENTITY** | Edge AI, LoRa mesh, TAK integration, mutual TLS, release engineering. Built end to end. |
| [**P4wnP1 HID Scripting**](https://github.com/Teerasak-Mairoddee/P4wnp1_HID_Scripting) | Physical attack research: USB HID payloads on a Raspberry Pi, run in controlled labs to understand detection and defence. |
| [**ESP32-C3 Desk Buddy**](https://github.com/Teerasak-Mairoddee/esp32-c3-oled-animations) | Embedded firmware: a BMI160 motion sensor drives frame-by-frame animation on an SSD1306 OLED. |
| [**Mobile Conversion Assistant**](https://github.com/Teerasak-Mairoddee/mobile_conversion_assistant) | A real operational problem solved in React + TypeScript with almost no infrastructure. |
| [**Cover Letter AI**](https://github.com/Teerasak-Mairoddee/cover-letter-ai) | CV parsing and AI generation on a self-hosted Node/Express stack behind a reverse proxy. |

---

## Doctrine

1. **No cloud dependency.** If it needs the internet to work, it isn't resilient.
2. **Attack it first.** I break my own systems before anyone else can.
3. **Evidence over claims.** Every number on this page comes from a test.
4. **Built to be deployed.** One click to set up, clear to operate, documented so someone else can run it.

---

## Open to

Roles in **defence technology, security engineering, embedded and edge systems, and DevSecOps**, where software, security and hardware come together.

---

<p align="center"><b><i>Build it. Break it. Secure it. Deploy it.</i></b></p>
