# Install Carbonite
## Source Server, Target Server, & Console Server 
### Windows
- Double click DoubleTake_8.4.1.458.0.exe <br>
![image carbonite](assets/1.png) <br>

- Pilih Install Carbonite Availability <br>
![image carbonite](assets/2.png) <br>

- Pada menu Carbonite Replication - InstallShield Wizard pilih button Install <br>
![image carbonite](assets/11.png) <br>

- Pada menu Welcome to the Installation Wizard for Carbonite Replication, Pilih No, Skip this step and continue the current installation <br>
![image carbonite](assets/3.png) <br>

- Pada menu License Agreement, pilih I accept the terms of services <br>
![image carbonite](assets/4.png) <br>

- Pada menu License Activation, pilih Next <br>
![image carbonite](assets/6.png) <br>

- Pada menu Setup Type, pilih Client and Server Components lalu Next <br>
![image carbonite](assets/7.png) <br>

- Pada menu Windows Firewall Configuration, pilih open only the ports that are not in use <br>
![image carbonite](assets/5.png) <br>

- Pada menu License Key Information, pilih Next <br>
![image carbonite](assets/8.png) <br>

- Pada menu Queue Options, pilih Next <br>
![image carbonite](assets/9.png) <br>

- Pada menu Security Groups, pilih Next <br>
![image carbonite](assets/10.png) <br>

- Pada menu Ready to Install the program, pilih Install <br>
![image carbonite](assets/13.png) <br>

- Tunggu hingga proses install selesai <br>
![image carbonite](assets/12.png) <br>

- Pilih Finish <br>
![image carbonite](assets/14.png) <br>

- Untuk mengecek apakah sudah berjalan service dari carbonite, cari pada search bar start **Services**
- Cari Double-Take Management Service & Double-Take makan akan terlihat status Running. <br> 
![image carbonite](assets/21.png) <br>

### Linux
- Donwload terlebih dahulu DoubleTake_8.4.1.458.0-1.x86_64.rpm (Oracle Linux, rhel, CentOS) atau DoubleTake_8.4.1.458.0_amd64.deb (Debian dan Ubuntu)
- Jalankan pada syntax pada local terminal scp DoubleTake_8.4.1.458.0-1.x86_64.rpm user@ip-public:/directory/directory tujuan.
- Masuk ke server linux, jalankan perintah ```rpm -ivh DoubleTake_8.4.1.458.0-1.x86_64.rpm``` tunggu hingga selesai proses install
- Jalankan perintah ```DTSetup```
- Accept the License Agreement. Press **ENTER** to view the complete agreement.
- Press **Q** and Type **YES** to accept the agreement.
- Press 2 – To Start/Stop Double-Take daemon
- Press 1 – To Start Double-Take and process driver config
- Now we can see the DT process and Modules are running.
- Now exit from the menu by pressing **Q** twice.

## Add Server pada Carbonite Console Server
- Pada console carbonite pilih Add Server <br>
![image carbonite](assets/22.png) <br>

- Pada menu Add Servers, isi kolom server dengan IP dari server tersebut, isi kolom User Name dengan user login server tersebut, isi kolom Password dengan password login server tersebut, apabila ada Domain isi dengan domain server tersebut <br>
![image carbonite](assets/23.png) <br>

- Lalu pilih Add dan OK

# License
- Target Server (Windows)
  - Pada targer server Install DTMUConfiguratorSetup.exe <br>
  ![image carbonite](assets/15.png) <br>

  - Pada menu Welcome to the Metered Usage, pilih Next <br>
  ![image carbonite](assets/16.png) <br>
  
  - Pada menu Destination Folder, pilih Next <br>
  ![image carbonite](assets/18.png) <br>   
  
  - Pada menu Ready to Install Metered Usage Configurator, pilih Install <br>  
  - Apabila telah selesai maka pilih Finish <br>
  ![image carbonite](assets/17.png) <br>
  
  - Pada target server pilih menu start, lalu cari Metered Usage Configurator dan double click <br>
  ![image carbonite](assets/19.png) <br>
  
  - Isi kolom sesuai License Carbonite yang dimiliki <br>
  ![image carbonite](assets/20.png) <br>

- Source Server
  - Buka carbonite console yang ada pada instance console <br>
  - Pilih source server, klik kanan properties

# Open Port Carbonite
- ICMP ALL
- UDP 6326
- TCP 6326
- UDP 6320
- TCP 6320
- UDP 6325
- TCP 6325
- TCP 1506
- TCP 1501
- TCP 1500
