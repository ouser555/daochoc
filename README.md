# daochoc
daochoc, zmk config, nrfMicro1.4

daochoc資料夾放到 zmk/app/boards/shields/底下


執行


west build -d build/left -b nrfmicro_13 -- -DSHIELD=daochoc_left


west build -d build/right -b nrfmicro_13 -- -DSHIELD=daochoc_right


燒錄檔於


zmk/app/build/left


zmk/app/build/right

