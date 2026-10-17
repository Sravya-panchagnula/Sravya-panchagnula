### Sravya Panchagnula
Engineer — VLSI/ASIC physical design, embedded flight software, spacecraft OBC/mainframe integration & test.

Background spans RTL-to-GDSII chip design on the open-source Yosys/OpenROAD/OpenLane flow, embedded C flight-software development on NASA's Core Flight System (cFS), ground-segment/SDR systems work, and hands-on Assembly, Integration & Testing on a real spacecraft mission.

---

**VLSI / ASIC Design**
- **RISC-V-based SoC — cache controller + ML accelerator, for space telemetry anomaly detection.** RTL design of radiation-hardening building blocks (TMR voting, Hamming-based SECDED memory protection, INT8 MAC accelerator, CCSDS-style telemetry parser) with a Python/NumPy golden-reference model, verified in Vivado, carried through a full open-source RTL-to-GDSII flow — DRC-clean, LVS-clean, zero timing violations.
- **Onboard AI accelerator — radiation-hardened satellite image classifier.** 4x4 INT8 weight-stationary systolic array (16 PEs), TMR-protected classification score, ECC-checked weight memory, trained via gradient descent and verified bit-exact against the golden model, carried through RTL-to-GDSII.
- **Single-cycle RV32I CPU core.** From-scratch RISC-V base integer core, verified against an independently-computed golden model, carried through RTL-to-GDSII with a fully clean signoff — 0 DRC, 0 LVS errors, 0 antenna violations, 0 timing violations.
- **Asynchronous (dual-clock) FIFO.** Gray-code pointer synchronization across genuinely unrelated clock domains, verified with a 2000-word randomized self-checking testbench, carried through RTL-to-GDSII.

**Flight Software / Ground Segment / Embedded Systems**
- **CubeSat ground-to-space command & telemetry prototype.** A 3-node system — BeagleBone Black OBC running a custom NASA cFS application, an ADALM-Pluto SDR TT&C radio, and an ADS-B payload — with a dual-mode downlink (live streaming vs. onboard store-and-forward), a real CCSDS TM chain (convolutional coding, PRBS scrambling, frame sync), and a from-scratch ground decoder feeding a live mission dashboard.

**Spacecraft Assembly, Integration & Testing**
- AIT Engineer on ISRO's SPADEX (Space Docking Experiment) mission — mainframe (core bus) subsystem checkout: OBC, AOCS, power, and mechanisms, verifying functional readiness ahead of qualification and pre-launch testing.

---

Most repositories here are kept private; happy to share access on request.
