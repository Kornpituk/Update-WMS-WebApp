# Update WMS Web App
  ### dashboard
  ### Inventory
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
    ** ปรับ ช่องเลือก ช่วงเวลาที่ จะแสดงข้อมูล เป็น years , month , week , day ,  --> `[กำลังดำเนินการ]`
