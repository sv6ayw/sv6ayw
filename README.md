- š Hi, Iām @sv6ayw
- š Iām interested in ...openwebrx in pc linux and setup sdrplay not work
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
sv6ayw/sv6ayw is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


1installAPI.sh
SDRplay_RSP_API-Linux-3.07.1.run
2buildSoapy.sh

OPENWEBRX INSTAll and SETINGS

wget -O - https://repo.openwebrx.de/debian/key.gpg.txt | apt-key add
echo "deb https://repo.openwebrx.de/ubuntu/ hirsute main" > /etc/apt/sources.list.d/openwebrx.list
apt-get update
apt-get install openwebrx

AND LAST THIS

git clone -b master https://github.com/jketterl/owrx_connector.git
cd owrx_connector
mkdir build
cd build
cmake ..
make
sudo make install
