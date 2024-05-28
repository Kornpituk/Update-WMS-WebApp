# Update WMS Web App
  ### General
  ### Stock Update
  ### dashboard
  ### Stock Update
  ### Product List
  ### Import Data
  ### Set Permission
  ### Setting

## Version 1.0
### :watch: `03-05-2024`
### dashboard
  * delivery —> date picker  - start to End  - | Search | Exit |
  * po date —> date picker - start to End
  * received date —> date picker - start to End
  * status --> select Box
  * Location --> select box
  * ปรับหน้า Received PO  complete
  * Status Update
  * Filter Update
  * Details Image Update
  * Label Back Update --> History
  * ปรับหน้า Received PO  --> Start

## Version 1.1
### :watch: `04-05-2024`

### General
  * Search filter อันใหม่ ปรับแก้ให้มีขนาดเล็กลง เอา label ออก
  * กด โลโก แล้ว กลับมายังหน้า dashbord
  * Login แล้วเข้าหน้า dashbord  
### Inventory
  * แก้หน้า Search หน้าแรก  เอา UoM ออก ใส่  serial search เข้าไปแทน ---> ค้นหา อันเดียวได้ข้อมูลหน้าสามเลย

## Version 1.2
### :watch: `06-05-2024 & 07-05-2024`

### dashboard
  - Min Max
    - กดข้างหน้าได้ว่าจะเข้าสู้ Max / Min
    - แล้วข้างในสามารถ กดเลือกได้อีกที
    - ทำหัวข้อเป็น Stock Min & Max กด tabs
    - เอาข้อมูลใส่แค่ Min / Max อย่างเดียว
    - เอาปุ่มด้านบน ขาวออก เหลือแต่ ด้านล่าง
    - เอาสีออก
  - Top Move
    - กดเลือกจาก กราฟ
    - เลือกเวลลา Day,Week, Month, Custom เลือกช่วงเวลาได้ Lock วันที่ด้วย
    - เปลี่ยนบาแท่ง สี ให้แยกซัดเจน
    - เอา status ออก ใส่จำนวน แทน
    - ช่วงเวลา ที่งานเอามาเยอะ กราฟแท่ง ในแต่ช่วงเวลา --> รวมคนแล้ว
    - Timing ของ คน ในแต่ล่ะช่วงเวลา
    - To Day ว่า รอรับเข้ามันเยอะขนาดไหน  สินค้ารับเข้าเข้ามาเยอะขนาดไหน
    - แยก Picking , Received

## Version 1.3
### :watch: `08-05-2024`

### dashboard
  - ปรับ ขนาดตัวหนังสือ ให้เท่ากัน ตรง หัวข้อ ให้เท่ากับ ตรง navi
  - Font familir ให้เป็นแบบเดียวกัน
  - Label ของ chart donut 4
  - เพิ่ม version Web WMS APP ลง Fotter
  - Top Move & non Move
    - ปรับ Responsive
  - Performance
    - เอา ชื่อประเภท Received / Picking ขึ้นมาใส่ ตรงกับ icon
    - color สามารถ hover ได้ทั้ง แทบล่าง หัวข้อ icon
    - Card กด เอา ชื่อประเภทมาใส่แทน dddd และทำให้มัน hover ได้ เพิ่ม คำว่า details position end
    - เอา CardAction ออก
    - Create Mock Data ให้ ทั้ง Received & Picking
      - Mock Data Category จะเป็น ข้อมูล ที่ สำเร็จแล้วทั้งหมด ของ Received [ PO, Transfer In,
      - Other ] / Received [ Transfer Out, Delivery, White Off ]
      - Mock  Data Item จะเป็นการนำข้อมูล  Mock Data Category มาหาค่าเฉลี่ยน
  - ปรับ ช่องเลือก ช่วงเวลาที่ จะแสดงข้อมูล เป็น years , month , week , day ,  --> `[กำลังดำเนินการ]`

## Version 1.3.1
### :watch: `09-05-2024`

### dashboard
  - Performance
    - เอาสเลกแต่ล่ะ bar ออกให้เหลือแค่อันเดียว ไม่เกิน 100
    - เปลี่ยนคำว่า category --> transection
    - Scale Y ทำให้เปลี่ยน ตามการเลือกช่วงเวลา
    - Label ทำให้เปลี่ยน ตามการเลือกช่วงเวลา
    - มี Label แสดง ค่าสูงศุดในแต่ล่ะประเภท
    - ทำ MockData ให้ สามารถแสดงข้อมูลตาม ช่วงเวลา ได้
        - ปรับ การแสดงข้อมูล ให้แสดง ข้อมูลที่ต้องใช้ก่อน และใช้หลัง
    - เปลี่ยน ปุ่มกดเลือก ช่วงเวลาให้ แสดง Icon กับ ข้อความ
   
## Version 1.3.2
### :watch: `10-05-2024`

### dashboard
  - ทำปุ่ม กดเลือกช่วงเวลาของข้อมูล
    - าเลือกวัน day วันที่ปัจจุบันจะเป็นค่าดั้งเดิม 

### Stock Update
  - ตั้งค่า config เรื่อง RFID Tag Non Tag
  - ตั้งค่า config เรื่อง Digit 
  - ตั้งค่า ให้ ตาราง ข้อมูลมีขนาดเท่ากัน

### Performance 
  - Chart Label ใช้ แบ UpperCase ทั้งมหด
  - เมื่อกดเข้ามาแล้วให้ขึ้นข้อมูลช่วงเวลา today เลย
  - เปลี่ยน คำตรง ช่วงเวลาให้เป็น Daily, Weekly, Monthly, Yearly
  - เอาคำสั่ง
    ```script
      chartDataAll.value = mockDataFunction(8).dataReceived
    ```
    มาไว้ข้างนอก watch เราไม่อย่างงั้นมันจะเป็น ค่า default ทูกครั้ง
  - Received ---> details
    - เปลี่ยน คำว่า fileter --> Search
  - Transfer In ---> details
    - เปลี่ยน คำว่า fileter --> Search
  - Other   ---> details
    - เปลี่ยน คำว่า fileter --> Search
  - Transfer Out ---> details
    - เปลี่ยน คำว่า fileter --> Search
  - Delivery  ---> details
    - เปลี่ยน คำว่า fileter --> Search
  - Write Off  ---> details
    - เปลี่ยน คำว่า fileter --> Search
      
  - Move / Non Move
    - ชื่อ Category กับ Item ใช้ชื่อเดียวกัน
    - ข้อมูล mock data เว้นช่องว่าที่ชื่อ product
   
## Version 1.3.3
### :watch: `13-05-2024`

### Genaeral 
  - เปลี่ยนคำตรงที่ แสดง ทศนิยม มันสลับกัน 
  - หัวคอมลัมตารางข้อมูล NO -> No. 

### Dashboard
  - ตอนช่องเวลาให้กดที่ ช่องเลยไม่ต้องมีปุ่น
  - WaraHouse Select --> ทำ function ให้แสดงค่าตามจริง
  - Date Select
    - ทำ  function สามารถเลือกเวลาได้ ทั้ง day,week Month หรือ range
  
### Inventory
  - Product Code --> เปลี่ยน c-> C
  - เพิ่ม column Serial --> Mock Data
  - เพิ่ม margin ของ ช่อง tag,non tag, serail

### Performance
  - Day -> Daily
  - ตัด Years ออก เรียงใหม่เป็น daily -> Weekly -> Monthly
  - Received – PO

## Version 1.3.4
### :watch: `14-05-2024`

### Genaeral 
  - เปลี่ยน คำว่า category --> categories 
  - Setting Side bar เมื่อเปลี่ยนการแสงดผลของตัวเลข แบบบมีทศนิยมกับไม่มีเมื่อกดแล้วสามารถ รีเฟรซหน้าเว็บได้อัตโนมัติ
  - Thememizer
    - Digit ปรับเป็นเมื่อradio -> Yes = Show Digit , No = Don’t' Show Digit
    - Theme color --> ลบ Radio Label ออก เข้าเป็น label check แทน
  - Setting Config
    - ปรับให้ checkbox Show Digit ลิ้งค์กับ Theme Customizer Digit
    - ปรับเมื่อกับ radio คือ check (True) = Show , check (False) = Don't Show
    - ปรับคำให้เหมือนกัน 

### Dashboard
  - Warahouse Select --> สามารถเลือก คลังได้แล้ว เมื่อเลือกแล้วกด aaply คลังหลักภายใน เว็บจะเป็นคลังนั้นๆ 
  - Card ของ Expiry Date, Stock Min Max ไม่ได้ลบ CardTitle เลยทำให้ CardText โดนลงมา เลยทำให้ดูไม่เท่ากับ Product Data, Performance --> ปรับให้เท่ากันแล้วโดนเอา CardTitle  ออกProduct Data --> ต่อเข้ากับ ข้อมูล จาก API แล้ว (เฉพาะข้อมูล summary)
    - เปลี่ยนสี หลัง ของ Product Data เป็น color Primary 
  - Expiry Date -->  ต่อเข้ากับ ข้อมูล จาก API แล้ว (เฉพาะข้อมูล summary) 
  - Stock Min Max -->  ต่อเข้ากับ ข้อมูล จาก API แล้ว (เฉพาะข้อมูล summary)
    - ตรงช่อง Product ของ ค่า max ใส่ค่า Padding ผิด มากไปจาก Padding ของ min ไป 1 px แก้กับให้มี ค่า padding เท่ากัน คือ 16 px
  - Performance
    - เปลี่ยนสี หลัง ของ Product Data เป็น color Amber 
  - Move / Non Move
    - Add Categories Product --> เพิ่มระยะห่างระหว่าง titel Categorise กับ Iocn
      - Bug!! --> เมื่อเลือก ไปคอนแล้วกดเลือกอีกรอบ ชื่อจะซ้อน --> แก้แล้ว โดยเปลี่ยน จาก Autocomplete  -> Select เหตุผลน่าจะมาจาก ที่ Autocomplete   เอาไว้เลือก item ทีละหลายๆ items แต่ เราต้องการเลือกแค่อันเดียว  Select  จึงเหมาะกว่า 
  
### Inventory
  - เอา Serial ออก เพราะหลังจากการประชุม ได้ข้อสรุปว่า ณ ตอนนี้เรายังเอามาแสดงตรง หน้าแรก หรือ ค้นหาจากหน้าแรกได้ --> เอา Unit กลับมาเหมือนเดิม
  - 

## Version 1.3.5
### :watch: `15/16-05-2024`
 
### Dashboard
  - Stock Min Max
    - ให้ สามารถกดดู รูปได้
    - ต่อกับ api แล้ว แต่แสดงได้แค่ ข้อมูล ยังไม่สามารถใช้งาน search filter อื่นๆ ได้
    - Formate Date ให้เป็นรูปแบบ วว/ดด/ปปปป
  - Performance
    - เปลี่ยนสี หลัง ของ Product Data เป็น color Amber
  - Expiry Date
    - ต่อกับ api แล้ว แต่แสดงได้แค่ ข้อมูล ยังไม่สามารถใช้งาน search filter อื่นๆ ได้
    - เพิ่มคอลัม Status
    - เมื่อกดรูปแสดงรายละเอียด และแยกสีตาม status
    - เอาคอลัม แสดงจำนวนที่ alert ออก
    - Formate Date ให้เป็นรูปแบบ วว/ดด/ปปปป
    - ใส่ foramte ```.toLocaleString('en-US') ```
      - Total QTY
  - Stock Update
    - หน้า lot เอา Remark มาไว้ด้านล่าง

## Version 1.3.7
### :watch: `20-05-2024`

### Dashboard
  - Expiry Date
    - สมารถ ใช้ Filter, search, sort, ได้แล้ว
    - ปรับสีตรง หัวตาราง status เป็นแบบเลือกว่าจะ search อันไหน
    - Search Status เปลี่ยนสีตามที่เลือกค้นหา
    - Formart Total ตรง dialog Card 
  - Min /Max
    - สมารถ ใช้ Filter, search, sort, ได้แล้ว
    - ต่อกับ api สมารถ ใช้ Filter, search, sort, ได้แล้ว
  - Date Data
    - ปรับวันที่ ให้เป็น วว/ดด/ปปปป จากเดิม ที่เป็น ดด/วว/ปปปป
### Inventory
  - View ---> ปรับให้ช่องค้นหา ตรงหัว คอลัม ปุ่ม Cancel. Reset มีขนาดความกว้าง 100%
  - Lot ---> ปรับให้ช่องค้นหา ตรงหัว คอลัม ปุ่ม Cancel. Reset มีขนาดความกว้าง 100%
    - Format Total กับ Non-Tag ให้สามารถ เลือก แสดง ทศนิยมได้ 
### General
  - แก้คำผิกจาก EaseTrack --> Easetrack 
### Set Permission
### Setting


## Version 1.3.8
### :watch: `21-05-2024`

### General
  - Details ของรูป ทุกหน้าให้เหมือนกัน
  - ปรับ table แสดงข้อมูล โดย การใช้สูตรคำนวณ เลขลำดับใหม่ จากเดิม `index+1`
  - Setting Config
    - เอา conifg batch Received ออก  เพราะยังไม่ได้ใช้งาน
  - Search Column ทำให้ ปุ่ม Reset cacel เท่ากันทุกหน้า และมี ขนาด 100 %
  - Filter ทุกหน้าเพิ่มปุ่ม Clear เอาไว้ ล้างค่าที่ค้นหาไปแล้ว
  - เลข index ของ ตาราง ทุกหน้า จะมี ตั้งแต่ 1- N โดย N คือจำนวนสุดท้ายของจำนวนข้อมู,ที่จะแสดง จากเดิมที่ มีปแค่ 1-10
### Stock Update
  - แก้บัค `.toLocaleString('en-US')` ให้สามารถใช้งานได้ ที่ติดเพราะ ถ้าค่าที่จะใช้ไม่มี ไม่สามารถใช้งานได้ เลยต้อง ใช้ v-if ช่วยเซ็คค่า
  - ทำให้ตัวหนังสือ ของค่า categories เท่ากับ ค่าอื่นๆ
### Dashboard
  - Expiry Date
    - สมารถ ใช้ Filter, search, sort, ได้แล้ว 
    - ตรงข่อง status ทำให้ listItem เท่ากัน 
  - Min /Max
    - แก้บัค ที่ Search Column ให้กลับมา ค้นหาได้แล้ว 
### Dashboard
  - ต่อ Features ค้นหาเข้ากับ api  ตอนนี้ใช้ได้ เกือบทุกอย่าง  ``** ยกเว้น Categories, Group, Sub Gounp**``
  - Features  Action ท้ายตารางยังใช้งานไม่ได้
  - ปริ้น --> ใช้งานไม่ได้
  - Create  --> ใช้งานไม่ได้
    - ต้องทำ UI ใหม่
   
## Version 1.3.9
### :watch: `23-05-2024`

### dashboard
  - Product Data ----> Stock Update
  - Min -> minimum / Max -> maximumExpiry Date
    - เหลือวันน้อยๆอยู่บนสุด
    - Status เอา Reset&Cancel ออก ให้เหลือแค่ Expired
    - เอา Alert ออก คำว่า Expired เป็นสีแดง
    - Expiry Date (ตารางข้างบน) —> Expired 
### Stock Update
  - Remark เซ็ค
### Product List
  - แก้ไขคำผิดนิดหน่อย
  - สามารถปริ้น Barcode, QRCode  ได้แล้ว
  - Action
    - Edite --> ยังไม่ได้ทำ
    - Print --> ใช้ได้แล้ว
    - Delete  --> ยังไม่ได้ทำ 


## Version 1.3.10
### :watch: `24-05-2024`

### Inventory  --> เพิ่มเมนูใหม่สำหรับ การแสดงข้อมูล serial ทั้งหมด 
  - Total Details  --> ทำ UI และทำการ Mock ข้อมูล
  - Total Summary  --> ทำ UI และทำการ Mock ข้อมูล 

### Product List
  - ทำการต่อ UI Create เสร็จแล้ว
  - ทำ funtion Delete

## Version 1.3.11
### :watch: `27-05-2024`

### Dashboard
  - Font size ปรับให้ขนาด 16px
    - Warehouse select, Date select
### Categories, Sub, Sec , color, UoM, Size
  -  Label หน้า และ search create ใหม่
### Product List
  - Api ``การอัพโหลด / แก้ไข้สินค้า สามารถทำให้ไม่ต้องใส่รูปได้ไหม ปล่อยเป็นค่าว่าง ไม่ต้องส่ง ``
  - Product List
    - ต้องการค่า Model, Size, Style, Weight, Unit, Wide, Long, Hight, Uint
    - Expired Date, Alert, Details
  - Alert
    - เปลี่ยน คำว่า "Close" --> "( X )"
    - Multible --> ลบออก
  - Create
    - แก้บัค การอัพโหลดรูปโดย ทีแรก เราต้องกด ลบรูปก่อนที่จะทำหารอัพโหลดรูป แต่ตอนนี้สามารถกดอัพโหลดรูปได้เลย
    - เปลี่ยน ตำแหน่งของปุ่ม ลบรูป ให้มาอยู่ด้าน ขวาสุด และทำให้เป็นปุ่มมากขึ้นจากที่ เป็นแค่ไอคอน
  - Edit
    - สามารถเลือกสินค้าที่หน้า list  เพื่อไปยังหน้า edit ได้  ***แต่ ติดบัค ถ้าเราไม่อัพโหลดรูปใหม่จะไม่สามารถแก้ไขข้อมลสินค้าได้
   
## Version 1.3.12
### :watch: `27-05-2024`

### General
  - ทำการเปลี่ยนแปลงรูปแบบ barcode จากเดิมที่ แสดงเป็นตัวเลขทำให้เป็น แทบ บาร์โค้ดแทน  --> ในอนาคตจะทำให้สามานถ กดดู ขนาดใหญ่ได้
  - แก้ไขขนาดตัวหนังสือของปุ่ม  ให้มีขนาด 16 px
  - Icon ปุ่มกด ให้มีขนาด 30 px

### Configuration
  - #### Product List 
    - Create
      - รูปสามารถกดดูได้แบบใหญ่
    - Edit
      - รูปสามารถกดดูได้แบบใหญ่
  - #### Categories, Sub, Sec , color, UoM, Size
    - แก้ไขคำผิด Product second/Sub Categories --> Group , Sub Group
    - แก้ไข รูปแบบ Label Page
      - เอา search กับ Add มาคนล่ะบันทัดกับ Label Page 
