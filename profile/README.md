<p align="center">
  <img src="assets/tesaiot-ecosystem.jpg" alt="TESAIoT Ecosystem — Build, Develop, Learn, Apply" width="100%">
</p>

<h1 align="center">TESAIoT Foundation</h1>

<p align="center">
  <b>Secure · Intelligent · Connected</b><br>
  From secure Edge AI hardware to real-world solutions, by the Thai Embedded Systems Association (TESA)<br>
  จากฮาร์ดแวร์ Edge AI ที่ปลอดภัย สู่โซลูชันที่ใช้งานได้จริง โดยสมาคมสมองกลฝังตัวไทย (TESA)
</p>

<p align="center">
  <a href="https://www.tesaiot.com"><img alt="Website" src="https://img.shields.io/badge/web-tesaiot.com-1f6feb"></a>
  <a href="https://tesaiot.github.io/tesaiot-pse84-devkit-sdk/"><img alt="SDK docs" src="https://img.shields.io/badge/docs-Dev%20Kit%20SDK-2ea44f"></a>
  <a href="https://tesaiot.github.io/developer-hub/"><img alt="Developer Hub" src="https://img.shields.io/badge/Developer%20Hub-open-8957e5"></a>
  <a href="https://www.tesa.or.th"><img alt="TESA" src="https://img.shields.io/badge/TESA-tesa.or.th-d73a49"></a>
  <a href="https://www.linkedin.com/company/93718897"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-TESA-0a66c2"></a>
</p>

<p align="center"><b>Choose your language · เลือกภาษา</b><br><sub>Click a heading below to open or close it · กดที่หัวข้อด้านล่างเพื่อเปิดหรือปิด</sub></p>

<details open>
<summary><h2>🇬🇧 English</h2></summary>

### What we build

TESAIoT is an open, end-to-end AIoT foundation for products that must be secure from the first line of firmware: device identity, encrypted connectivity, Edge AI on the device and analytics in the cloud. It is designed for regulated industries and mission-critical systems, and ready for cybersecurity labelling (CLS, ETSI EN 303 645).

It is built in Thailand, documented in Thai and English, and open source under Apache-2.0 wherever TESA wrote the code.

<p align="center">
  <img src="assets/secure-edge-ai-economy-platform.jpg" alt="Secure Edge AI Economy Platform: AIoT foundation, core modules and product development, commercial scaling" width="100%">
</p>

| Layer | What it gives you |
|---|---|
| **1 · AIoT Foundation** | AIoT SoM and BSP (ModusToolbox, Zephyr OS, MicroPython), a secure firmware stack that is CLS-ready, DEEPCRAFT Studio for Edge AI models, Digital Twin Studio, and a secure Edge AI data platform |
| **2 · Core modules and product development** | TESAIoT Dev Kit, IoT gateway, BCU/BMS, actuators, the Ternion Digital Twin Studio and enterprise cloud |
| **3 · Commercial scaling** | Healthcare, LEV and energy, service robotics, critical infrastructure and creative industries |

### Start here: our open repositories

| Repository | What it is | Start with |
|---|---|---|
| [**tesaiot-pse84-devkit-sdk**](https://github.com/tesaiot/tesaiot-pse84-devkit-sdk) | Firmware stack and SDK for the Infineon PSoC™ Edge E84: ModusToolbox and ModusToolbox + MicroPython project templates, C examples, API reference, and firmware tested on real boards. | [Docs](https://tesaiot.github.io/tesaiot-pse84-devkit-sdk/) · [Latest firmware](https://github.com/tesaiot/tesaiot-pse84-devkit-sdk/releases/latest) |
| [**tesaiot-community-edition**](https://github.com/tesaiot/tesaiot-community-edition) | A free, self-hostable secure IoT platform for one organization: Vault PKI device identity (server-TLS and mTLS), EMQX MQTT broker, APISIX gateway, MongoDB + TimescaleDB telemetry. One-command Docker Compose install. | [Overview](https://www.tesaiot.com/#community-edition) |
| [**developer-hub**](https://github.com/tesaiot/developer-hub) | One hub across the whole stack: firmware on the MCU, middleware on the edge, web applications in the browser. Remix any example and ship. | [Open the hub](https://tesaiot.github.io/developer-hub/) |
| [**tesa-qualification-program**](https://github.com/tesaiot/tesa-qualification-program) | TESA Open Knowledge: open learning material for embedded systems, AIoT and Edge AI, and the TESA Qualification Program (TESA × Infineon). | [Course site](https://tesaiot.github.io/tesa-qualification-program/) |

### TESAIoT Dev Kit: hardware and the firmware that runs on it

A three-core Edge AI board, shipped with its whole firmware as an open SDK. It boots to a touch menu, reads every sensor, runs MicroPython, talks TLS to the cloud and runs an Edge AI model on the NPU.

- **Silicon:** Cortex-M55 at 400 MHz with Helium and an Ethos-U55 NPU, plus 2 × Cortex-M33 with TrustZone. Wi-Fi 6 and BLE. 4.3" touch display.
- **Security:** an OPTIGA™ Trust M hardware root of trust, secure boot, HSM-backed device identity, and mTLS where the private key never leaves the silicon.
- **Open source:** about 237,000 lines of C and 60+ public APIs, with 31 C examples in the tree.
- **Documentation:** 838 pages in Thai and English.
- **Two ways to build:** pure C with ModusToolbox, or C + MicroPython. Same libraries, same board.

```bash
git clone https://github.com/tesaiot/tesaiot-pse84-devkit-sdk.git
cd tesaiot-pse84-devkit-sdk/bento-firmware-template-mtb-mpy   # or bento-firmware-template-mtb-only
./setup.sh --build      # checks the toolchain first, then builds
make program            # then unplug USB fully, wait ten seconds, plug back in
```

Each firmware release publishes its `.hex` with a SHA-256 checksum: the same file we flash on our own test boards.

### The AIoT Foundation Platform

<p align="center">
  <img src="assets/aiot-foundation-platform.jpg" alt="Overall AIoT Foundation Platform: device, embedded OS, backend and frontend layers" width="100%">
</p>

- **Security by design:** ETSI EN 303 645 cybersecurity compliance, a 4-tier PKI with automated certificate issuance and renewal, and HSM key protection.
- **Secure AIoT connectivity:** MQTTs and HTTPS with server-TLS or mTLS, plus hardware-based onboarding with the Infineon OPTIGA™ Trust M factory certificate.
- **Smart data:** schemas for industrial domains, validated live telemetry, and ETL with data labelling for Edge AI.
- **Digital Twin:** real-time product design and development on the device's live data.

<p align="center">
  <img src="assets/tesaiot-platform-use-cases.jpg" alt="TESAIoT Platform: edge identity and authentication, foundation services, applications and use cases" width="100%">
</p>

### Where it is used

| Domain | Examples |
|---|---|
| **Healthcare IoT** | Fall detection for seniors on the edge, vital-signs monitoring, baby cry and siren recognition, PDPA-aware data handling |
| **Industry 4.0** | Factory alarm detection with audio AI, predictive maintenance, visual inspection, OT network segmentation |
| **Smart energy** | Energy-efficient edge computing, grid integration, EV charging optimization, solar and battery forecasting |
| **Smart home and city** | TLS and key storage on the device, Matter provisioning, accessory authentication, product activation |
| **Mobility** | Cars and light electric vehicles: advanced security with a TPM, car access, accessory authentication |

<p align="center">
  <img src="assets/accelerated-product-development.jpg" alt="Accelerated product development: from core boards and firmware to applications, services and data analytics" width="100%">
</p>

### Learn with us

- **Video course:** 28 episodes, about 4 hours 18 minutes, recorded on real hardware: the platform overview, getting firmware onto the board, the Digital Twin, and the BitStream Studio course. See [tesaiot.com](https://www.tesaiot.com).
- **TESA Qualification Program:** open courseware for embedded systems, AIoT and Edge AI. See [tesa-qualification-program](https://tesaiot.github.io/tesa-qualification-program/).
- **Developer Hub:** examples across firmware, middleware and the web. See [developer-hub](https://tesaiot.github.io/developer-hub/).

### License and contact

Source written by TESA is released under the **Apache License 2.0**. A small number of third-party libraries keep their own licences; each repository names them.

Website: [www.tesaiot.com](https://www.tesaiot.com) · [www.tesa.or.th](https://www.tesa.or.th) · Email: [contact@tesa.or.th](mailto:contact@tesa.or.th)

</details>

<details>
<summary><h2>🇹🇭 ภาษาไทย</h2></summary>

### TESAIoT คืออะไร

TESAIoT คือ AIoT Foundation Platform แบบ open และ end-to-end สำหรับผลิตภัณฑ์ที่ต้อง secure ตั้งแต่ firmware บรรทัดแรก ครอบคลุม device identity, encrypted connectivity, Edge AI บนตัวอุปกรณ์ และ data analytics บน cloud ออกแบบมาสำหรับ regulated industries และ mission-critical systems พร้อมรองรับ Cybersecurity Labelling Scheme (CLS, ETSI EN 303 645)

พัฒนาในประเทศไทย มีเอกสารทั้งภาษาไทยและอังกฤษ และเป็น open source ภายใต้ Apache-2.0 ในทุกส่วนที่ TESA เป็นผู้เขียน

<p align="center">
  <img src="assets/secure-edge-ai-economy-platform.jpg" alt="Secure Edge AI Economy Platform by TESAIoT" width="100%">
</p>

| Layer | สิ่งที่ได้ |
|---|---|
| **1 · AIoT Foundation** | AIoT SoM & BSP (ModusToolbox, Zephyr OS, MicroPython), Secure Firmware Stack ที่ CLS-ready, DEEPCRAFT Studio สำหรับ Edge AI model, Digital Twin Studio และ Secure Edge AI Data Platform |
| **2 · Core Modules & Product Development** | TESAIoT Dev Kit, IoT Gateway, BCU/BMS, Intelligence Actuator, Ternion Digital Twin Studio และ Enterprise Cloud |
| **3 · Commercial Scaling** | Healthcare, LEV & Energy, Service Robotics, Critical Infrastructure และ Creative Industries |

### เริ่มต้นที่ open repositories ของเรา

| Repository | คืออะไร | เริ่มที่ |
|---|---|---|
| [**tesaiot-pse84-devkit-sdk**](https://github.com/tesaiot/tesaiot-pse84-devkit-sdk) | TESAIoT Firmware Stack & SDK สำหรับ Infineon PSoC™ Edge E84 — project template แบบ ModusToolbox และ ModusToolbox + MicroPython พร้อมตัวอย่าง C, API reference และ firmware ที่ทดสอบบนบอร์ดจริงแล้ว | [Docs](https://tesaiot.github.io/tesaiot-pse84-devkit-sdk/) · [Latest firmware](https://github.com/tesaiot/tesaiot-pse84-devkit-sdk/releases/latest) |
| [**tesaiot-community-edition**](https://github.com/tesaiot/tesaiot-community-edition) | Secure IoT platform ที่ใช้ฟรีและ self-host ได้สำหรับหนึ่งองค์กร — Vault PKI device identity (server-TLS & mTLS), EMQX MQTT broker, APISIX gateway, telemetry บน MongoDB + TimescaleDB ติดตั้งด้วย Docker Compose คำสั่งเดียว | [Overview](https://www.tesaiot.com/#community-edition) |
| [**developer-hub**](https://github.com/tesaiot/developer-hub) | Hub เดียวที่ครอบคลุมทั้ง stack — firmware บน MCU, middleware บน edge และ web application บน browser นำตัวอย่างไป remix ต่อได้ทันที | [Developer Hub](https://tesaiot.github.io/developer-hub/) |
| [**tesa-qualification-program**](https://github.com/tesaiot/tesa-qualification-program) | TESA Open Knowledge — คลังความรู้เปิดด้าน Embedded Systems, AIoT และ Edge AI และหลักสูตร TESA Qualification Program (TESA × Infineon) | [Course site](https://tesaiot.github.io/tesa-qualification-program/) |

### TESAIoT Dev Kit: hardware พร้อม firmware ที่รันอยู่บนบอร์ดจริง

Edge AI board แบบ 3 core ที่มาพร้อม firmware ทั้งหมดในรูป open SDK — boot ขึ้นมาเป็น touch menu อ่าน sensor ได้ทุกตัว รัน MicroPython คุยกับ cloud ผ่าน TLS และรัน Edge AI model บน NPU

- **Silicon:** Cortex-M55 400 MHz + Helium + Ethos-U55 NPU และ Cortex-M33 อีก 2 core พร้อม TrustZone, Wi-Fi 6 + BLE, 4.3" touch display
- **Security:** OPTIGA™ Trust M เป็น hardware root of trust, secure boot, HSM-backed device identity และ mTLS ที่ private key ไม่เคยออกจาก silicon
- **Open source:** C ประมาณ 237,000 บรรทัด, public API มากกว่า 60 ตัว และ C example 31 ตัวใน repo
- **Documentation:** 838 หน้า ภาษาไทยและอังกฤษ
- **Build ได้ 2 แบบ:** C ล้วนด้วย ModusToolbox หรือ C + MicroPython ใช้ library ชุดเดียวกัน บนบอร์ดเดียวกัน

```bash
git clone https://github.com/tesaiot/tesaiot-pse84-devkit-sdk.git
cd tesaiot-pse84-devkit-sdk/bento-firmware-template-mtb-mpy   # หรือ bento-firmware-template-mtb-only
./setup.sh --build      # ตรวจ toolchain ก่อน แล้วจึง build
make program            # จากนั้นถอด USB ออกจนสุด รอ 10 วินาที แล้วเสียบใหม่
```

Firmware ทุก release มีไฟล์ `.hex` พร้อม SHA-256 — เป็นไฟล์เดียวกับที่เรา flash ลงบอร์ดทดสอบของเราเอง

### AIoT Foundation Platform

<p align="center">
  <img src="assets/aiot-foundation-platform.jpg" alt="Overall AIoT Foundation Platform" width="100%">
</p>

- **Security by Design:** สอดคล้อง ETSI EN 303 645, 4-tier PKI ที่ออกและ renew certificate อัตโนมัติ และ HSM key protection
- **Secure AIoT Connectivity:** MQTTs & HTTPS แบบ server-TLS หรือ mTLS และ hardware-based onboarding ด้วย factory certificate ของ Infineon OPTIGA™ Trust M
- **Smart Data Schema & Industrial Domains:** validation และ live telemetry พร้อม ETL และ data labelling สำหรับ Edge AI
- **Digital Twin:** real-time product design & development บน live data จากอุปกรณ์

<p align="center">
  <img src="assets/tesaiot-platform-use-cases.jpg" alt="TESAIoT Platform: edge identity & authentication, applications & use cases" width="100%">
</p>

### Applications & Use Cases

| Domain | ตัวอย่าง |
|---|---|
| **Healthcare IoT** | Fall detection สำหรับผู้สูงอายุด้วย Edge AI, vital signs monitoring, baby cry & siren recognition, รองรับ PDPA |
| **Industry 4.0** | Factory alarm detection ด้วย audio AI, predictive maintenance, visual inspection, OT network segmentation |
| **Smart Energy** | Energy-efficient edge computing, smart grid integration, EV charging optimization, solar & battery forecasting |
| **Smart Home & City** | TLS & key storage บนอุปกรณ์, Matter provisioning, accessory authentication, product activation |
| **Mobility (Car & LEVs)** | Advanced security ด้วย TPM, Car Access (CCC), accessory authentication |

<p align="center">
  <img src="assets/accelerated-product-development.jpg" alt="Accelerated Product Development" width="100%">
</p>

### Learn with us

- **Video course:** 28 ตอน รวมประมาณ 4 ชั่วโมง 18 นาที บันทึกกับ hardware จริง — platform overview, การ flash firmware ลงบอร์ด, Digital Twin และ BitStream Studio course ดูได้ที่ [tesaiot.com](https://www.tesaiot.com)
- **TESA Qualification Program:** open courseware ด้าน Embedded Systems, AIoT และ Edge AI ที่ [tesa-qualification-program](https://tesaiot.github.io/tesa-qualification-program/)
- **Developer Hub:** ตัวอย่างครบทั้ง firmware, middleware และ web ที่ [developer-hub](https://tesaiot.github.io/developer-hub/)

### License & Contact

Source code ที่ TESA เป็นผู้เขียนเผยแพร่ภายใต้ **Apache License 2.0** ส่วน third-party library บางตัวใช้ license ของตัวเอง ซึ่งแต่ละ repo ระบุไว้แล้ว

Website: [www.tesaiot.com](https://www.tesaiot.com) · [www.tesa.or.th](https://www.tesa.or.th) · Email: [contact@tesa.or.th](mailto:contact@tesa.or.th)

</details>

<p align="center"><sub>Together, we build a smarter, safer and more connected future. · ร่วมกันสร้างอนาคตที่ฉลาดขึ้น ปลอดภัยขึ้น และเชื่อมต่อกันมากขึ้น</sub></p>
