https://www.digikey.tw/zh/product-highlight/x/xilinx/zynq-ultrascale-mpsoc-zcu102-evaluation-kit

Altek AL6100
https://www.altek.com.tw/zh_TW/news-detail/node/1548825547001

[“BL” 通常是 “Base Length” 的縮寫，表示基準長度](https://zhidao.baidu.com/question/576119871.html)

ToF （Time-of-Flight）
[3D 技術：時差測距與雙目視覺 | Basler AG](https://www.baslerweb.com/zh-tw/learning/time-of-flight-stereovision/)

1. **Stereo Matching** 是一種從兩張不同角度的圖像中計算深度信息的技術。這種技術可以分為 **主動立體匹配 (Active Stereo Matching)** 和 **被動立體匹配 (Passive Stereo Matching)** 兩種。
    
    1. **主動立體匹配 (Active Stereo Matching)**:
        
        - [使用投影儀在場景中投射出特定的光學圖案（如紅外線圖案）來增加圖像的紋理](https://www.mdpi.com/1424-8220/22/9/3332)[1](https://www.mdpi.com/1424-8220/22/9/3332)。
        - [這些圖案幫助填補無紋理區域，使得匹配過程更加準確](https://www.mdpi.com/1424-8220/22/9/3332)[1](https://www.mdpi.com/1424-8220/22/9/3332)。
        - [常見於需要高精度深度信息的應用，如3D掃描和機器人導航](https://openaccess.thecvf.com/content_cvpr_2017/papers/Fanello_UltraStereo_Efficient_Learning-Based_CVPR_2017_paper.pdf)[2](https://openaccess.thecvf.com/content_cvpr_2017/papers/Fanello_UltraStereo_Efficient_Learning-Based_CVPR_2017_paper.pdf)。
    2. **被動立體匹配 (Passive Stereo Matching)**:
        
        - [僅依賴於場景本身的自然紋理來進行匹配](https://www.mdpi.com/1424-8220/22/9/3332)[1](https://www.mdpi.com/1424-8220/22/9/3332)。
        - [不需要額外的光源或投影設備](https://www.mdpi.com/1424-8220/22/9/3332)[1](https://www.mdpi.com/1424-8220/22/9/3332)。
        - [常見於消費級相機和一些自動駕駛技術中](https://openaccess.thecvf.com/content_cvpr_2017/papers/Fanello_UltraStereo_Efficient_Learning-Based_CVPR_2017_paper.pdf)[2](https://openaccess.thecvf.com/content_cvpr_2017/papers/Fanello_UltraStereo_Efficient_Learning-Based_CVPR_2017_paper.pdf)。
    
    3D算法轉移到RTL代碼（Register-Transfer Level，寄存器傳輸級別）是指將三維算法轉換為硬體描述語言（如Verilog或VHDL）的過程。RTL代碼用於描述數位電路中數據在寄存器之間的流動以及對這些數據進行的操作。

這個過程通常包括以下步驟：

1. **算法分析**：理解和分析3D算法的功能和需求。
2. **架構設計**：設計適合硬體實現的架構，包括數據路徑和控制邏輯。
3. **RTL編碼**：使用硬體描述語言編寫RTL代碼，描述數據流和操作。
4. **模擬和驗證**：通過模擬工具驗證RTL代碼的功能和性能，確保其符合設計要求。
5. **綜合和優化**：將RTL代碼綜合成門級網表，並進行優化以提高性能和效率。

這種轉換對於實現高效的硬體加速器非常重要，特別是在需要高性能計算的應用中，如圖像處理和計算機視覺。

MIPI D-PHY是一種結合高速、低功耗的訊號傳輸模式，主要應用於Camera (CSI)、Display (DSI)。

訊號組合1對Clock差分訊號以及1~4對Data差分訊號，支援HS mode (High Speed)和LP mode (Low Power) 模式之間切換。

空間精細化（Spatial Refinement）是一種技術，用於提高低解析度數據的空間解析度。
SR (Spatial Refinement): Refine 360p to 720p

[時域濾波（Temporal Filtering, TF）是一種技術，用於減少深度圖像中的閃爍現象。這種技術特別適用於 RGB-D 相機（如 Kinect），因為這些相機在捕捉深度圖像時，常常會出現噪聲和閃爍問題](https://dspace.zcu.cz/bitstream/11025/29713/1/Avetisyan.pdf)

