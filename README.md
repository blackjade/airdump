AirDump
-------
Dumping WiFi frames in RadioTap format. Need libpcap, and a wireless interface which supports "Monitor" mode.  

Instructions for Compilation
----------------------------

Compiling the sniffer follows the steps of standard CMake based build.

Basically, just run the following steps in the source directory:

```
mkdir bin
cd bin
cmake ..
make
```

This will create a `airdump` file which can then be used to sniff packets from an wireless interface.

Usage Syntax
------------

Running `./wifi-sniffer` without any parameters shows the usage

```
Usage: ./wifi-sniffer [options] interface
  -m, --macstat   : Show number of detections of each MAC and timestamps
  -t, --time t    : Run sniffer for t seconds (default: 60)
  -v, --verbose   : Output more information
  -d, --debug     : Show debugging information
  -h, --help      : Show this help text

Note: This program needs to be run as root
```

Do note that you need to have a wireless interface which supports "Monitor" mode to be able to use this software.

Legal
-----

Please read the [LICENSE](LICENSE) file to know legal details of how you are allowed to use this software. But in short, this software is licensed under MIT License.

Disclaimer
----------

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
