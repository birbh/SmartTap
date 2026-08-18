# SmartTap

SmartTap is a sleek, credit card thin(.8mm) personal card powered entirely by NFC and its energy harvesting tech. i.e no battery required!!!

## Overview:
SmartTap is a custom engineered PCB business card which is designed to make a great first impression among colleagues. It's equipped with an "NXP NT3H1101" energy harvesting NFC chip with an integrated PCB trace antenna coil and active indicator leds, the card wirelessly harvests power directly from any smartphone or NFC reader to illuminate upon tapping.

### What makes it unique?

- Zero external power: Operates completely wirelessly and without a battery!! It's done by harvesting 13.56 MHz RF energy from a phone's NFC field. 

- Credit card form factor: It's engineered at custom 0.8 mm thicknes, perfectly matching the ISO 7810 ID-1 standard for standard credit cards. 

- Aesthetic Silver Trace: Designed with exposed custom coil loops finished in smooth Lead-free HASL for high quality durability and sleek look against a matte black soldermask. 

- Instant Contact Sharing: Embedded NTAG I2C functionality which prompts to open digital portfolio links on modern nfc supported devices. If any device has no nfc compatibility, then I have attached a qr code to linktr.ee as to let everyone access my portfolio and know abt me. 

### Why I made it?

The standard paper business cards are very easy to lose, forget or throw away. So I awnted to design a physical hardware project that combines embedded engineering, PCB antenna design and a personal branding to an unforgettable hands-on experience. 

Also who wants a boring paper businesss card nowdays in the era or modern tech. So I developed this idea to leave our techy impression whenever we meet a person or go somewhere. Actually it helps us to farm some aura in front of our fellow friends😝.......jk. 

Creating this card solved two main challenges for me:
1. Learning hoow to design RF trace coils and passive energy harvesting power stages without needing bulky batteries. 
2. Creating a clean, modern networking tool that lets me share my work, social links, and contact info instantly with simple smartphone tap. 

### How to use it?

1. Take a mobilephone that supports NFC. 
2. Tap the card: 
    Bring your phone's NFC reader area(usually on top rear of iphones, center/top of android phones) close to the nfc coil area of the business card. 
3. Watch it light up: 
    The harvesting circuit draws power wirelessly from the phone's field and instantly lights up the onboard leds. 
4. Open Portfolio: 
    A notification will pop up instantly on your phone screen. Tap it to view my cintct details and online portfolio!!!
5. For those who dont have a nfc supported mobilephone, there is a qr code in the pcb's silkscreen which opens the same link as the nfc chip does. 

### Visuals in pcb:

1. Front:
    In the front part I have added my personal data like github,insta and linkedin along with my name. I have also added cool floral design in the silkscreen too which has leds embedded in its different vacant spaces. This has made my design more cool to look for a stranger.        

2. Back:
    Its the back part where the brain of my pcb is located. On the left side of my pcb there is a coil made with wire which helps to capture the nfc field of phone and convert it into electrical energy which is connected to NT3H1101W0FTTJ nfc chip module which then helps to light up the led in the front. Also there's a cool floral design along with an art of lord Krishna which has made my pcb more attractive. And there are some details abt me and a qr code linking to linktree as I have stated above.
    And I have planned to cover the copper coil with Lead-free HASL which would make my pcb look more attractive and cool. 
    
## Instruction to make this project:

Setting up and assembling the card is straightfoward:

### 1. PCB manufacturing specs:
When submitting the greber files to your pcb manufacturer, ensure the following settings are specifies:
- Board Thickness: 0.8 mm (which is crucial for credit card flexibility and thickness)
- Solder mask color: Matte black or black
- Silkscreen color: White
- Surface finish: Lead-Free HASL
- Copper weight: 1oz

### 2. SMT component soldering:
1. Clean the PCB pads with isopropyl alcohol(if available) before soldering. 
2. NFC IC(U1- NT3H1101): Align pins using the indicator in silkscreen. Apply flux and reflow using hot air station or a fine tip soldering iron. 
3. Passive Components: Solder the 100nf decoupling capacitor across VOUT and VSS, followed by the 33 ohm curreny limiting resistors. 
4. LED orientation: Check the polarity on the back of the 0603 SMD leds(red led preferred) before soldering to ensure correct polarity. 
5. Also make sure that you don't erase or damage the silkscreen data as there's a qr code in it and erasing it may corrupt the data. 

### 3. Programming the NT3H1101W0FTTJ data:
No external programmer or hardware flasher is required!!!
1. Download NFC Tools(available for free on [ios](https://apps.apple.com/np/app/ntag-i2c-demoboard/id1495775864
NTAG I2C Demoboard) and [android](https://play.google.com/store/apps/details?id=com.nxp.nfc.tagwriter)).
2. Open the app, select "Write", and add your record (eg. URL Link,vCard or social media handle). 
3. Tap "Write" and hold the PCB card near your phone to save your digital information directly ti onboard chip. 

## Photos:
### CAD:
1. PCB:
<img width="818" height="475" alt="Screenshot 2026-08-18 at 2 29 23 PM" src="https://github.com/user-attachments/assets/be3b168e-2040-4b1f-8253-a7a108b9bb57" />
<img width="813" height="509" alt="Screenshot 2026-08-18 at 2 30 11 PM" src="https://github.com/user-attachments/assets/a48cea20-6f1d-498e-a88f-b23acf121ca4" />

2. LED:
<img width="526" height="509" alt="Screenshot 2026-08-18 at 2 33 27 PM" src="https://github.com/user-attachments/assets/e59ea91b-98b7-41f5-a5f3-2b23a0cbea85" />

3. Capacitor:
<img width="542" height="495" alt="Screenshot 2026-08-18 at 2 34 09 PM" src="https://github.com/user-attachments/assets/60486c66-14aa-40e4-a0e4-0ca35f0fc5f5" />

4. NT3H1101W0FTTJ nfc chip:
<img width="666" height="466" alt="Screenshot 2026-08-18 at 2 35 03 PM" src="https://github.com/user-attachments/assets/5e6ba8ce-65ac-4bdc-9881-50b10fb2808c" />

5. Resistor:
<img width="596" height="474" alt="Screenshot 2026-08-18 at 2 35 22 PM" src="https://github.com/user-attachments/assets/16f3d2fc-9dbe-48a3-b027-f56871e16c20" />




### Schematic:
<img width="933" height="442" alt="Screenshot 2026-08-18 at 2 28 03 PM" src="https://github.com/user-attachments/assets/f6b38256-db87-4f59-9021-5a14385ec6d4" />


### PCB:
<img width="806" height="728" alt="Screenshot 2026-08-18 at 2 36 14 PM" src="https://github.com/user-attachments/assets/6a8095ef-1995-44a3-b205-468ab20920df" />
<img width="618" height="464" alt="Screenshot 2026-08-18 at 2 36 52 PM" src="https://github.com/user-attachments/assets/691bcd71-7ee2-4034-ab7d-63ffd28cb546" />


## BOM(initial):

1. 100nf Capacitor_SMD:C_0603_1608Metric
2. LED_SMD:LED_0603_1608Metric
3. 33 ohm Resistor_SMD:R_0603_1608Metric
4. NT3H1101W0FTTJ:TSSOP8_SOT505-1_NXP(nfc chip)
5. Printed pcb ready for soldering
