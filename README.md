# TRS-80 Model 1 Mini Monitor

A 3D-printable, 65%-scale enclosure that restyles a modern 8" Eyoyo LCD into a faithful mini version of the original TRS-80 Model I monitor, complete with front “fake” knobs, a front power LED, hidden IR window option, and mounting points for the stock speakers and main PCB. Everything is designed to reuse the donor monitor’s electronics wherever possible. Released under the MIT-license.

|![Front Case](/Images/Monitor_Front.png) | ![Back Case](/Images/Monitor_Back.png) |
|-------------------------------------|-------------------------------------|

## Project Details

### Latest Files

Find the most up-to-date printable parts in the **`/Latest`** folder:

- **Case**
  - [`M_Front.stl`](/Latest/M_Front.stl) — front shell  
  - [`M_Back.stl`](/Latest/M_Back.stl) — back shell
- **Hardware**
  - [`Knob.stl`](/Latest/Knob.stl) — decorative front-panel knobs (print **2x** total)  
  - [`Tab.stl`](/Latest/Tab.stl) — universal retaining tab used for screen, speakers & buttons (print **6×** total)
- **Finishing Aid (Optional)**
  - [`Spray_Cover_Optional.stl`](/Latest/Spray_Cover_Optional.stl) — paint mask that snaps in to protect the black center while spraying the silver surrounding


### Donor Display

This project is designed around a readily available 8" Eyoyo monitor (example: [Eyoyo 8" 1024×768 Model EM08F](https://www.amazon.com/dp/B0BG77R6ST)).  
Transplant the LCD panel, main PCB, button/IR board, and stereo speakers into the Mini Monitor enclosure.

### Implementation

- Designed for FDM printing
- Hidden, top-rear button access preserves the vintage look while still giving you power/menu/source/volume control.
- A front 5mm LED replaces the original mechanical power button.
- Optional IR receiver tunnel on the bottom allows remote use without spoiling the front aesthetic.

All mechanical parts are provided as STL files suitable for FDM printing. The design uses snap-fit and tabs to secure the LCD and speakers. The back shell provides mounting points for the main PCB and a control area so modern function buttons remain accessible yet hidden. Make sure to use the plastic buttons provided in the original case and don't throw them out with the donor case.

### Assembly Guide

For the following steps, keep the donor LCD’s foil cable safe from kinks and excessive strain.

1. **Print Parts**
   - Required: `M_Front.stl`, `M_Back.stl`, `Tab.stl (×4)`, `Knob.stl (×2)`  
   - Optional: `Spray_Cover_Optional.stl` to simplify paint spraying
2. **Paint**
   - Apply a black primer spray that also functions as the base color.
   - The original monitor was fully black ont he back shell. The original aesthetic for the front shell is **silver body** with a **black center**. Use `Spray_Cover_Optional.stl` as a paint mask that locks into the bezel to shield the black area while spraying the silver surrounding. 
     ![Spray cover applied](/Images/Spray_Cover_Applied.png)
   - After enough time drying, apply a layer of top-coat to protect the paint. I used a gloss top-coat, but made this thin to avoid excessive shine.
   - You might want to paint the two knobs at this point as well.
3. **LCD Panel Install**
   - Slide the panel **top-first** into the front shell’s upper lip/gap until it seats.  
   - Secure the **bottom** with **two tabs** (`Tab.stl`) using small screws or hot glue as preferred.  
   - Keep the foil cable relaxed—route toward the main PCB mount on the back shell.  
     ![Mount detail](/Images/Monitor_Mount.png)
4. **Main PCB Mount**
   - The board is installed upside-down.
     ![PCB mount](/Images/PCB_Mount.png)
   - Fix the board in place using a 3mm screw with 12mm length. Use the first holes on the interface side. When inserting the screw, fix it with a nut on the other side. Add an additional nut on top of it, leaving about a 1-2mm gap. This gap is provided as the pins peaking through the PCB sometimes are longer and this will give enough clearance. Insert the screw into the case mount point and add another nut on top to fix it in place. Overall, you need 2 screws with a total of 6 nuts, three for each side.
5. **Front Power LED**
   - On the button PCB, there are two LEDs, one displaying power while the other shows button presses. We want to replace the power LED.
   - When you have the board in front of you, the buttons should be on the left, while the two LEDs are on the right. The far-most right LED is the power LED.
   - Desolder the SMD LED from the donor button PCB, attach leads, and wire a **5 mm red LED** to the front LED hole. The upper pad is GND and should be attached to the cathode (shorter lead).
   - Use an LED holder/grommet or hot glue to secure it. You are reusing the donor’s LED pads/drive so no extra resistor is needed.  
     ![LED](/Images/LED.png)
6. **Speakers**
   - Transplant the two donor speakers. They are glued into place in the donor monitor and will require some effort to get them out.
   - When transferred, you probably need to add longer wires to them.
   - During mounting, each uses **one tab** to keep them in place. You can also hot-glue the speakers in, if you prefer that.
     ![Speaker mounts](/Images/Speaker_Mount.png)
7. **Optional IR Receiver**
   - A hidden **IR window** underneath the display provides remote control support without spoiling the look. Desolder the donor IR receiver from the button board, extend with **3 wires** (keep polarity), and hot-glue it into the **bottom IR pocket** (light-trap geometry keeps it unobtrusive).  
     ![IR mount](/Images/IR_Mount.png)
8. **Buttons (Top-Back Relocation)**
     ![Buttons](/Images/Buttons.png)
   - Insert the plastic buttons first with the flat side to the back.
   - Insert the PCB on top of the buttons. Make sure to orient the board the right way so the plastic buttons from the outside press the momentary switches.
   - Fix in place with two tabs or hot-glue the board in place.
9. **Close the Case**
   - Use plastic screws to connect the front and back of the cases. You need 4 of these screws.
   - Add the **two decorative knobs** (`Knob.stl`) to the lower right front. Use super glue to glue them in place.


### Recommended Print Settings

Material: PLA or PETG (PETG for higher heat tolerance)
Supports:
- M_Front.stl: Flat on back and add supports
- M_Back.stl: Flat on the front and add supports
- Tab.stl, Knob.stl: Off
- Spray_Cover_Optional.stl: Flat and add supports. Feel free to leave them on after printing as they don't matter during spraying.

## Main TRS-80 Model 1 Repository

For additional resources related to the TRS-80 Model 1, be sure to check out the [central page for the TRS-80 Model 1](https://www.github.com/RetroStack/TRS-80-Model-I) on [RetroStack](https://www.github.com/RetroStack).

## Support this Project

RetroStack is passionate about exploring and preserving the legacy of older computer systems. My work involves creating detailed documentation and videos to share the knowledge. I am also dedicated to reviving these classic systems by reimplementing them and offering replacement parts at no cost. If you're keen on supporting this unique project, I invite you to visit my [Patreon page](https://www.patreon.com/RetroStack). Your support would be immensely valuable and greatly appreciated!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
