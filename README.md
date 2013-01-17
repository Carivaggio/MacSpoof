MacOSX by default doesn't let you permanently change your MAC Address.
Every time you restart your address is set to whatever was before the restart.

To enable startup MacSpoofing you have to follow the instructions listed below

Startup Installation Instructions :

    mkdir -p /tmp/MacSpoof
    git clone https://github.com/harshavardhana/MacSpoof.git /tmp/MacSpoof
    cd /tmp/MacSpoof
    sudo mkdir /Library/StartupItems/MacSpoof
    sudo cp MacSpoof StartupParameters.plist /Library/StartupItems/MacSpoof
    cd /Library/StartupItems/MacSpoof
    sudo chown root:wheel MacSpoof StartupParameters.plist
    sudo chmod 0755 MacSpoof
    sudo chmod 0644 StartupParameters.plist

That's it you are good to go from next restart
