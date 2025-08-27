---
Title: "Controller"
Author: "Nithling"
Description: "A custom 3D printed controller"
Created On: "13/08/2025"
---

# August 13th: Creating the profile sketches!

Created the profile sketches for the side and top of the controller grips using splines. Then experimented in adding additional splines along the length of the grips to try loft the entire grip.

<img width="450" height="221" alt="image" src="https://github.com/user-attachments/assets/b52ccb11-db53-4001-8d91-596240fb9c58" />
<img width="539" height="438" alt="image" src="https://github.com/user-attachments/assets/df65f12d-4b5d-4317-b554-798c73a9525f" />

**Total time spent: 3.5h**

# August 14th: Finished hand grips

Remade the wireframe for the grips using 3d splines and lofted the surfaces to make a solid object that will be the hand grips. This took a lot of trial and error.

<img width="999" height="565" alt="image" src="https://github.com/user-attachments/assets/f2195076-1026-4ce1-9257-4d8b04b4aa17" />

**Total time spent: 3hr**

# August 15th: Redid hand grips
Once again I redid how I lofted the grips, I instead used two lofts instead of 4 and used fewer curves as guides to create a more natural shape. I also angled the grips away from the centre which took a lot of trial and error as well as redoing many of the sketches as they kept breaking due to some geometry being defined weirdly.

<img width="518" height="562" alt="image" src="https://github.com/user-attachments/assets/3db6e3fc-98de-4b71-8ffb-c4c2cf54c7d8" />
<img width="1253" height="541" alt="image" src="https://github.com/user-attachments/assets/ebcdf363-a1a2-4582-8720-e7dcb022a167" />


**Total time spent: 3hr**


# August 16th: Sketching rest of body
Drew the sketches for the rest of the body

<img width="1059" height="589" alt="image" src="https://github.com/user-attachments/assets/a487782e-ac62-40d0-af69-16b86493023c" />

**Total time spent: 15min**

# August 24th: Faliure
Made a crude loft for the centre of the body but discovered that I was not able to shell the hand grips. Spent several hours trying to change the geometry of the grips to be able to be shelled  but was not able to. In the end I had to just leave part of the grip solid and try to fit the electronics around it.

<img width="494" height="369" alt="image" src="https://github.com/user-attachments/assets/e3d386b7-816f-4335-a84b-4501fc5fff4a" />

**Total time spent: 4hr**

# August 25th: Adding Electronics
Started sketching out all the locations for the electronics and other components. Not physically having the components made it much more difficult to plan where they would go as I was not able to see how they would fit together. This was further complicated by the fact that many of the components do not have proper documentation for their dimensions. I also decided to mount the pico and some other items like the buzzer and accelerometer on veraboard as it gave me more flexbility in how I could place componenents. I also began extruding the mounts for some of the components which was difficult as the surface of the controller was not flat and was instead curved and also on an angle. This was particuarly hard for the mounting of the joystick as I had no physical model or drawings to work with and creating the correct holes that would fit the joystick(ended up guestimating). Creating the geometry for the holes was also very difficult and took a lot of trial and error. (second time writing this :(, forgot to commit edits)

<img width="834" height="466" alt="image" src="https://github.com/user-attachments/assets/43fc8494-dbba-40f2-b5e6-24fb50c4ac5b" />
<img width="1183" height="631" alt="image" src="https://github.com/user-attachments/assets/3ca07211-a3f2-4523-939b-c0d9b7f3b312" />


**Total time spent: 4hr**

# August 26th: more of ^^^^
Continued creating the mounting for the electronics such as finalising the mounting point for the joysticks, the power button and creating a hole for micro usb cable for the pico. Smoothed out some of the mounting points on the top surface using drafts and fillets. Next step is to create the holes to connect the two halves together

<img width="1646" height="686" alt="image" src="https://github.com/user-attachments/assets/548259e2-79e0-43f9-a56b-e6e72a1a5e3f" />
<img width="603" height="433" alt="image" src="https://github.com/user-attachments/assets/260386be-0544-48b7-8585-20bbc8836aaf" />
<img width="283" height="193" alt="image" src="https://github.com/user-attachments/assets/98b429fb-4400-4e7f-91d4-4b4f5da3818d" />

**Total time spent: 2hr**

# August 27th: Finalising Design
Added the holes to connect the two halves of the controller together. Added chamfers on the various mounting posts to help ensure they do not snap off as well as chamfers on the holes to aid in getting screws into the part. I searched for a bit(some of the total time includes finding suitable components that I could use) to find a LiPo battery charger that I could add to the pico so that i can charge the LiPo without removing it from the case. I did some calculations to determine that if the pico w drew around 100mA, a 200mah LiPo battery should be able to power it for 2hr however without knowing the current draw of thhe other periphals this would likely be less.

<img width="1079" height="636" alt="image" src="https://github.com/user-attachments/assets/d905b943-5b3f-4575-b0a9-6fefd91ea1d7" />
<img width="1111" height="495" alt="image" src="https://github.com/user-attachments/assets/e1606b45-21aa-4dc3-bf8b-2facff346f2c" />

**Total time spent: 2hr**

BOM:

* 2x Joystick https://www.amazon.com/HiLetgo-Controller-JoyStick-Breakout-Arduino/dp/B00P7QBGD2/ref=sr_1_1_sspa?crid=KYT8WOXR70KB&dib=eyJ2IjoiMSJ9.u3HQgtLAVkNqZIGo3SvKEA7RskrJilcONKhjTH6egbTEWsr7WmupRZueitZ0x5hb7Cb4Yzew3gl9MiQhRmm7nOaB5gvGEq_MVG3k2icl3Oh-C00FafB827dkG6ojczR_bHUl-RXigeR6rSJXhj7r9eQCIMyzqlzdLEC3AkdGUIn3BtYUesnvFV6Urj0GIB6SpwnTdvdlM-ZATm4RWD2DLwYgTgtgBzqP1BDzUuNp46M.t2rhjNqCVw5MOI6deHCI6IE1kL_NqTWg6scY0_GoipE&dib_tag=se&keywords=Joystick+module&qid=1753994354&sprefix=joystick+modu%2Caps%2C132&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1

* 1x accelerometer https://www.amazon.com/HUAREW-MPU6050-Gyroscope-Accelerometer-Converter/dp/B0CRVR1P66/ref=sr_1_2_sspa?crid=CTOWJJKNW0L8&dib=eyJ2IjoiMSJ9._zRQIjLy8SJUb458TCsORc8ZhQjoyMgCOrU-agTTG_xrWYf4yKToVOe1l5yPHYQoS5tOqvsrEvDqiKAprtgPPJkV5b9dVLMxRw60lF3AQI-Q0Q3o8onIPsuC50Qo169MJO-V5KFh1VldFRw-SVZIk2nGnhvKKk6kCAl3AV6bSGOpw-0wfF7z7TMeQWQ2wyaYbBsgIh67fdMxgyBsoXbyf5YrhsPYKgN157Dh1TaiO0k.JxQlPk08Al-afuWwE5dMTx2sxM8SSHjSp5Ln7J6WHZ4&dib_tag=se&keywords=MPU6050&qid=1754065568&sprefix=mpu6050%2Caps%2C111&sr=8-2-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1

* 8x small buttonhttps://www.amazon.com/DAOKI-Miniature-Momentary-Tactile-Quality/dp/B01CGMP9GY/ref=sr_1_3?crid=3LVXY81MDD2D8&dib=eyJ2IjoiMSJ9.K8ztKL3l65wCk2uoh4BBBHHPZV-A3oKg2_qkEgKbg2dJ-XoTQh6fU61cTVXCZeLWbmcVmOXfH9rC8N14ti0ezSGgYY4VvpOD6F-CQwFaWiT5HMFhTj_KxQr4sM8f1QaTMKgbZxIT7wCFOpcjqnCSxeAMCTTyw4Ug9DJU3rTsj3BGn_z_VvkrWYUTW2ViqQ2F9s90jOr9Lr9J5XI0_Vus44LPOuFmrcQq1kB8sCprjBWCQyA67OoRHOIQYSCO_8BgwwCzIwnkO_ejQL5aHebcZnGwkBEoaM_jajL7jB2_tPE.bpiHyW0VSub5KoPw7Zsew1WifKI6gRyIhn1XCoys1OQ&dib_tag=se&keywords=button%2Bfor%2Bpcb&qid=1753993505&s=industrial&sprefix=button%2Bfor%2Bpcb%2Cindustrial%2C106&sr=1-3&th=1

* 1x buzzer https://www.amazon.com/mxuteuk-Electronic-Computers-Printers-Components/dp/B07VK1GJ9X/ref=sxin_16_pa_sp_search_thematic_sspa?content-id=amzn1.sym.3afbfb03-37f9-433d-812b-5618f5fce9ff%3Aamzn1.sym.3afbfb03-37f9-433d-812b-5618f5fce9ff&crid=3MTRB51RSXNE5&cv_ct_cx=piezo+electric+buzzer&keywords=piezo+electric+buzzer&pd_rd_i=B07VK1GJ9X&pd_rd_r=a2ef178e-056a-4cc1-9c17-70a39eb765f1&pd_rd_w=W8bRn&pd_rd_wg=0PDGW&pf_rd_p=3afbfb03-37f9-433d-812b-5618f5fce9ff&pf_rd_r=RMG1HGAXD1S8A3GMT8QH&qid=1753993828&s=industrial&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=piezo+ele%2Cindustrial%2C111&sr=1-1-6024b2a3-78e4-4fed-8fed-e1613be3bcce-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&psc=1

* 1x segment led display https://www.amazon.com/Bestol-Segment-Digital-Display-Bright/dp/B07F11P2X9/ref=sr_1_1_sspa?crid=1FI3VFYYT44UZ&dib=eyJ2IjoiMSJ9.mb1oB5LQW9eDu7dFGDQkwKmAOz1d7PCNFlB3vSyy2LjU2aGJLSZ7RZf5XoFwW1M4tUD7YlHiEdqDjYYzbwIQZZ5Ahn_xxtZ2TEbtSJ4ASl585aQKHq9SW8wpTLVim0dkvTPH2a-2Uv-QGEBXivhRiRT6SfiiGqFLpQzf2vADmdTQtKrJPBBvtpyqEhkrVWF8Wr1LR9ytGUvrPNMH02pvJkIprlebZW-CxRUB7EOCL4A.2qmpnm3pgIbcT3EEtZ-kVW42iazFl0UlWs3ctP6T5UM&dib_tag=se&keywords=LED%2BBar%2BGraph&qid=1754057982&sprefix=led%2Bbar%2Bgraph%2Caps%2C286&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1

* 2x pot https://www.amazon.com/DIYhz-Rotary-Encoder-Digital-Potentiometer/dp/B07D3DF8TK/ref=sr_1_9?crid=2YI39WSAQUZC1&dib=eyJ2IjoiMSJ9.Cv5zJCxgmluCk3m2K7331Qwt5khelIvbEEsAhHX8KoOrz1c5vWVc_OcJj9NBuSiY5b_utQMUjLxCkpjmR7Enr0GyOPzEwCSudVj5vrIZ3ZoD5m5Ev3LWQvx6I71SL0ulrj0gG-Qj3D2C6-OA4J2U24IBLbbCED8Hs6-jvpFonkqPdU-9n5vYxJr7OgiGE13V84OtMyyLf6-ouEesV1dsV9BDuv7tfxHoTc7kakS3qkk.KbdX1mnt_iHBjLFkTRqGgC-DEMSIkOA-5R8iW4dBm5o&dib_tag=se&keywords=PCB+Encoder&qid=1753994705&sprefix=pcb+encoder%2Caps%2C114&sr=8-9

* 1x 1.8 screen https://www.digikey.com/en/products/detail/adafruit-industries-llc/358/5801368?gclsrc=aw.ds&gad_source=1&gad_campaignid=20228387720&gbraid=0AAAAADrbLlj6J1-CXjMvB2poJDP6vXZk8&gclid=Cj0KCQjwtMHEBhC-ARIsABua5iSUqiseLrZ0jIoWnQQAKtPOi3Fta5P42dNPiDKyF84q20x1jw7Lat0aAqg6EALw_wcB

* 1x analog/digital breakout https://www.sparkfun.com/sparkfun-analog-digital-mux-breakout-cd74hc4067.html or https://www.adafruit.com/product/5836?srsltid=AfmBOopbR_FtnUanDIy2z5l5viOq5bFq5tQ5RCXxs68W7XwBSWc96bWj

* 1x Power button https://www.aliexpress.com/item/1005006090350341.html?

* 1x pi pico header kit https://core-electronics.com.au/header-kit-for-raspberry-pi-pico.html

* 1x veraboard https://www.jaycar.com.au/pc-boards-vero-type-strip-95-x-152mm/p/HP9542?srsltid=AfmBOoqQs_fIcNC6aYXQac2ZbTbnSsgYArLCiu_3CRI3g2MDDvFBJ_Ss
  
* 1x solid core wire https://core-electronics.com.au/hook-up-wire-spool-black-25-ft.html
  
* 1x EYESPI breakout and cable for  1.8screen https://www.adafruit.com/product/5613 https://www.adafruit.com/product/5239

* 1x LiPo battery https://www.auselectronicsdirect.com.au/rechargeable-li-po-battery-3.7v-200mah-for-nh010-t

* 1x LiPo battery charger https://core-electronics.com.au/pimoroni-lipo-shim-for-pico.html
