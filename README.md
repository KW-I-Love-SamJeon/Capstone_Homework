# ๐ค์ฐํํ๋ ฅSWํ๋ก์ ํธ Homework๐ฌ

---
**Contributors**
> ๐ฑโ๐ป[syw2045](http://github.com/syw2045)  
> ๐ป[KiKi-Daehaksaeng](https://github.com/KiKi-Daehaksaeng)  
> ๐ฑ[6Whistle](https://github.com/6Whistle)  
> โพ[dlwnsgud8406](https://github.com/dlwnsgud8406)  
> ๐[angrymusic](https://github.com/angrymusic)  

---
**Purpose**
- ํ๋ก์ ํธ๋ฅผ ์งํํ๊ธฐ ์์ ํ๋ก์ ํธ์ ๋ํด ํ์ํ ์ง์์ ์ดํดํจ๊ณผ ๋์์ ์์ฉ ๋ฐ ์ ์ฉํ๋ ๋ฐฉ๋ฒ์ ์ตํ๊ธฐ ์ํด ๊ณผ์ ๋ฅผ ์ํํจ.

---
# ๐๊ณผ์  ๋ชฉ๋ก
1. Rotation
2. Normal vector
3. Canny edge detection

## 1. Roatation
![img_1](./img/Rotation.png)

`Euler Angle`์ ์ด์ฉํ์ฌ `3D Object`๋ฅผ ํ์ ํ๋ ๊ณผ์ 

## 2. Normal vector
![img_2](./img/Normal_vector.png)

`vertex`์ `edge` ๋ฐฐ์ด์ ์ ์ฅํ๊ณ  ๊ณต์์ ํตํด ๊ฐ `edge`์ `normal vector`๋ฅผ ์ถ๋ ฅํ๋ ๊ณผ์ 

## 3. Canny edge detection
![img_3](./img/Canny_edge_detection.png)

`OpenCv api`๋ฅผ ์ฌ์ฉํ์ง ์๊ณ , `Canny edge detection`์ ๊ตฌํํ๋ ๊ณผ์ 

### ๊ตฌํ ๋ฐฉ์
1. `Gaussian Filter`๋ฅผ ํตํด ๋ธ์ด์ฆ ์ ๊ฑฐ
2. `Sobel filter`๋ฅผ ํตํด `gradient`์ `theta` ํ๋
3. `gradient`์ `theta`๋ฅผ ๋ฐํ์ผ๋ก `Non-max suppression`์ ํตํด ์ ๋ถ์ ๋ฐฉํฅ์ ํ์ธํ์ฌ ๊ตต๊ธฐ ์กฐ์ 
4. 2๊ฐ์ `threshold`๋ฅผ ์ฌ์ฉํ์ฌ ์ ๋ถ์ ๊ฐ๋ ์ ๋ณ
5. `Hysteresis`๋ฅผ ํตํด ๊ฐํ ์ ๋ถ๊ณผ ์ฝํ ์ ๋ถ์ ์ฐ๊ด ๊ด๊ณ๋ฅผ ํ์ธํ์ฌ ๋ธ์ด์ฆ ์ ๊ฑฐ
