# wmt_gd32_study
My GD32VF103 study

## Ref      
* https://github.com/riscv-mcu/GD32VF103_Firmware_Library  
* https://github.com/riscv-mcu/GD32VF103_Demo_Suites  

## Document  
* https://www.riscv-mcu.com/site/  
* https://www.rvmcu.com/quickstart-quickstart.html  

## IDE  
* Nuclei Studio IDE  
https://www.nucleisys.com/download.php  
https://www.riscv-mcu.com/site/Nuclei_Studio/  

## UART ISP firmware burning  
* https://dl.sipeed.com/LONGAN/Nano/Tools  
GD32_ISP_CLI_(Windows)1.0.0.5109.rar  
GigaDevice_MCU_ISP_Programmer_V3.0.2.5782_1.rar  
* command line  
GD32_ISP_CLI.exe -c --pn <PORT> --br 57600 --db 8 --pr EVEN --sb 1 --to 1000 -i GD32E230F8P6 -d --a 8000000 --fn D:\download.bin --v  
