### Security System for a Topology built in GNS3

Assalamu Alaikum everyone,
In this project We have built a security system on a topology/network inside GNS3 to prevent it from Cyber attack such as **SQL Injection** and so on.

Now a days all Website, Apps we use by connecting to the internet are vulnerable to many cyber attacks. As a result all our public and private data going in the wrong hands. Data breach like these can cause many problems to us. So to prevent problem like these we need to secure the we have to take some masures.

So we have built a topology consists of 4 routers which contains their own networks consists of one switch and a PC. One of the PC is acting as a Web Server.

![Screenshot (340)](https://user-images.githubusercontent.com/60141836/207384006-ecc825b9-7b14-4c7c-a35e-79c28aa22fa8.png)

<br>
Still editing....
<br> <br>

**Team: Elation** <br>
**Members:**
1. *Ali Khatami (Leader)*
2. *Md. Rafidul Islam*
3. *Md. Hasanur Rohoman Khan*
4. *Md. Rokib Khan*
5. *Md. Arafatul Islam*


1. Ali Khatami (Leader)
2. Md. Rafidul Islam
3. Md. Hasanur Rohoman Khan
4. Md. Rokib Khan
5. Md. Arafatul Islam


- [] Installing GNS3
- [] Installing GNS3 VM
- [] Installing VMware Workstation Player
- [x] Write a blog
### Write some code<br>
Navigate to the downloaded floder.
- [x] Write some more code
- [x] Write some more more code

```
conf t
    int f0/0
        ip address 192.16.68.100 255.255.255.0
        no shut
        exit
```














### Building the Topology <br> <br><br>

Assalmualaikum,
I'm Mohammad Arafatul Islam. Me and my team is working on a project where we've built a security system on a topolgy inside GNS3 to protect it from **Cyber Attack**. I made the website that is put into the server PC. I did the followings:
<br>
- [x] Made the website. Source code is given above.
- [x] Made the website live so that it can be accessed from another PC in the same network.
<br><br><br><br>




I made the website for our project. The source codes are given above. Then I installed XAMPP and used it as our database also by using it I've made our website live in the same network.

First, I've put all our source codes in the folder named **htdocs** in the installation folder of XAMPP. To do that at first I've created a folder named **cn** in the htdocs folder<br>
![1](https://user-images.githubusercontent.com/60141836/209843031-bf5103b4-33a2-4a55-9e1e-7366586431d4.png)
<br><br>

Then I copied all the source codes into the **cn** folder<br>
![2](https://user-images.githubusercontent.com/60141836/209843033-688bab88-c87c-4a55-a2b7-b1ae3fc0bcc8.png)
<br><br>

Then open **XAMPP** and click **Start** on **Apache** and **MySQL**<br>
![3](https://user-images.githubusercontent.com/60141836/209842981-68ea7238-fa34-4956-9b93-58e9850357a7.png)
<br><br>

Then click **Admin** on **Apache**<br>
![4](https://user-images.githubusercontent.com/60141836/209842991-cf6c9063-72c1-44fd-aa2d-34f4744aa236.png)
<br><br>

This page will come up. Then I'll click **phpMyAdmin**<br>
![5](https://user-images.githubusercontent.com/60141836/209842993-28696341-1eac-41cf-b553-3ac7be7af523.png)
<br><br>

This page will come up. Then I'll click on **New** to create a new database<br>
![6](https://user-images.githubusercontent.com/60141836/209842996-7c84a989-4bd1-4ccf-a9aa-6b079144ea80.png)
<br><br>

Then I'll give the new database a name and the click **Create**<br>
![7](https://user-images.githubusercontent.com/60141836/209842998-81fb5fc7-d863-4df4-9551-a3f29f17f3db.png)
<br><br>

Database will be created. Then I'll go to the SQL tab and paste below code<br>
```
CREATE TABLE `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `username` varchar(100) NOT NULL,
  `email` varchar(100) NOT NULL,
  `password` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
<br>

Then I'll click **Go** on the bottom<br>
![8](https://user-images.githubusercontent.com/60141836/209891248-df21fed1-0e4a-4991-8815-8d8dfa3ac796.png)
<br><br>

We will get a success message<br>
![9](https://user-images.githubusercontent.com/60141836/209843002-68a7b359-8ecc-4e39-bb42-88360446c46a.png)
<br><br>

Now, we can see that new table **users** has been created under our new database. If we go there we can see that ```id``` ```username``` ```email``` ```password``` fields have been created<br>
![10](https://user-images.githubusercontent.com/60141836/209843006-73193285-0b1e-45ee-9794-f01cd162628d.png)
<br><br>

Now I can access it from the browser when I type **localhost/cn** here cn is our database name. <br>
![11](https://user-images.githubusercontent.com/60141836/209843007-de52b8d8-68a8-4827-9f7f-4a776878e103.png)
<br><br>

I can only access the Website from the host machine. Our project requires that, we have to be able to access the website from other computers in the same network. To do that first I'll go to the installation folder of XAMPP then **apache**->**conf** there is a file named **http.conf**. I'll open it<br>
![12](https://user-images.githubusercontent.com/60141836/209843013-4f5a2490-2bc7-4187-99e3-758270124cf1.png)
<br><br>

Then I'll add a line Listen **ip_address_of_the_device:port_number** in our case which is **172.16.68.50:8000** and then save the file<br>
![13](https://user-images.githubusercontent.com/60141836/209843022-fd5f654f-42be-46d3-949f-e389403dd570.png)
<br><br>

We can verify the IP address from cmd by the command ```ipconfig```<br>
![14](https://user-images.githubusercontent.com/60141836/209843026-d8ea9476-3fb7-4c5d-b6d6-03c1ef440f63.png)
<br><br>

After doing all that now we can finally access the website by its ip address from other computers in the same network<br>
![15](https://user-images.githubusercontent.com/60141836/209843028-94b1d700-9357-46ea-97a8-2ac80b6f2459.png)
<br><br>



https://mega.nz/folder/A1xARKoC#hePhI2TJjqjrkZ7Gq8qMcA

https://mega.nz/file/VEhwwICB#MWqOVjKyP9fuxHSlmfXDXdNc2jsnpMoNieeN1ZpBCKw

connected BlockChain2 <br>
connected BlockChain1



https://twitter.com/HRKHAN001/status/1619711315546869766?t=X3Yz19gbeUKOHOPPlLuoiQ&s=19



https://www.allthatnode.com/faucet/ethereum.dsrv <br>
0xA5FF30085aA000D091EA3112918f7F24FaA9b95f




Turorial: https://www.youtube.com/watch?v=M576WGiDBdQ

Ethereum Doc-1: https://geth.ethereum.org/docs
Ethereum Doc-2: https://docs.ethers.org/v5/
Ethereum Doc-3: https://ethereum.org/en/developers/docs/

Ethereum with Go language: https://geth.ethereum.org/docs
Chainlink: https://docs.chain.link/getting-started/conceptual-overview



https://slidesgo.com/search?q=blockchain#rs=search

https://slidesgo.com/new-theme/blockchain-company-profile#search-blockchain&position-1&results-126&rs=search



https://help.ubuntu.com/community/How%20to%20Create%20a%20Network%20Share%20Via%20Samba%20Via%20CLI%20(Command-line%20interface/Linux%20Terminal)%20-%20Uncomplicated,%20Simple%20and%20Brief%20Way!








### For Linux
Open terminal and navigate to the downloaded folder. Then run the following commands.

to unzip the file run this command:
```
sudo tar -xvf geth-linux-amd64-1.10.26-e5eb32ac.tar.gz
```

<br>Navigate to the extracted folder:
```
cd geth-linux-amd64-1.10.26-e5eb32ac
```

<br>Make the geth file executable:
```
sudo chmod +x geth
```

<br>Copy the geth file to /usr/local/bin directory
```
sudo cp geth /usr/local/bin
```

<br>to check the geth version:
```
geth version // to check the geth version
```
<br>If the installation is successful it will show<br>
```
Geth
Version: 1.10.26-stable
Git Commit: e5eb32acee19cc9fca6a03b10283b7484246b15a
Git Commit Date: 20221103
Architecture: amd64
Go Version: go1.18.5
Operating System: linux
GOPATH=
GOROOT=go
```


![Screenshot from 2023-03-10 08-41-01](https://user-images.githubusercontent.com/60141836/224209733-63a5467b-d096-4235-8977-0be89b3e545f.png)







# Hello World!
# Hello World! Ubuntu VM
