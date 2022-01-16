# C64_1541_SERIAL_TO_USB
Open source project to interface a Commodore 64 1541 5.25" floppy disk drive with serial to USB. This project is aimed at backing up C64 disks for historical benefit before the disks end up experiencing data decay and disappearing for good.

NOTE: this may take a while between school and work, don't expect magic by tomorrow. I also have to check and fix the operation of at least one of the 1541s I recently got.  
NOTE2: I'm hoping to get started on this in the next coming months. Life has been crazy for us all but soon mine will settle down a bit. I'm looking forward to having a repo of ripped C64 disks.  

Interface version: 0.000  
Script version: 0.000  
(no code made yet, planning phase)  


### Workflow plan:
- [ ] Connect the interface to the PC (USB) (atmega
- [ ] Connect the drive to the interface (6 pin DIN)
- [ ] Scan the face of the disk into image file, alternativly, take a photo
- [ ] Name the photo and file to be taken in from disk
- [ ] Creates new folder with name of disk, contains scan/photo of disk and disk image

### Hardware plans:
- [ ] For ease of access and development, the AVR platform will be used, platformIO or atmel studio 7?
- [ ] Possibly include a reversible modification including an endstop to prevent platter crash, have to check version of drives.
- [ ] Otherwise, perhaps a mic to detect specific sound of head crash (more complicated?, might, over time, damage the drive)
- [ ] Possibly model and print an endstop mount to go inside the drive, DIO pin, easy enough to implement, will have extra pins, why not?
- [ ] Custom board design, has female 6 pin DIN connector (eventually), find out exact connector type used.
- [ ] First built on protoboard unless 6 pin DIN won't fit right in 0.1" spacing
- [ ] ~~~Likely going to use an Arduino Nano dev board, they're cheap and easy to embed as a daughter~~~, arduino NANO boards don't have USB, will use 16U4 instead, build in D+/D-


### Software plans:
- [ ] ~~~A custom C64 serial to USB protocol will be made~~~, not made, implementation of C64 flavor of serial protocol, more research required.
- [ ] The process should be streamlined to enable ease of backing up.
- [ ] There will be a python script to control backing up the disks, maybe HTML frontend?
- [ ] The python script should have GUI control, KIVY
- [ ] The AVR that interacts with the drive should prevent damage to the drive (head crash)
- [ ] Script communicates with serial comm port attached to interface device
- [ ] python script should interact with printer to scan disk, or at least scanned pic file and
   read the text on the disk to fill out the info, semi automated process, disk scanned then info dumped, packed together in a zip  
- [ ] ~~~use tkinter to make GUI~~~, probably KIVY instead, easier to port around  


### Reference documentation:
Serial port info
https://www.c64-wiki.com/wiki/Serial_Port








