# POINTER TUTORIAL OVERVIEW

## I/ĐỊNH NGHĨA
- **`POINTER`** là kiểu dữ liệu dùng để ám chỉ địa chỉ của một biến khác  

- Nó trỏ đên địa chỉ của các biến khác ( có thể hiểu địa chỉ của biến ở đây như là CCCD vì biến đều có giá trị khác nhau )

## II/ ĐỊA CHỈ VÀ MỘT SỐ THỨ BASIC   

>``` php 
> int value = 1;
>```

| `STT` 	| `VALUE` 	| `DEFINITION`                 	| `OUTPUT EXAMPLE` 	|
|-------	|---------	|------------------------------	|------------------	|
| 1     	| &value  	| ĐỊA CHỈ CỦA BIẾN             	| 0xd5a2dffd6c     	|
| 2     	| value   	| GÍA TRỊ CỦA BIẾN             	| 1                	|
| 3     	| *&value 	| GIÁ TRỊ CỦA ĐỊA TRỊ CỦA BIẾN 	| 1                	|


## III/ DÙNG CON TRỎ
### A. KHAI BÁO CON TRỎ

>```PHP 
>int = *pointer ; 

 ___`DẤU * LÀ CÚ PHÁP KHAI BÁO`___
### B. CON TRỎ TRỎ TỚI MỘT ĐỊA CHỈ

>```PHP
>int value = 1 ;

- Lúc này :


>```PHP
> &value = 0xd5a2dffd6c`
> value = 1
> *&value = 1

* ___`TOÁN TỬ  `*` CÓ NGHĨA LÀ TRỎ TỚI GIÁ TRỊ CỦA ĐỊA CHỈ`___
* ___`ĐỊA CHỈ CỦA VALUE Ở ĐÂY LÀ `0xd5a2dffd6c`  NÊN DẤU  `*`  TRỎ TỚI GIÁ TRỊ CỦA NÓ LÀ  `1` `___

- Lúc này :


>```PHP
> pointer = &value = 0xd5a2dffd6c`
> *pointer = value = 1

* ___` `pointer`  lúc này là một con trỏ mang  `ĐỊA CHỈ`  nên  `*`  tới  `ĐỊA CHỈ`  thì nó có giá trị bằng  `1`  `___
