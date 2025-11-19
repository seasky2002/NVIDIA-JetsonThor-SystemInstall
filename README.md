# NVIDIA-Thor-System-Install
Nvidia AGX Thor安裝log

I. 硬體準備:
  1. NVIDIA AGX Thor本體
  2. 官方提供的變壓器(type-C頭)
  3. HDMI傳輸線(以方便在螢幕上操作)
  4. 鍵盤
  5. 空間大於16GB的隨身碟(系統碟)
  6. 一臺電腦(用來灌系統碟)

II. 軟體準備:
  1. Jetson 官方鏡像檔:https://developer.nvidia.com/embedded/jetpack/downloads
  2. Etcher系統燒錄套件:https://etcher.balena.io/#download-etcher

III. 安裝流程:
  1. 先在隨身碟上用Etcher燒錄官方鏡像檔，燒錄好之後插到Jetson的USB端口，並接上HDMI線、鍵盤，供電可以直接插Jetson的兩個type-C插口其中一個
  2. 開啟電源後，理論上會進入GNU GRUB的畫面，此時點選第一個"Jetson Thor options"
       如果沒有成功，而是進去以下畫面，則先輸入exit，而後進入Boot Manager，把USB拉到第一啟動位
  3. 進入之後，點選第一個"Flash Jetson AGX Thor Developer Kit on NVMe 0.2.0-r38.2"，這代表將系統燒錄到硬體裡(第二個選項就是將系統燒到USB內)
  4. 點選之後，等待15分鐘
     
