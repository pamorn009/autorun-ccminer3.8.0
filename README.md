# AUTO RUN CCMINER IN TERMUX

แตะจอค้าง เลือก more
เลือก Keep screen on

```
termux-setup-storage
...
กดยอมรับ

## การติดตั้งตามขั้นตอน
```
apt-get update -y
```
```
apt-get install git -y
```
```
git clone https://github.com/pichetx/autorun-ccminer3.8.0
```
```
cd autorun-ccminer3.8.0
```
```
chmod +x setup.sh && sh setup.sh
```
* หลังจากเปิดไฟล์ bash.bashrc เพิ่มบรรทัดแรกเป็น
- ```run-miner```
* แล้ว save

## เพิ่มเติมการใช้โปรแกรม
* หากต้องการหยุดขุดให้ใช้กด ```CTRL + C```
* หากต้องการเปลี่ยน TAG ใช้คำสั่ง ```edit-miner```
* หากต้องการเปิดขุด ใช้คำสั่ง ```run-miner```
* หากต้องการอัพเดทโปรแกรม ใช้คำสั่ง ```cd && cd ../etc/mobile-mining && python3 update.py && cd```
