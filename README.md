# wmt_gd32_study
My GD32VF103 study

## Ref      
* https://github.com/riscv-mcu/GD32VF103_Firmware_Library  
* https://github.com/riscv-mcu/GD32VF103_Demo_Suites  

## Examples  
* http://longan.sipeed.com/zh/examples/printf.html  
* http://longan.sipeed.com/zh/examples/badapple.html  
* https://github.com/sipeed/Longan_GD32VF_examples  

## Document  
* https://www.riscv-mcu.com/site/  
* https://www.rvmcu.com/quickstart-quickstart.html  
* http://longan.sipeed.com/zh/  

## IDE  
* Nuclei Studio IDE  
https://www.nucleisys.com/download.php  
https://www.riscv-mcu.com/site/Nuclei_Studio/  
* Arduino IDE  
https://github.com/sipeed/Longduino  

## UART ISP firmware burning  
* https://dl.sipeed.com/LONGAN/Nano/Tools  
GD32_ISP_CLI_(Windows)1.0.0.5109.rar  
GigaDevice_MCU_ISP_Programmer_V3.0.2.5782_1.rar  
* isp command line (for example, serial port 7)    
GD32_ISP_CLI.exe -c --pn 7 --br 57600 --db 8 --pr EVEN --sb 1 --to 1000 -i GD32E230F8P6 -d --a 8000000 --fn D:\download.bin --v  
see stm32flashloader  
https://www.st.com/content/st_com/en/products/development-tools/software-development-tools/stm32-software-development-tools/stm32-programmers/flasher-stm32.html  
* platformio firmware flash (download) command line (for example, serial port 7)      
https://github.com/sipeed/platform-gd32v/blob/master/builder/main.py  
stm32flash -g 0x08000000 -b 115200 -w D:\download.bin PORT7
