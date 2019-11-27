# MIPS project reflection (CID: 01497270)

Imperial Login : cw3918

Group Name : Yeet2

## Group working

In general, I played a supportive role in this group project. I was mainly involved in the process of debugging source code, building MIPS instructions files and testing functionality of specific instructions. We mainly worked separately on different sections but we always keep in touch on Messenger and updated the latest code on Github so both of us could access. Any critical bug discovered was instantly sent to our group chat to be discussed and solved collaboratively. Group meetings were held twice a week and we mainly focused on understanding and testing code we have finished and making future plans.

## Time management
In this project, we did manage our time in an organized way. Before internal submission on Nov 08, we have built a mips_simulator that is executable and generally functional. We then debugged the simulator by generating multiple mips_instructions binary files and kept fixing problems including error message identification, sign and unsigned numbers indication, instruction data type, memory allocation issue and linux system compatibility. On Nov 16 we built mips_testbench for more efficient testing and started to focus on corner cases to look for minor bugs. On Nov 20, we passed all tests and finished the project 2 days before deadline. 

## Software skills
In terms of generating mips_instruction bitstream, I initially intended to use a hex-editor and manually wrote bits as testbenches. However, By mapping instruction name with a corresponding opcode and other fields with a corresponding number, we found out by writing another C++ file, MIPS assembly code in each instruction set could be converted into a 32-bit binary file. This significantly increased the efficiency of testing our simulator and allowed us to test more corner cases. This idea inspires me to jump out of the specimen and discover other uses of programming language to support my project in the future.

## Tools and infrastructure
This project encouraged me to explore more functions embedded in Atom. By installing a package named “platformio-ide-terminal”, a built-in terminal which supports Linux command is provided, which allowed me to efficiently compile, test and run our project. A “Spell_check” Package has been used to prevent any typo and errors made while programming. In addition, “Neo hex-editor” was installed and used to visualize and edit testbenches from testbench generator C++ file. 

## Understanding of computer architecture
In this project, I have thoroughly read through MIPS Instruction Set and fully understand the impact of each instruction on the computer architecture system. All integers, values and memory declared in the class MIPS all have a corresponding part in the real MIPS CPU, and all instructions follow the datapath according to how a real CPU runs. I have tried to add more subfunctions like RegDst_MUX, MemtoReg_MUX, Opcode control unit to simulate in a more realistic way, but eventually removed them and manually assign values on different cases for more efficient running and better readability of the code. 
