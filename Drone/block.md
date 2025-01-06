
Novel image
![[Drone_Novel.jpg]]
EO1, EO2 is RGB sensor  IMX586 8000 x 6000pixels 解析度，可拍攝4800 萬畫素照片
4800萬 4800,0000  48M
LWIR thermal IR 
EO1 or 2 using 48M or binning (12M)

Sensor Fusion
https://weilihmen.medium.com/sensor-fusion-%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%B4%B9-amazon-go-and-autonomous-vehicle-3284f23f04b8
Tom image
EO1 (TELE), EO2 (WIDE), (fixed lens)  , in digital zooming 交界, EO1 EO2 need on at same time
![[Pasted image 20250103160439.png]]

use Qualxomm too heavy, board is < 10g
Tom image
![[Pasted image 20250103162528.png]]

https://zh.wikipedia.org/zh-tw/USB%E8%A6%96%E9%A0%BB%E9%A1%9E%E5%88%A5
**USB video class**（又稱為**USB video device class** or **UVC**）就是[USB](https://zh.wikipedia.org/wiki/%E9%80%9A%E7%94%A8%E4%B8%B2%E8%A1%8C%E7%B8%BD%E7%B7%9A "通用序列匯流排") device class影像產品在不需要安裝任何的驅動程式下隨插即用，包括[網路攝影機](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E6%94%9D%E5%BD%B1%E6%A9%9F "網路攝影機")、數位[攝影機](https://zh.wikipedia.org/wiki/%E6%94%9D%E5%BD%B1%E6%A9%9F "攝影機")、類比影像轉換器、[電視卡](https://zh.wikipedia.org/w/index.php?title=%E9%9B%BB%E8%A6%96%E5%8D%A1&action=edit&redlink=1)及[靜態影像相機](https://zh.wikipedia.org/wiki/%E9%9D%9C%E6%85%8B%E5%BD%B1%E5%83%8F%E7%9B%B8%E6%A9%9F "靜態影像相機")。
UVC v1.1 支援壓縮影片流，包括[MPEG-2 TS](https://zh.wikipedia.org/w/index.php?title=MPEG_transport_stream&action=edit&redlink=1 "MPEG transport stream（頁面不存在）")，[H.264](https://zh.wikipedia.org/wiki/H.264/MPEG-4_AVC "H.264/MPEG-4 AVC")，[MPEG-4 SL](https://zh.wikipedia.org/w/index.php?title=MPEG-4_SL&action=edit&redlink=1 "MPEG-4 SL（頁面不存在）") [SMPTE VC1](https://zh.wikipedia.org/wiki/VC-1 "VC-1")和[MJPEG](https://zh.wikipedia.org/wiki/Motion_JPEG)

request /target product
https://www.nextvision-sys.com/dragoneye-2/
![[Pasted image 20250103170113.png]]
use Qualcomm , size too big, weight too heavy, functoin too much. ( outdise IC too much, ex, PMIC, DDR, flash...)
FPGA seems bettrt. ( PMIC less, DDR/flash in FPGA)