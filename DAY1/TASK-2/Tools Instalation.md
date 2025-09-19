# Task-2: Tool & PDK Installation Proof

This folder contains screenshots verifying installation of all required tools and the SkyWater PDK on Ubuntu 20.04+.

---

## 🔹 Tools Installed and Verified

1. ✅ **Yosys**
   - Command: `yosys -V`
   - Screenshot: `yosys.png`

2. ✅ **Icarus Verilog**
   - Command: `iverilog -V`
   - Screenshot: `iverilog.png`

3. ✅ **GTKWave**
   - Command: `gtkwave --version`
   - Screenshot: `gtkwave.png`

4. ✅ **ngspice**
   - Command: `ngspice -v`
   - Screenshot: `ngspice.png`

5. ✅ **Magic (Layout Tool)**
   - Command: `magic` (startup banner / GUI)
   - Screenshot: `magic.png`

6. ✅ **Docker**
   - Command: `docker --version`
   - Screenshot: `docker.png`

7. ✅ **OpenLane**
   - Command: `make test` inside `~/OpenLane`
   - Screenshot: `openlane.png`

---

## 🔹 SkyWater PDK Verification (sky130A)

- Verified Magic integration with **Sky130A PDK**:  
  ```bash
  magic -T /usr/local/share/pdk/sky130A/libs.tech/magic/sky130A.tech
  - Screenshot: `skypdk.png`

