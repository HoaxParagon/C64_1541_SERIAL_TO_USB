# C64_1541_SERIAL_TO_USB
Open source project to interface a Commodore 64 1541 5.25" floppy disk drive with serial to USB. This project is aimed at backing up C64 disks for historical benefit before the disks end up experiencing data decay and disappearing for good.

NOTE: this may take a while between school and work, don't expect magic by tomorrow



### Workflow plan
* Connect the interface to the PC (USB)
* Connect the drive to the interface (6 pin DIN)
* Scan the face of the disk into image file, alternativly, take a photo
* Name the photo and file to be taken in from disk
* Creates new 

### Hardware plans:
* For ease of access and development, the AVR platform will be used.
* Possibly include a reversible modification including an endstop to prevent platter crash.
* Possibly model and print an endstop mount to go inside the drive
* Custom board design, has female 6 pin DIN connector (eventually)
* First built on protoboard unless 6 pin DIN won't fit right in 0.1" spacing

### Software plans:
* A custom C64 serial to USB protocol will be made
* The process should be streamlined to enable ease of backing up.
* There will be a python script to control backing up the disks
* The python script should have GUI control
* The AVR that interacts with the drive should prevent damage to the drive (head crash)
* Script communicates with serial comm port attached to interface device









