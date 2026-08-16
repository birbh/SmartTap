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
    Its the back part where the brain of my pcb is located. On the left side of my pcb there is a coil made with wire which helps to capture the nfc field of phone and convert it into electrical energy which is connected to NT3H1101W0FTTJ nfc chip module which then helps to light up the led in the front. Also there's a cool floral design along with an art of lord Krishna which has made my pcb mor attractive. And there are some details abt me and a qr code linking to linktree as I have stated above.
    And I have planned to cover the copper coil with Lead-free HASL which would make my pcb look more attractive and cool. 
    
## Instruction to make this project:

