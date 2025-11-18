# Installing-TensorFlow-on-Raspberry-Pi-4B-arm-71
关于树莓派4B arm71架构，opencv+tensorflow训练识别图像处理的一些踩坑建议：
1、关于树莓派的arm71架构，与64位新系统不同，许多软件和环境无法兼容，只能通过安装特定版本的opencv 和 tensorflow版本
2、直接调用pip 命令本地安装如上的whl文件，由于树莓派的性能过低，训练模型的难度较大，可以通过虚拟机Ubuntu（乌班图）18.04系统安装相同版本的tensorflow训练模型，注意后缀要一致为2.5.0
3、在后续使用模型可视化界面需要安装models文件夹，通过clone相关库，或者在本地下载相关压缩包，传输到树莓派4B中
4、由于树莓派4B arm71架构，许多vpn软件无法兼容，导致pip命令 和apt 命令下载速度太慢导致超时，因此建议在虚拟机中下载相关的文件，通过局域网传输到树莓派中本地安装
Regarding the Raspberry Pi 4B arm71 architecture, here are some tips for troubleshooting OpenCV + TensorFlow image recognition training:
1. Due to the Raspberry Pi's arm71 architecture, unlike newer 64-bit systems, many software and environments are incompatible. You may need to install specific versions of OpenCV and TensorFlow.
2. Directly using pip to install the above whl file locally is not recommended due to the Raspberry Pi's limited performance and the difficulty of training models. It's advisable to install the same version of TensorFlow on a virtual machine (Ubuntu 18.04) to train the model. Ensure the file extension is consistent (e.g., 2.5.0).
3. When using the model visualization interface, you'll need to install the `models` folder. This can be done by cloning the relevant libraries or downloading the necessary compressed packages locally and transferring them to the Raspberry Pi 4B.
4. Due to the Raspberry Pi 4B's arm71 architecture, many VPNs are incompatible, causing slow download speeds and timeouts with pip and apt commands. Therefore, it's recommended to download the relevant files in a virtual machine and transfer them to the Raspberry Pi for local installation via a local network.
