### Cells
[Cells](http://systems.cs.columbia.edu/projects/cells/) migrated from CS Software Systems Lab, Columbia

Manifests for Cells on 

- Jelly Bean 4.3
- android-goldfish-3.4

This is a port version of Cells on Android Emulator

### Download Cells

For Linux users:

    $ repo init -u https://github.com/RudyChin/cells.git -b goldfish -g common,linux,goldfish,pdk

After initializing the Cells source with one of the two above commands, you can download the code using:

    $ repo sync

For network trouble shooting issues and tips on saving network bandwidth, please refer to the [Android source download](http://source.android.com/source/downloading.html) page.

### Build

    $ mv kernel-goldfish kernel
    $ source source-me.sh
    $ make -j4

### License
GNU [GPLv2](http://www.gnu.org/licenses/gpl-2.0.html)
