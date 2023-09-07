# Write-ups Flare-on 9 (2022)

## Challenge 1

Tìm flag thì thấy được `flag` được nối string như sau:

![picture 0](../../../images/cd7bc0ca2d269bcec8552c734c036977029de86ad44bca4bdbee53f64b78e7a2.png)

Tìm biến `rightGuessString` thì thấy:

![picture 1](../../../images/f2f23652e85abeacf36be18edfd45f52c635393186afe505d8d2bcd3e211271e.png)

Thấy rằng `rightGuessString` là lấy từ `WORDS[57]`, nên kiểm tra file `words.js` xem `WORDS[57]` có giá trị là gì:

![picture 2](../../../images/d87a0e435708a214b51e7f83536fb01ab5eb85c755eb85c401df7f83da19ab11.png)  


flag: `establishmentarianism@flare-on.com`

## Challenge 2

Sau khi chạy, mở trong IDA tìm được đoạn thay đổi giá trị vị trí của chuột, đoạn code bên dưới thấy giá trị vị chuột này được so sánh với hai giá trị width và height khi chia dư cho hai số const, nên cần phải debug để kiểm tra:

![picture 5](../../../images/b79c9efcc0f0ba5870f8555f1d3a9104dc0c931d20f3c8a17d02ecf4a69480e3.png)  

Debug thì thấy được được giá trị của weight và height:

![picture 3](../../../images/8ae76b99007dbcf3f1b83417eb11a067f4dd499480964dc847caff263e91f31a.png)  

Giá trị vị trí của chuột tìm được là:

![picture 6](../../../images/fabe360a017df3c9061a1a9d77a6553a18c2669ae32c45fabc89c43570933fe0.png)  

Sau khi click giá trị trên, kết quả thu được:

![picture 4](../../../images/07d3eb597e66315050011eea61ea7b821c1217e198864417d5325799fdd2be92.png)  

flag: `w1nN3r_W!NneR_cHick3n_d1nNer@flare-on.com`
