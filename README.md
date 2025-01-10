# USB-C RTL-SDR mod

<img src="/images/img_1.jpg?raw=true" alt="USB-C RTL-SDR v3" width=400 /> <img src="/images/img_2.jpg?raw=true" alt="USB-C RTL-SDR v3" width=400 />

## Kicad files
If you want to open and modify the original project in Kicad 8 (>=8.0.7), you can find both the `.kicad_sch` and `.kicad_pcb` files in the `kicad` folder in this repository. I recommend you use the latest Kicad 8 version available for better compatibility.

## Gerber files
If you want to fabricate your own PCBs from a PCB manufacturer of your choice, you can go ahead and download the `Gerber-v1.x.zip` file from the `gerber` folder in this repository. Upload it or send it to the PCB fabrication house and select the following specifications (if not already filled out):
- **Layers**: 2
- **PCB Thickness**: 1.2 mm
- **PCB Color**: any (green is usually cheaper and faster to produce, but black also looks nice and might blend with the black outer case)
- **Surface finish**: HASL or ENIG (gold plating)
- **Outer Copper Weight**: 1 oz
- **Via Covering**: Tented
- **Mark on PCB**: Remove Mark (JLCPCB specific, now free of charge)
- **Castellated holes**: Yes

## BOM and assembly

Included in this repository is the HTML BOM (`ibom.html`) to help you in the assembly/soldering process after you received your PCBs. You can [access the Interactive HTML BOM here](https://umbertoragone.github.io/usbc-rtl-sdr/bom/ibom.html), without having to download the .html file. Also, here is the list of components you will have to source and solder yourself:

| Reference(s) | Value                   | Footprint         | LCSC Part #                                                   | Qty |
| ------------ | ----------------------- | ----------------- | ------------------------------------------------------------- | --- |
| R1, R2       | 5k1 1%                  | R_0402_1005Metric | [C25905](https://www.lcsc.com/product-detail/C25905.html)     | 2   |
| USB1         | USB_C_Receptacle_USB2.0 | TYPE-C-31-M-12    | [C2988369](https://www.lcsc.com/product-detail/C2988369.html) | 1   |
