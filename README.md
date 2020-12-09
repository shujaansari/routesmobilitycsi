
Instructions to install routes mobility model on ns-3.31 UBuntu 18


After downlinading the files from the repo, run following commands

sudo apt install autoconf libtool libboost-dev libcurl4-openssl-
tar xvfz GeographicLib-1.50.tar.gz 
ls
cd GeographicLib-1.50/
./configure 
make
sudo make install
cd ..


tar xvfz curlpp_v0.7.4
cd curlpp-0.7.4/./autogen.sh 
./configure 
make
sudo make install


tar xvfz xerces-c-3.2.3.tar.gz 
cd xerces-c-3.2.3/
./configure 
make
sudo make install
cd ..
tar xvfz mobility-service-interface.tar.gz 
mv mobility-service-interface ns3-mmwave/src/


Building the module with ns-3

cd ns3-mmwave/
ls
./waf configure --enable-examples
./waf build



