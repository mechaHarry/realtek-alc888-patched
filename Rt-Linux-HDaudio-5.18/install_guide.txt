The source code copy from www.alsa-project.org.      ver:5.15
Linux Source Code for ALC audio codec
Support Codec list:
====AC97 Codec=====
ALC100,100P
ALC200,200P
ALC650D
ALC650E
ALC650F
ALC650
ALC655
ALC653
ALC658
ALC658D
ALC850
ALC101
ALC202
ALC250
ALC203

====HD Audio codec ====
ALC221
ALC231
ALC233
ALC255
ALC260
ALC262
ALC267
ALC268
ALC259
ALC269
ALC270
ALC271X
ALC272
ALC273
ALC275
ALC276
ALC280
ALC281X
ALC282
ALC283
ALC284
ALC285
ALC286
ALC288
ALC290
ALC292
ALC293
ALC656
ALC660
ALC660VD
ALC661
ALC662
ALC663
ALC665
ALC668
ALC670
ALC671
ALC672
ALC680
ALC861
ALC861VD
ALC880
ALC882
ALC883
ALC885
ALC888
ALC889A
ALC898
ALC892
ALC899
ALC900
ALC1150
ALC1200


Installation:
This Source Code is from www.alsa-project.org.
For OS installation, please remember add the Development tool kit.
For driver installation, please follow below steps. 

Note: Please check Development tool kit on your OS.   

Manual install:
Step 1. unzip source code
        tar xfvj alsa-driver-1.0.xx.tar.bz2

Step 2. Complied source code
	a. cd alsa-driver-1.0.xx
	b. ./configure --with-cards=hda-intel
	c. make
	d. make install

Step 3. reboot your machine

Step 4. Use the alsamixer the disable mute (All audio line default is mute)
        excute alsamixer

Note: 	1. The most detail information, can refer the alsa-kernel/Documenttation/ALSA-Configuration.txt in the azx-021705.tar.bz2.
	2. Kernel Version must be 2.6 or later.
	3. All mixer channels are muted by default. You must use a native
		or OSS mixer program to unmute appropriate channels.
	4. If can not compile the source code, try to rename the /usr/src/linux-2.x -> /usr/src/linux.
	5. The driver added to support the SPDIF functoin. 	
	6. a. You can download the alsa-lib-1.0.x and alsa-utils-1.0.x form the www.alsa-project.org, then unzip and install them. 
	   b. Suggest use "alsamixer" to control mixer function.
	   c. Used "alsaconf" can autodetect which drive you need to install (step 4). 	
        7. SUSE Distribution must install the ncurses package. 
