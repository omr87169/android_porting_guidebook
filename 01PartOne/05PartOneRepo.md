An overly detailed guide to repo
================================

Quick Setup
-----------
It may be that you never need to use most of the advanced features of repo. If
you just want to port CyanogenMod to a new device, for example, you only need to
know about how to initialize, synchronise, and create manifests.  

###Initializing and Syncing a Repository
Developed by Google, repo is a tool used to download a large number of git
repositories using files called "manifests," which are XML files that describe
the location of a git repository and where to place it in the local source tree.
Since you are porting, you will eventually need to write your own repo local
manifests and include your source code.

####repo init
To get a copy of the Android source code, you need to initialize the repository,
naming a branch. This will install the "repo" tool in the directory where you
initialize the repository, under the hidden directory named ".repo" where all
it's data will be stored.

This command will initialize the Replicant Android variant repository in the
current directory.  
        
        repo init -u git://gitorious.org/replicant/manifest.git -b replicant-4.2

This does not download the repository for you, it simply sets up the repository
for download.  

####Explore the .repo folder

manifest.xml

manifests.git

manifests

local_manifests

project.list

projects

project-objects

repo

####repo sync
Now we download the contents of the source code repository using repo sync. Repo
will download everything listed in the manifest.xml file and everything listed
in an .xml file under the folder .repo/local_manifests  

It will take an annoyingly long-ass time.  

        repo sync

###Using Manifests to Import Supplemental Repositories
Manifests are used to add and remove repositories from your personal copy of the
source code. Since you're probably using this guide to port Android to your
own hardware, you are going to want to use git repositories and manifests.  

Manifests are housed in two directories, the .repo directory, and the 
.repo/local_manifests/ directory.

####Just Enough XML

####What's in a Manifest Line

####Local Manifests

####Example Local Manifest file

This is an example local manifest file which will import repositories for the LG
Optimus Logic.  

        <?xml version="1.0" encoding="UTF-8"?>
        <manifest>
          <project name="omr87169/android_device_lge_l35g" path="device/lge/l35g" remote="github" revision="2.3.7" />
          <project name="omr87169/android_kernel_lge_l35g" path="kernel/lge/l35g" remote="github" revision="2.3.7" />
          <project name="omr87169/android_vendor_lge_l35g" path="vendor/lge/l35g" remote="github" revision="2.3.7" />
        </manifest>

Advanced Guide
--------------

###


