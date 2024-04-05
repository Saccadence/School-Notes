# Algorithm
A sequence of steps to accomplish a task
- The basic concept of programming
## Procedural Programming
A focus on *actions*, also called procedures or functions
- Requires a specific set of instructions in a specific order to complete a task
	- More difficult to write and get correct due to the limiting nature of this style
## Object Oriented Programming (OOP)
A focus on *modeling* things: both their characteristics and actions
### Objects
A "thing" with a set of descriptors attached that allows the object to be more dynamically manipulated
- Descriptors are attributes/characteristics/properties and actions
#### Class(ificiation)
The complete object with its descriptors attached
- Made up of variables and/or functions
##### Variables
Hold data about characteristics/attributes/properties of a thing
##### Functions
Hold data about what the things can perform (methods/behaviors)
# Programming Languages
Classes are just concepts
- They are made up of multiple different factors that are categorized into one term
- They are also apart of, and made of, hierarchies
A language used to write a sequence of instructions for a computer
- Allows for the use of symbols regardless of the hardware it is present on
- The higher level a language is, the more directly related it is to 1's and 0's
## Inheritance Hierarchy
The higher the level of a command in a hierarchy, the more commands it procures underneath it
- This also translate to writing more/less code, depending on the level your command(s) is at
### Microcode
The code that a CPU can execute is called the Instruction Set Architecture (ISA)
- Microcode resides on ROM and is unpublished and proprietary (i.e. not used by an end-user)
	- Also called firmware
#### Complex Instruction Set Computer (CISC)
Only essential basic actions are hardwires
- The CPU relies on microcode to combine basic actions to handle other needed hardwired actions
- Easier to design
#### Reduced Instruction Set Computer (RISC)
All actions are hardwired
- More difficult to design
### Machine
If the hardware is built based on RISC, then Machine code is the lowest level of programming
- Otherwise, for CISC systems, the code may be turned into Microcode
### Assembly
Uses words to program where each word represents a string of 1's and 0's
#### Source File (Source Code)
The original typed out program in the respective language
- This file, and the code stored on it, will then be translated to Machine (1's and 0's)
	- Done through the use of a Key (compiler), also called Compiling or Interpreting
	- Result is a Binary File or Executable File
## High Level Languages
Tend to conform to a syntax (grammar) made of key commands with a properly applied order
- In their basic format, they work to make a a large set of basic commands (lower level) accessible in one or more key commands
# Flow Charts
A general analogy for high level programming (OOP)
- The ability to visualize what a code is doing through a flow charts not only shows what the code is doing, but how to properly navigate the code's instructions to add to, remove from, or edit a source code
# Software Development Life Cycle (SDLC)
A collection of "best" practices to ensure consistent and valid progress
- Not verifying changes to code and ensuring that the change will be well implemented in future development leads to regression as you have to spend more time trying to fixing issues than writing new code
- Some of these practices include:
	- Documentation
	- Review
	- Signing-Off on the Change(s)
The goal is to catch mistakes or future problems sooner, rather than later
### Traditional SDLC
Spending more time on each (self-determined) step to ensure minimal errors, at the cost
### Rapid Application Development (RAD)
Faster development timeline, but more error prone
- Can increase development time due to fixing bugs the entire time, or can outright kill a project if there are too many fundamental flaws
# Programming and Integrated Development Environments (IDEs)
IDEs are programs that make the resources necessary (or convenient) for developing programs
- Originally was done via Command Line (CLI) and Text Editors