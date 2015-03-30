## JAVA JDK Installation (Ubuntu)

```sh
# Extract JDK
tar -xvf jdk-7u3-linux-i586.tar.gz
# Create Destination Folder
sudo mkdir -p /usr/lib/jvm/jdk1.7.0
# Copy Extracted Files to Destination Folder
sudo mv jdk1.7.0_03/* /usr/lib/jvm/jdk1.7.0/
# Set Symbolic Links for System Default Commands
sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk1.7.0/bin/java" 1
sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk1.7.0/bin/javac" 1
sudo update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/lib/jvm/jdk1.7.0/bin/javaws" 1
```
