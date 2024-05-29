# Writing a C code to count the sum of numbers from 1 to n and running this program using RISC-V simulator
## Writing a C code to count sum of numbers from 1 to n.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/a248fc9e-6d0d-43cd-b4f6-710a7d961386)

I . First, I opened the terminal and wrote code to create and open a new C file in Leaf pad, as demonstrated below:

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/ee490d05-c8a0-4a2a-8364-fc5b1dcb7189)

II . Next, I wrote my code in Leaf pad as illustrated below :

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/112c0988-4d15-4f00-b0cc-889d9eed950a)

III. Then I compiled and ran it in the terminal to verify, and achieved the desired output.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/ce5f6a61-33c8-401a-b8bf-4a5c64735492)

IV. Then  I tested different values of n, such as n=100, and obtained the results.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/7b3e05e2-f581-4de0-8698-54eb5b0208b2)
![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/73b69829-a7da-41f4-8c9e-1b8f62e42550)

# Running the above program in RISC-V Simulator
After running the code in the terminal, I need to execute it in the RISC-V simulator. For this, a specific set of code is required, which I have implemented in the following steps.:

1)	First, I wrote a code to compile it with the RISC-V GCC compiler using option 1, which generates a file with a .o extension.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/dcd11e0a-b497-4ad7-b9a1-21ac5944d358)

2)	With the command `riscv-unknown-elf-objdump -d sum1ton.o` to obtain the assembly code for the above C program. This generated numerous assembly instructions, which I filtered by appending `| less` to the command. To locate the main section, I searched for "main." The byte address for main was found to be 10184, and there were 15 instructions when using option 1. It was observed that the address of each consecutive instruction increments by 4.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/d5901f40-cbed-40e0-b575-8ac6519f5053)

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/2042bfed-d1b1-411a-b650-7745b87951dd)

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/277bc9b8-a3b8-43cc-895b-58d0c871d526)

3)	Next, I ran the same commands but used the `-Ofast` option instead of `-O1`. This time, I got fewer instructions, specifically 12. This demonstrates that the assembly instructions in the file change based on the different compilation options used.

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/0198f1a1-ae98-4b42-971b-69525d4d9cec)

![image](https://github.com/SuriyaNatarajan02/VSD_Mini_Research-Internship/assets/110706394/4034cecf-37d5-4514-b814-c724bf6b513d)

And that’s all !!!
