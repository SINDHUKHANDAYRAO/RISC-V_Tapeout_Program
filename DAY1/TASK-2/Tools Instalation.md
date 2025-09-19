# Task-2: Tool & PDK Installation Proof

This folder contains documentation for tool installation verification.  
Screenshots are stored in the `images/` folder.

---

## 🔹 Tools Installed and Verified

1. ✅ **Yosys**
   - Command: `yosys -V`
   - ![Yosys](../images/yosys.png)

2. ✅ **Icarus Verilog**
   - Command: `iverilog -V`
   - ![Icarus Verilog](../images/iverilog.png)

3. ✅ **GTKWave**
   - Command: `gtkwave --version`
   - ![GTKWave](../images/gtkwave.png)

4. ✅ **ngspice**
   - Command: `ngspice -v`
   - ![ngspice](../images/ngspice.png)

5. ✅ **Magic**
   - Command: `magic`
   - ![Magic](../images/magic.png)

6. ✅ **Docker**
   - Command: `docker --version`
   - ![Docker](../images/docker.png)

7. ✅ **OpenLane**
   - Command: `make test` inside `~/OpenLane`
   - ![OpenLane](../images/openlane.png)

---

## 🔹 SkyWater PDK Verification (sky130A)

- Verified Magic integration with **Sky130A PDK**:  
  ```bash
  magic -T /usr/local/share/pdk/sky130A/libs.tech/magic/sky130A.tech
  load 5k_resistor
