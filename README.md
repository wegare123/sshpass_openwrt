# sshpass_openwrt
mkdir -p package/sshpass
<br>
wget --no-check-certificate "https://www.dropbox.com/s/kr1hfprl5uwrm6u/sshpass-1.06.zip" && unzip sshpass-1.06.zip && rm -rf sshpass-1.06.zip
<br>
mv sshpass-1.06 package/sshpass/src
<br>
chmod +x package/sshpass/src/*
<br>
wget --no-check-certificate "https://www.dropbox.com/s/wp4asjlqjp2ah4s/makefile" -O package/sshpass/Makefile
<br>
make package/sshpass/compile V=99
