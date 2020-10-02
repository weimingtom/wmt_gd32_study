# wmt_gd32_study
My GD32VF103 study

## template project  
* search Running_Led_v1_isp.rar  

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
* **NOTICE**  
ISP for GD32VF103C-START:  
switch JP4 to High,   
after running stm32flash (after burning or after isp), auto into running mode, press reset button to return to burn mode (no need to change JP4)  
* https://dl.sipeed.com/LONGAN/Nano/Tools  
GD32_ISP_CLI_(Windows)1.0.0.5109.rar  
GigaDevice_MCU_ISP_Programmer_V3.0.2.5782_1.rar  
* isp command line (for example, serial port 24), burn and run      
.\gd32_isp_cli\GD32_ISP_CLI.exe -c --pn 24 --br 57600 --db 8 --pr EVEN --sb 1 --to 1000 -i GD32VF103CBT6 -d --a 8000000 --fn ..\Debug\Running_Led.hex --v  
.\gd32_isp_cli\GD32_ISP_CLI.exe -c --pn 24 --br 57600 --db 8 --pr EVEN --sb 1 --to 1000 -i GD32VF103CBT6 -r --a 8000000  
https://www.st.com/content/st_com/en/products/development-tools/software-development-tools/stm32-software-development-tools/stm32-programmers/flasher-stm32.html  
* platformio firmware flash (download) command line (for example, serial port 24)      
https://github.com/sipeed/platform-gd32v/blob/master/builder/main.py  
.\tool-gd32vflash\stm32flash.exe -g 0x08000000 -b 115200 -w ..\Debug\Running_Led.hex COM24  
