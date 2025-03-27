# LGUltraGear34GP950
This is an early solution to the lack of drivers and ICC profiles for the 34GP950G
# ✅ LG UltraGear Monitor Driver Fix for Windows 11
**Bypass "Generic PnP Monitor" and unlock HDR, 10-bit color, and proper ICC profiles**

---

## 📌 Problem

Windows 11 may incorrectly identify high-end LG UltraGear monitors (e.g., **LG 34GP950G-B**) as a **Generic PnP Monitor**, leading to:

- 🛑 No HDR toggle in settings
- 🎨 Washed-out colors and poor contrast
- ⚠️ ICC color profiles not available or misapplied
- ❌ Incorrect refresh rate and color bit-depth detection

Even on LG’s official support page, the correct driver and ICC profile for many UltraGear models are *missing*.

---

## 💡 Solution

We fix this by **using a similar UltraGear monitor's driver and ICC profile**, forcing Windows to recognize your monitor properly.

---

## 📂 Files Included

- `ULTRAGEAR_32GQ850B.inf` — Monitor driver from the LG **32GQ850-B**
- `ULTRAGEAR_ICC_Profile.icc` — ICC profile sourced from [RTINGS.com](https://www.rtings.com/monitor)

These files work well for other HDR UltraGear displays like the **LG 34GP950G-B**.

---

## 🛠 Installation Steps (Manual "Have Disk" Method)

1. **Unzip this repo** to a folder (e.g., `UltraGearFix/`)

2. Open **Device Manager**  
   → Expand `Monitors`  
   → Right-click `Generic PnP Monitor` → `Update driver`

3. Choose:  
   `Browse my computer for drivers` →  
   `Let me pick from a list of available drivers on my computer` →  
   Click **Have Disk...**

4. Browse to the `.inf` file you downloaded from this repo (e.g., `ULTRAGEAR_32GQ850B.inf`)  
   → Click **OK** and continue through the prompts

5. Reboot your PC

---

## 🖼 Enable HDR & Set ICC Profile

### Enable HDR in Windows: !This doesnt work all the time yet! I'll take help!
- Go to **Settings → System → Display**
- Scroll down to **HDR**, toggle it **ON**
- Use **Windows HD Color Settings** to fine-tune

### Apply the ICC Profile:
1. Open **Control Panel → Color Management**
2. Under **Devices**, select your monitor (now correctly named)
3. Check "Use my settings for this device"
4. Click **Add…** and select `ULTRAGEAR_ICC_Profile.icc`
5. Click **Set as Default Profile**

---

## ✅ Results

- ✅ HDR working in Windows 11 !Sometimes!
- ✅ Monitor correctly identified as an UltraGear display
- ✅ Color profile auto-applied or assignable
- ✅ 10-bit color, correct refresh rate (up to 180Hz), and better contrast

---

## 🙋‍♂️ Notes

- This is a workaround for missing official support
- Works well for **Nano IPS**, **HDR600**, and **QHD UltraGear** panels
- Tested on **Windows 11 Pro + AMD Radeon RX 7900 XTX**
- Do this at your own risk — but it's safe and reversible

---

## 🌐 Credits & Sources

- Driver: Official LG support page for [LG 32GQ850-B](https://www.lg.com/us/support/product/lg-32GQ850-B.AUS)
- ICC Profile: [RTINGS.com LG Monitor Reviews](https://www.rtings.com/monitor)
- Original idea & discussion: [Reddit /r/ultrawidemasterrace thread](https://www.reddit.com/r/ultrawidemasterrace/comments/qj5wdf/lg_34gp950gb_driver/)

---

## 🧠 Pro Tip

After setup, create a System Restore Point!  
Just search **"Create a Restore Point"** in the Start menu.

---
