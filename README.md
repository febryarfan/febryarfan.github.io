## Basic Test : 10

<p align="left">
  1. What are the project models used in SDLC? Which model do you think is best and why?, Explain that model <br>
  2. Find more than 2 bugs and make a bug report in trello https://www.saucedemo.com, with the username "standard_user", invite us on trello or bug report that you make by email: faris.ardi@roomme.space
  
  **Answer :
  
 1. Menurut saya, Model SDLC yang paling baik dan efektif adalah Spiral Model. Karena pada Spiral Model proses pembuatan sebuah software atau prototype sangat jelas dan terencana dengan beberapa tahapan yang sistematis. di tahap awal (Liason) model ini ada pihak user dan pihak-pihak yang melakukan pengembangan software terlibat yang mempermudah tim dalam memperbaiki dan mengembangan software sesuai kebutuhan dan keinginan hingga memuaskan pelanggan. kemudian tahap planning memudahkan tim dalam membuat estimasi biaya yang harus dikeluarkan. lalu ada juga tahapan analisis resiko untuk mengidentifikasi resiko yang berpotensi akan terjadi dan menghasilkan solusi alternatif yang dapat dijalankan. Adapula tahapan engineering yang mana ada pengujian pada aplikasi dan membuat dokumentasi terhadap aplikasi yang diuji, di sini dapat terlihat apakah beberapa case yang di uji sudah sesuai dengan apa yang diinginkan oleh user atau belum, dan dapat melihat apakah masih ada bug atau error pada aplikasi yang diuji.
2.
2.1 ![Screenshot (11)](https://user-images.githubusercontent.com/84786558/119529113-002e7000-bdac-11eb-921c-813abd15ba23.png)

Pada Screenshot 2.1 di atas, Ketika user masuk ke menu "Your Cart" tanpa adanya item yang di order / beli dan kemudian user menekan tombol Checkout, seharusnya user tidak bisa lanjut ke tahap selanjutnya. Lebih baik pada aplikasi tersebut ditambahkan notifikasi "Please add item to cart"

2.2 
  
<img width="951" alt="Screenshot (17)" src="https://user-images.githubusercontent.com/84786558/119531739-6ddb9b80-bdae-11eb-8d42-fe6ba40cecee.png">
<img width="943" alt="Screenshot (18)" src="https://user-images.githubusercontent.com/84786558/119531808-7df37b00-bdae-11eb-85e0-270d2422ec95.png">
  
![Screenshot (20)](https://user-images.githubusercontent.com/84786558/119531821-81870200-bdae-11eb-9c14-8e7035f48b86.png)

Perhatikan urutan gambar 2.2 dari atas ke bawah, jadi setelah user melakukan memesan 4 item akan muncul 4 item pada cart. Kemudian user remove 1 item yang menjadi item di cart menjadi 3 item. Selanjutnya user klik tombol icon cart seperti gambar 2, item pada cart akan berkurang menjadi 2 item namun dengan kondisi gambar pada icon cart masih berjumlah 3. 
  
</p>

## Logic Test : 10


<p align="left">
  Show data with parameters such as : <br>
  Show data with parameters such as with postman : <br>
  - Name      : Pres. Aasa Malik<br>
  - Status    : Active<br>
  - Gender    : Female
  
  and create a validating schema for that result ??


**Answer : 
  
{"code":200,"meta":{"pagination":{"total":1600,"pages":80,"page":2,"limit":20}},"data":[{"id":34,"name":"Pres. Aasa Malik","email":"aasamalik@gmail.com","gender":"Female","status":"Active","created_at":"2021-05-25T04:50:03.837+05:30","updated_at":"2021-05-25T04:50:04.378+05:30"}]}

</p>


## Query Test : 20
<p align="left">
  Write database query for below based on the table shown <br>
  <img src="https://ngomah.com/wp-content/uploads/2021/05/test-query.jpg"/><br>
  1. Display all detail in table “order” from low price to high price<br>
  2. Display the cust_name who purchased the prod_id A101 and A103<br>
  3. Display All detail in table Product purchased by Budi
  
  **Answer:
  
(Nomor 1)
  
SELECT *
  
from Order
  
order by amount ASC
  
  
  
  
(Nomor 2)
  
SELECT Customer.cust_name
  
from Customer
  
inner join Order on Customer.id = Order.cust_id
  
inner join Product on Order.prod_id = Product.id
  
where Product.id = ' A101' or 'A103'   
  
  
  
</p>
