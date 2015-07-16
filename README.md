### Cells
[Cells](http://systems.cs.columbia.edu/projects/cells/) migrated from CS Software Systems Lab, Columbia

Manifest that contain Jelly Bean 4.3 branch

### Download Cells
You can freely download the Cells code using Github, however, if you plan on contributing to the Cells project, you need to be a registered developer. See the instructions on [contributing to Cells](http://systems.cs.columbia.edu/projects/cells/contrib/), and download the code using SSH. To save on bandwidth and local disk space, we have organized the repositories into groups. For example, when building on Linux it is not necessary to include all of the prebuilt Darwin toolchains, and vice-versa. You can pass a set of comma-separated groups to the repo init command. The current supported groups are:


- common – all the common source code and repositories

- linux – supporting binary tools necessary for a build on a Linux system

- darwin – supporting binary tools necessary for a build on OSX

- grouper – necessary repositories for the Nexus 7 (grouper)

- aosp – all repositories contained in the Android Open Source Project

The general format for initializing the Cells source code is:

    $ repo init -u https://github.com/RudyChin/cells.git -b [BRANCH] -g [GROUPS]
where:

- **[BRANCH]** will specify the Android release. Currently only cells-jb is supported for the Jelly Bean (4.3) build.

- **[GROUPS]** is the comma-separated list of repository groups, e.g.,**common,darwin,grouper** for building on OSX, and **common,linux,grouper** for building on Linux.
We recommend the following repo initialization commands for building on Linux and OS X (respectively):

We recommend the following repo initialization commands for building on Linux and OS X (respectively):


    $ repo init -u https://github.com/RudyChin/cells.git -b cells-jb -g common,linux,grouper
    $ repo init -u https://github.com/RudyChin/cells.git -b cells-jb -g common,darwin,grouper
After initializing the Cells source with one of the two above commands, you can download the code using:


    $ repo sync

For network trouble shooting issues and tips on saving network bandwidth, please refer to the [Android source download](http://source.android.com/source/downloading.html) page.

### Build
Please refer to this [page](http://systems.cs.columbia.edu/projects/cells/build/) for more detail.

### Contribute
Please refer to this [page](http://systems.cs.columbia.edu/projects/cells/contrib/)

### License
GNU [GPLv2](http://www.gnu.org/licenses/gpl-2.0.html)
