# PDL
researching about PDL file format

## Partition
PDL파일 끝부분 4자리를 읽으면 SectionInfo 시작점 위치가 나옴 (int)
또한 해당 시작점의 숫자는 PDL Version
그리고 바로 다음 4자리는 PDL Checksum (SectionInfo를 제외한 
※IM-100 PDL은 다름  
각 파티션의 정보 사이즈는 96Byte  
No. 번호는 파티션 번호를 의미 (No.10 PHONEINFO 은 mmcblk0p10)

## Checksum
Checksum 32bit (Use Winhex Compute Hash)

### IM-A770K_S0833317.pdl
![IM-A770K_S0833317.pdl](/image/IM-A770K_S0833317.jpg)

### IM-A870K_S0839213.pdl
![IM-A870K_S0839213.pdl](/image/IM-A870K_S0839213.jpg)

### IM-A910K_S0844131.pdl
![IM-A910K_S0844131.pdl](/image/IM-A910K_S0844131.jpg)

### IM-A910S_S0224129.pdl
![IM-A910S_S0224129.pdl](/image/IM-A910S_S0224129.jpg)

## Binwalk
PDL파일을 Binwalk 사용해서 분석한 파일들
<pre><code>IM-A800S_S0212317.pdl
IM-A840S_S0215224.pdl
IM-A870K_KFVN.S01.pdl
IM-A870K_S0839213.pdl
IM-A870L_S1235210.pdl
IM-A870S_KFVN.S01.pdl
IM-A870S_S0218215.pdl
IM-A880S_S0221220.pdl
IM-A890K_S0842214.pdl
IM-A890L_S1237219.pdl
IM-A890S_S0222216.pdl
IM-A900K_S0843237.pdl
IM-A900L_S1238232.pdl
IM-A900S_S0223237.pdl
IM-A910K_S0844131.pdl
IM-A910L_S1239127.pdl
IM-A910S_S0224129.pdl
IM-A920S_S0225122.pdl
IM-100K_S0850122.pdl
IM-100S_S0228122.pdl
</code></pre>
