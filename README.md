<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# laravel-satoshi
laravel10-docker-compose

# สิ่งที่มีให้สำหรับการใช้งานเบื้องต้น
- Laravel v10
- PHP v8.2+
- MySQL v8.1
- MariaDB v10.11
- phpMyAdmin v5.2.1
- Mailpit v1.8.4
- Node.js v18.17.1
- NPM v10.1.0
- Yarn v1.22.19
- Vite v4.4.9

# ติดตั้ง docker ด้วยนะคลิกที่ลิงค์ด้านล่างนี้เลย
- Stable version of [Docker](https://docs.docker.com/engine/install/)

# การ Deploy

### สำหรับเริ่มต้นใช้งานครั้งแรก
- `docker compose up -d`
- `docker compose exec php bash`
- `composer setup`

### สำหรับครั้งต่อไป
- `docker compose up -d`
- `docker compose exec php bash`

# การใช้งาน

###  รันโปรเจค 
- URL: http://localhost

### เข้าฐานข้อมูล phpMyAdmin
- URL: http://localhost:8080
- Username: `root`
- Password: `root`
- Database: `satoshi`

### คำสั่งการใช้งาน docker พื้นฐาน
- Build 
    - `docker compose build`
- สร้างและเริ่ม containers
    - `docker compose up -d`
- ดูสถานะการทำงานของ services
    - `docker compose ps`
- สั่งหยุดหรือลบ containers, networks
    - `docker compose down`
- หยุดบริการทั้งหมด
    - `docker compose stop`
- Restart containers 
    - `docker compose restart`
- สำหรับ Run คำสั่ง command ใน container
    - `docker compose exec [container] [command]`

