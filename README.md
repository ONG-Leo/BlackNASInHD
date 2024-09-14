黑群晖硬盘启动搭建教程

黑群晖 硬盘启动使用 安装说明

	1、需要2台电脑，一台安装黑群晖，一台调试电脑，一个U盘

	   黑群晖电脑需要3个硬盘，1号硬盘用来装黑群晖系统，2号和3号硬盘用来保存数据。1号硬盘容量超过8G即可。最好用固态硬盘速度快。2号和3号硬盘最好同厂家，同容量。

	2、利用调试电脑，把U盘制作成一个WINPE启动盘。同时拷贝黑群晖引导镜像文件到U盘内。

	3、黑群晖电脑，修改BIOS，设置U盘启动，保存重启

  4、黑群晖电脑，重启后U盘引导，进入WINPE环境

	5、黑群晖电脑，WINPE环境下，用磁盘工具打开群晖系统的引导镜像文件，制作虚拟硬盘VDD
 
	6、黑群晖电脑，使用磁盘工具的磁盘镜像功能，将虚拟硬盘VDD的内容 镜像拷贝到 1号硬盘上。1号硬盘等效成一个黑群晖的启动U盘（3-6步可以使用其他方式实现）。

	7、黑群晖电脑，重启电脑，修改BIOS，设置1号硬盘启动

	8、黑群晖电脑，重启后，进入黑群晖引导安装程序

	   按照黑群晖安装程序要求，将黑群晖的前置准备环境安装好

	9、调试电脑，打开黑群晖电脑提示的网址，使用浏览器环境将黑群晖的系统安装完成

	
参考教程1：
http://www.nas50.cn/
2024年NVMe/M.2固态硬盘 安装黑群晖教程 - 正经De网站 (nas50.cn)
![image](https://github.com/user-attachments/assets/646a7747-f8af-4847-822a-a2ee3925c873)
![image](https://github.com/user-attachments/assets/3e31d5ec-ef0f-4d56-960c-1b8c36e7b6a3)
![image](https://github.com/user-attachments/assets/ba3d38cb-61dc-4800-90d7-2d601f1ea786)
![image](https://github.com/user-attachments/assets/ee2492a2-6f5e-4d28-8ebf-0f12af5b72ba)
![image](https://github.com/user-attachments/assets/151d7c1b-9050-432d-b303-1bcc26506df2)
![image](https://github.com/user-attachments/assets/690a0b1e-77cd-42d1-a051-5f1cee037db8)
![image](https://github.com/user-attachments/assets/e477e861-0a1c-493e-b6c9-658eaa6107f7)
![image](https://github.com/user-attachments/assets/ded872da-4408-4033-bd39-458e49696849)
![image](https://github.com/user-attachments/assets/23b94c52-76fc-4671-a719-2a57d62de510)
![image](https://github.com/user-attachments/assets/d1ff3ab6-11f3-4268-a631-68f275478107)

引导镜像：

https://github.com/RROrg/rr/releases/tag/24.6.7

 ![image](https://github.com/user-attachments/assets/c1c06616-7d0c-4a6d-b896-1d8d90a9611b)

镜像制作工具

Index of /downloads (rufus.ie)

 ![image](https://github.com/user-attachments/assets/8d239e26-958e-4c8d-85c9-bdd2212964d1)

硬盘引导进入群晖
 ![image](https://github.com/user-attachments/assets/d536d383-7d7f-4e20-a0c6-416d582a9f39)
![image](https://github.com/user-attachments/assets/e0d32219-ce13-4328-9d6a-dac14d3ddd94)
![image](https://github.com/user-attachments/assets/2e000edb-aece-4c9a-aec6-005973b561c1)
![image](https://github.com/user-attachments/assets/8f14d6e5-f4e0-433a-9b92-9b562498dd99)
![image](https://github.com/user-attachments/assets/6269ae88-4078-4bf8-bf82-610390a870fc)
![image](https://github.com/user-attachments/assets/9979dab9-da16-4616-b635-d3394a964069)
![image](https://github.com/user-attachments/assets/396c8931-0b39-4dcc-82a9-fed6f5966dca)
![image](https://github.com/user-attachments/assets/094c5d8c-1868-4909-b69f-29120f5dc020)
![image](https://github.com/user-attachments/assets/b051a603-1f21-4193-bceb-83c4f5e1bb3a)
![image](https://github.com/user-attachments/assets/eed0e0a3-15a6-4ef1-9551-df3830c2d96d)
![image](https://github.com/user-attachments/assets/347c2acc-e2f3-45d5-a3f8-dcc88d0e777c)

实际安装截图部分

克隆磁盘后，电脑的固态硬盘就等效为一个引导U盘了，所以重启后，BIOS需要修改为电脑的固态硬盘启动。

重启后，看到这个界面开始参考前面设置即可。

不同的引导版本这里可能大同小异。

![image](https://github.com/user-attachments/assets/da70cc89-1ecc-46b4-93bb-1cdc34397f13)

通过网页配置和通过MENU.SH配置效果一样。

网页配置前，先用ping测试服务器是否准备OK。
![image](https://github.com/user-attachments/assets/94d07b51-835c-4997-acf9-f5af70a9a32b)
![image](https://github.com/user-attachments/assets/25d5db28-7028-48ac-9bff-b05e5ca6464e)
![image](https://github.com/user-attachments/assets/93041d43-fb1d-4c29-8027-eb9bd08b4807)
![image](https://github.com/user-attachments/assets/f5778e53-b1e0-4d07-8e34-4bae5315f863)
![image](https://github.com/user-attachments/assets/69ea22f1-ee45-4f41-a5b5-14d4cd2db1f4)
![image](https://github.com/user-attachments/assets/ec96a43b-d4c9-4c1d-989f-058eb874e35f)
![image](https://github.com/user-attachments/assets/2c58ff7a-fa2a-4b26-9795-c9037c7ac6ac)
![image](https://github.com/user-attachments/assets/0f27365a-9484-4554-8f3b-9b48d161a9ac)
![image](https://github.com/user-attachments/assets/27c7cf45-6107-47b7-95e4-a35785c94026)
![image](https://github.com/user-attachments/assets/0f64712f-ff5b-4c9c-ab15-84ffe7b9a31f)
![image](https://github.com/user-attachments/assets/6f1e481a-3273-49ea-95a1-1706bfb64f7e)
![image](https://github.com/user-attachments/assets/a49c0adf-dad4-41f9-8b3f-3535ba4ca2d2)
![image](https://github.com/user-attachments/assets/bfa982aa-0263-4ff3-9fc6-bbfee959c634)
![image](https://github.com/user-attachments/assets/675937a8-c4e3-4857-a1b7-9503170d25da)
![image](https://github.com/user-attachments/assets/affbc7ba-99dc-40e5-a61c-65245d2a29e9)
![image](https://github.com/user-attachments/assets/e214024e-b3b4-49c7-a075-a385be91e655)
![image](https://github.com/user-attachments/assets/0cf8e927-742a-46ab-84c4-2bb1c6a07e66)
![image](https://github.com/user-attachments/assets/2b5c7b67-1d79-4812-b147-3cea32d25b0f)
![image](https://github.com/user-attachments/assets/6d418e89-4441-4930-b549-23853337de39)
![image](https://github.com/user-attachments/assets/ad9a8239-daca-4d53-b9c5-29af58936479)
![image](https://github.com/user-attachments/assets/9b5825e5-93ee-48e6-926b-05a2e0806dd1)
![image](https://github.com/user-attachments/assets/910c1fcb-caae-46e2-91cc-97c99fb676ea)
![image](https://github.com/user-attachments/assets/46241b28-9cb1-4fae-92cf-a7dbb232ed3d)
![image](https://github.com/user-attachments/assets/26a2a152-d2be-406a-a5c2-fd5e70bc782f)
![image](https://github.com/user-attachments/assets/928a07fc-f469-4ce2-9806-b2ebf6f8b3d0)
![image](https://github.com/user-attachments/assets/e21cd944-3aa5-4982-81c5-f1a2c887e2ad)
![image](https://github.com/user-attachments/assets/ceaf6339-d082-4392-8662-7c72e14b9b33)
![image](https://github.com/user-attachments/assets/0ccc8aa7-8626-442c-8ee3-97b3015a6dc3)
![image](https://github.com/user-attachments/assets/8f24c204-e645-43d2-b4af-52673d0479f4)
![image](https://github.com/user-attachments/assets/fc9566f8-4deb-4225-b9cb-595e7541b40e)
![image](https://github.com/user-attachments/assets/1ec3ac97-9053-45e1-9a70-ba79371ef8bd)
![image](https://github.com/user-attachments/assets/fe3511b4-e12f-4850-a307-c68178cb8c27)
![image](https://github.com/user-attachments/assets/63b5e28d-7fa3-4cf1-b1f2-ec56f5a88f81)
![image](https://github.com/user-attachments/assets/97b2586e-2347-45d7-995e-2ef79ea0e8b0)
![image](https://github.com/user-attachments/assets/e687b988-f837-4493-9bc8-145041d60ebd)
![image](https://github.com/user-attachments/assets/fc26ca28-b2ca-44dc-881a-e0a314aedc40)
![image](https://github.com/user-attachments/assets/a12d18cd-734a-463c-8576-2e1406937c93)
![image](https://github.com/user-attachments/assets/8158f62a-e3bf-4529-ac6d-a981981330f5)

 
群晖社群
非常简单——进入到套件中心，依次点击设置➡套件来源➡新增既可，在这里新增的名称可以随便填写，但是位置要将以下的套件地址正确填入。
•	1、synocommunity社区，套件地址：https://packages.synocommunity.com
•	2、我不是矿神，套件地址：https://spk7.imnks.com/
•	3、云梦，套件地址：https://spk.520810.xyz:666
•	4、4sag，套件地址：https://spk.4sag.ru/
•	5、sysco，套件地址：http://synology.sysco.ch/
•	6、acmenet，套件地址：http://synology.acmenet.ru/
•	7、cphub，套件地址：http://www.cphub.net
•	8、裙下孤魂，套件地址：http://spk.bobohome.store:8880
