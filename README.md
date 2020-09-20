# 在docker建立mysql server

# Step

1. 安裝 docker, docker-compose

2. 將`docker-compose.yml.default` 檔名改成 `docker-compose.yml`

3. 編輯 `docker-compose.yml`，選擇`image`(postgresql映像檔以及版本)，定義`port`, `user`, `password`, `root password`

4. 開命令列並在該目錄下執行 `docker-compose up -d`
  - 執行 `docker ps` 看看有沒有開啟成功，這裡可以看到container id
  - 執行 `docker exec -it <container_id | container_name> /bin/bash` 即可進入該container的bash

6. 開啟資料庫UI，連上
host:127.0.0.1
port: 5432 (看你`docker-compose.yml`怎麼編輯的)
