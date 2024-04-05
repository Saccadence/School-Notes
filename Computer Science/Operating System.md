# Operating System Overview
CPU needs instructions in RAM (from Data Drive) to start up
## Basic Input Output System (BIOS)
Solid state memory chip on the motherboard
- Stores all the basic instructions needed
	- Power Supply self-test
	- CPU loads BIOS into RAM
	- Power On Self Test (POST)
		- Check CPU
		- Check BIOS
		- Video Card Test
			- Run Video Card BIOS
			- Test and initialize Video Card
		- Memory Test
		- BIOS Start-up Screen
			- POST or Beeps will present themselves if anything goes wrong before this point
	- Locate Disk with OS
		- BIOS reads CMOS memory
			- Small memory chip that stores initialization data (maintained by battery on motherboard)
		- Locates sequence to check drives for OS
		- Examine Disk for Master Boot Record (MBR)
			- Load MBR into RAM
				- Contains a Partition Table (a description of the layout of the disk) and instructions of how to load the OS into RAM
				- BIOS transfers control to Partition Loader
					- Detects other hardware and notes configuration
	- Loads OS File System Drivers
		- Used to load KERNEL OS files
			- Interface between applications and hardware
	- Load OS into Ram and start OS subprograms
		- OS Object Manager
		- OS Executive
		- Security Manager
		- OS Memory Manager
		- OS Cache Manager
		- I/O Manager
		- OS Process Manager
	- Load OS System Device Drivers
	- Launches the Session Manager (SMSS)
		- Start up the Graphical User Interface (GUI)
		- User Login
	- Successful Startup
- Called EFI on Mac computers
## Operating System
Primarily Known and Consumer Used OSes:
- Mac
- Windows
- Linux
- Android
- iOS
### User Interface Manager
#### Character User Interface (CUI)/Command Line Interface (CLI) - Old
The user interface was made up of commands that a user would have to type in order to access and navigate the OS
- Still used today for interfacing with parts of the OS, or other code (like applications), that do not have a GUI associated with it.
#### Graphical User Interface (GUI) - New
Replaced the CLI by making the process less difficult for the end-user. Commands became clickable icons that would allow you to access parts of the OS that would've required one or more commands in a CLI to access, without the the need of memorization.
### Process Manager
Manages currently active programs running on the CPU
- Typically automatically managed by aforementioned system
	- Manages things like times to load processes, the affinity you assign processes, and more
### File Management
A system to keep track of and manage files/folders associated with the OS
- You can save, rename, create, and move files
- Files are stored in a hierarchy
### Device Managers
System that uses Device Drivers to interface between the OS and hardware
- Minimizes the need to write code dedicated to achieving a similar task for all applications
	- Makes programs more universalizable due to not having to account for every individual piece of hardware an end user might have
### Security/Login Manager
Password protection for the OS along with saving activity logs, scanning files/folders for malware, and backup/recovery through save states