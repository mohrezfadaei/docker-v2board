# Docker Lutos Network

Dockerized _Lotus Network_ application (a fork of _V2board_).

## Quick Start

1. Edit the environment variables:

    ```bash
    copy .env.sample .env
    vim .env
    ```

2. Edit the path of mysql volume in `docker-compose.yaml`.

3. Issue the following command:

    ```bash
    docker compose build
    docker compose up -d
    ```

4. Enter the container the enter configs:

    ```bash
    docker compose exec v2board bash
    ```

    ```bash
    \ \   / /___ \| __ )  ___   __ _ _ __ __| | 
     \ \ / /  __) |  _ \ / _ \ / _` | '__/ _` | 
      \ V /  / __/| |_) | (_) | (_| | | | (_| | 
       \_/  |_____|____/ \___/ \__,_|_|  \__,_| 
    
     请输入数据库地址（默认:localhost） [localhost]:
     > mysql      <- MySQL host
    
     请输入数据库名:
     > v2board    <- MySQL database name
    
     请输入数据库用户名:
     > root       <- MySQL user (recommeded: root)
    
     请输入数据库密码:
     > pa$$Word   <- MySQL user password
    
    正在导入数据库请稍等...
    数据库导入完成
    
     请输入管理员邮箱?:
     > test@sample.com    <- Admin email
    
    一切就绪
    管理员邮箱：mohrezfadaei@gmail.com
    管理员密码：2ad9a1d644b598fd31d3c66698bc0e0e
    访问 http(s)://你的站点/7afca88a 进入管理面板，你可以在用户中心修改你的密码。
    ```
