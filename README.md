# wmt_gd32_study
My GD32VF103 and GD32F450 study  

## GD32VF103, GD32VF103C-START    
* https://github.com/weimingtom/wmt_gd32_study/blob/master/GD32VF103_001.md   

## GD32F450VK, GD32450V-START  
* https://github.com/weimingtom/wmt_gd32_study/blob/master/GD32F450VK_001.md   

## 梁山派, GD32F470ZGT6    
* https://lckfb.com/project/detail/lckfb_lspi?param=baseInfo  
* liangshan-pi-nes-game-console-master.zip  
* liangshanpi-air-game-master.zip  
* http://club.szlcsc.com/forum/179_0_1.html  

## GD32F470V-START, GD32F470VKT6    
* GD32F4xx_Demo_Suites_V2.6.2_v1.7z  
* GigaDevice.GD32F4xx_DFP.3.0.4.pack  
* https://www.gd32mcu.com/cn/download/8?kw=GD32F4  

## 梁山派屏幕扩展板, LVGL  
* https://lckfb.com/docs/lspi_rgb_mcu_lcd_ex/#/屏幕扩展板资料下载  
* https://lckfb.com/project/detail/lspi_rgb_mcu_lcd_ex  
* 梁山派屏幕代码.zip  
* 梁山派LVGL移植RGB-480x800_v0.7z  
* https://blog.csdn.net/qq_51930953/article/details/129313750  

## GD32H759I-START  
```
入手了GD32H759I-START开发板，只能说这块板实在是绞尽脑汁都没办法烧录，
最后是通过外接J-Link用MDK5烧录才行——不能用jflash，
因为jflash和MDK5的jflash都无法识别到GD32H759，这个mcu太新了，
只能修改成Cortex-M7就能烧录，代价是不能读全片（可能通过命令行可以）。
为何要这么麻烦呢，因为这块板各种不方便：
（1）板载的daplink似乎不能用，只能供电
（2）串口也无法ISP烧录
（3）默认BOOT跳帽接L上方，在这种环境下就可以jlink了
（4）jlink必须和gd-link同时接（双重供电），jlink的swd引脚需要自己焊接
（5）板载的某些针脚不是2.54间距，不太适合研究GPIO，这点比不上
GD32F470V-START和梁山派那么好用
```
