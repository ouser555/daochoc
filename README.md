# daochoc
daochoc, zmk config, nrfMicro1.4

daochoc資料夾放到 zmk/app/boards/shields/底下


執行


west build -d build/left -b nrfmicro_13 -- -DSHIELD=daochoc_left


west build -d build/right -b nrfmicro_13 -- -DSHIELD=daochoc_right


燒錄檔於


zmk/app/build/left


zmk/app/build/right


* 簡易說明
  * 此鍵盤預設有四層，default/lower/raise/adjust
  * 右手鍵盤靠拇指的下方三個鍵，為方便說明先稱作，左/中/右。想成是筆電的FN鍵就很好理解。
  * 正常情形下都在DEFAULT層。
  * 按住左鍵可以進入LOWER層。放開就回DEFAULT層。單擊一下則是ESC鍵。
  * 按住右鍵可以進入RAISE層。放開就回DEFAULT層。單擊一下則是DEL鍵。
  * 先按住左鍵即進入LOWER層，不放開，接著按右鍵，此時就是LOWER層的右鍵，這個鍵也是設為切層鍵會切到ADJUST鍵。
  * 
  * 左手鍵盤ADJUST層，由上面數來第二排都是設定成BLUE TOOTH的功能鍵。預設可以設定五組配對。
    * 由左往右
    1. Reset
    2. 清除當下這組的配對設定
    3. 切到第0組
    4. 切到第1組
    5. 切到第2組
    6. 切到第3組
    7. 切到第4組
    8. 右手
    9. 切到第4組
    10. 切到第3組
    11. 切到第2組
    12. 切到第1組
    13. 切到第0組
    14. 清除當下這組的配對設定
    15. Reset
  * 所以有時候當下的組別與電腦端無法配對時，就可以利用功能鍵清除配對設定，然後就可以重新配對了。




