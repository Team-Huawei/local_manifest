LineageOS For Huawei Y6 codename ("scale")
==========================================

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/los

Next, naviate into that new directory via the terminal:

	cd ~/los

To initialize your local repository using the Turbo ROM trees, use this command:

	repo init -u git://github.com/LineageOS/android.git -b cm-14.1

Also add the local manifests:

	git clone https://github.com/Huawei-scale/local_manifest -b cm-14.1 .repo/local_manifests

Then sync up with this command:

	repo sync --force-sync
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

First:

	cd ~/los

Second:

	$ echo "export USE_CCACHE=1" >> ~/.bashrc
	$ prebuilts/misc/linux-x86/ccache/ccache -M 30G

Third:

	. build/envsetup.sh
	brunch scale

-------------
 
_Developers contributors_
---------------

	@giorgio130
	@CarlosArriagaCM
	@DestructoSphere
	@Runner85sx
	@nzh21

