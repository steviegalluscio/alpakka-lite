# Alpakka Lite
## Build Guide
1) Remove screws and take back cover off of controller.
2) Desolder the left and right rumble motors from the PCB and remove the motors by pulling straight out.
3) Remove the remaining screws from the PCB then fully disassemble the controller.
4) Drill out the hole from inside the front cover in the center of the thumb buttons. <table><tr><td><img src="./images/guide-1.png" alt="inside front cover" width="400"></td><td><img src="./images/guide-2.png" alt="drill hole" width="400"></td></tr></table>
5) File a notch on the same post down and to the left. <table><tr><td><img src="./images/guide-3.png" alt="file notch" width="400"></td></tr></table>
6) Strip a section end off of a wire and feed it through the hole from inside to out. <table><tr><td><img src="./images/guide-4.png" alt="wire in hole" width="400"></td></tr></table>
7) Screw in thumb screw. <table><tr><td><img src="./images/guide-5.png" alt="thumb screw wire" width="400"></td></tr></table>
8) Partially reassemble controller but leave the backplate off.
9) Desolder the USB cord. (Check for firmware updates one last time before this) <table><tr><td><img src="./images/guide-6.png" alt="usb pins" width="400"></td></tr></table>
10) Solder wires pointing downwards: 4x short 1"-2" wires to GND, GND, D+, D-, and 1x longer 3"-4" wire to 5V. <table><tr><td><img src="./images/guide-7.png" alt="usb pins" width="400"></td></tr></table>
11) Put muliple layers of electrical tape and/or automotive harness tape over the pins and screws. This will protect from shorts later. <table><tr><td><img src="./images/guide-8.png" alt="tape on pcb" width="400"></td></tr></table>
12) Press fit the left and right rumble mounts into the motor holders. <table><tr><td><img src="./images/guide-9.png" alt="rumble mount" width="400"></td></tr></table>
13) With a dab of hot glue, mount the left and right IMUs. Then solder ~7" wires to 3V3, GND, SCL, SDA, CS, and SAO. Then, run the wires up and underneath as shown. <table><tr><td><img src="./images/guide-10.png" alt="imu mount" width="400"></td><td><img src="./images/guide-11.png" alt="imu wiring" width="400"></td></tr></table> _Note: rubbing alcohol makes hot glue pop right off._
14) Solder the USB cord to the pico<table><tr><td><img src="./images/guide-12.png" alt="usb pins" width="400"></td></tr></table>
15) Hold BOOTSEL button, plug in USB cord, and flash firmware by drag and droping the .uf2 file from [releases](https://github.com/steviegalluscio/alpakka-lite/releases). After the intial flash you can use <a href="https://ctrl.inputlabs.io/" target="_blank">ctrl.inputlabs.io</a> to put the controller into BOOTSEL mode and flash updates.
16) Solder the pins according to [WIRING.md](./WIRING.md). Start with the controller PCB wires along the bottom of the pico first then use a blob of hot glue to hold the pico in place. Curved locking forceps or helping hands will make it easier especially where there are multiple wires sharing a pin. ![Alpakka Lite Wiring](./images/wiring-1.png)
17) Guide the wires as seen above and take your time when snapping on the back cover to make sure that no wires are pinched and that the paddle buttons are not blocked. Replace screws in back cover.
19) Enjoy gyro gaming and leave a star :star: on the repo.

<br/>
<br/>

## Troubleshooting
1) Check that your gamepad is in XInput/Xbox 360 mode. (For Tegenaria you have to do this once: hold HOME+X until green light)
2) When testing with a gamepad tester app, [switch to a profile](https://inputlabs.io/alpakka/manual/profiles) like "Console" the default is "FPS Fusion" and uses keyboard.
3) Check that the D+ and D- pins are not swapped and that you don't have any shorts or cold solder joints anywhere.
