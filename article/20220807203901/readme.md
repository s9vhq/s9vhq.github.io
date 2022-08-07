<h1 style="font-size: 2.5em;"> ����Э��</h1>
 


# A2DP (Advanced Audio Distribution Profile)

高级音频传�?�规�?, 蓝牙音频传输模型协定, 允许传输立体声音频信号�??

A2DP是能够采用�?�机内的芯片来堆栈数据，达到声音的高清晰度�?�有A2DP的�?�机就是蓝牙立体声�?�机。声音能达到44.1kHz，一般的耳机只能达到8kHz。如果手机支持蓝牙，只要装载A2DP协议，就能使用A2DP耳机了�?�还有消费�?�看到技术参数提到蓝牙V1.0V1.1 V1.2 V2.0—�?�这些是指蓝牙的�?术版本，是指通过蓝牙传输的�?�度，他们是否支持A2DP具体要看蓝牙产品制�?�商是否使用这个�?术�??

# HSP (Headset Profile)

手机规格, 提供手机（移动电话）与�?�机之间通信�?�?的基本功能�??

HSP 描述了Bluetooth 耳机如何与计算机或其它Bluetooth 设备（如手机）�?�信。连接和配置好后，�?�机可以作为远程设备的音频输入和输出接口。这是最常用的配置，为当前流行支持蓝牙�?�机与移动电话使用�?�它依赖于在64千比特编码的音频/s的CVSD的或PCM以及AT命令从GSM07.07的一个子集，包括环的能力�?小的控制，接听来电，挂断以及音量调整。典型的使用情景是使用无线�?�机与手机进行连接�?�可能会使用HSP的若干设备类型：耳机、手机�?�PDA、个人电脑�?�手提电脑�??

# HFP (Handfree Profile)

免提规格, �? HSP 的基�?上增加了某些扩展功能，原来只用于从固定车载免提装置来控制移动电话�?

让蓝牙设备可以控制电话，如接听�?�挂断�?�拒接�?�语音拨号等，拒接�?�语音拨号要视蓝牙�?�机及电话是否�??

# AVRCP (Audio/VideoRemote Control Profile)

音频/视频遥控规格, 用于从控制器（如立体声�?�机）向目标设备（如装有 Media Player 的电脑）发�?�命令（如前跳�?�暂停和播放�?

AVRCP设计用于提供控制TV、Hi-Fi设备等的标准接口。此配置文件用于许可单个远程控制设备（或其它设备）控制所有用户可以接入的A/V设备。它可以与A2DP或VDP配合使用。AVRCP定义了如何控制流媒体的特征�?�包括暂停�?�停止�?�启动重放�?�音量控制及其它类型的远程控制操作�?�AVRCP定义了两个角色，即控制器和目标设备�?�控制器通常为远程控制设备，而目标设备为特征可以更改的设备�?�在AVRCP中，控制器将�?测到的用户操作翻译为A/V控制信号，然后再将其传输至远程Bluetooth设备。对于�?�随身听”类型的媒体播放器，控制设备可以是允许跳过音轨的耳机，�?�目标设备则是实际的播放器�?�常规红外遥控器的可用功能可以在此协议中实现。AVRCP协议规定了AV/C数字接口命令集（AV/C命令集，�?1394行业协会定义）的应用范围，实现了�?化实施和易操作�?��?�此协议为控制消息采用了AV/C设备模式和命令格式，这些消息可以通过音频/视频控制传输协议(AVCTP)传输�?

# OPP (Object Push Profile)

OPP是对象存储规�?, 蓝牙通信程序部分�?采用用于设备之间传输数据对象, �?般用手机蓝牙功能传MP3, 图片之类的都可以用OPP传输�?

OPP profile又细分为OPPC (client)端和OPPS(server)端profile，这两个profile区别在于只有client端可以发起数据传输的过程，但是附件设备与手机通信的情景中，既有手机发起数据传输请求也有设备侧发起传输请求的需要，�?以要在设备中实现OPPC和OPPS两个profile�?

# PBAP (PhonebookAccess Profile)

电话号码簿访问协议�??

# HID (The Human Interface Device)

HID定义了蓝牙在人机接口设备中的协议、特征和使用规程。典型的应用包括蓝牙鼠标、蓝牙键盘�?�蓝牙游戏手柄等。该协议改编自USB HID Protocol�?

1. HID Reports:Bluetooth HID devices支持三种Report：Input, Output, and Feature�?
1. HID建立Control Channel和Interrupt Channel两个通道，report可以在这两条channel上传输，在Control channel上传输的report称为synchronous reports ；在Interrupt channel上传输的report称为asynchronous reports�?
1. Feature reports are always transferred synchronously using GET_REPORT or SET_REPORT requests�?
1. Report Protocol Mode和Boot Protocol Mode。Bluetooth HID Hosts至少支持�?种，Bluetooth HID Device则需要支持Report Protocol Mode，并且Report Protocol Mode是Bluetooth HID Device的默认Mode�?

# PAN (Personal Area Network)

个人�?域网�?

蓝牙PAN使用的是传统蓝牙的技�?, 使用BNEP协议实现网络层到L2CAP层的协议映射, BNEP为蓝牙提供了�?种新的解决方�?, 之前在RFCOMM上面使用PPP协议来实现网络的共享, 即网络层与L2CAP层无须再插入PPP和RFCOMM�?, 直接插入BNEP�?, PAN包括三种角色: GN, NAP, PANU.



# 参�??

[A2DP -- 百度百科](https://baike.baidu.com/item/A2DP/9819331?fr=aladdin)

[OPP -- 百度百科](https://baike.baidu.com/item/OPP/13977547?fr=aladdin)

[蓝牙协议 HFP,HSP,A2DP,AVRCP,OPP,PBAP](https://blog.csdn.net/peng825223208/article/details/52072680/)

[蓝牙 HID 剖析 (�?) ](https://blog.csdn.net/xiaoxiaopengbo/article/details/51658396)

[蓝牙PAN](https://blog.csdn.net/hh20161314/article/details/104531424)