# RegressionMiniProject
## กลุ่มสมาชิก หมู่ 200 (Members Section 200)
1. นาย ศิวกร ภาสว่าง 6410451423 ( หัวหน้ากลุ่ม )
2. นาย นิสิต นะมิตร 6410451148
3. นาย พีรสิษฐ์ พลอยอร่าม 6410451237

## เกี่ยวกับชุดข้อมูลตัวอย่าง (About Apples Dataset)
ชุดข้อมูลตัวอย่างที่ได้เป็น**ปริมาณของแอปเปิ้ลในแต่ละวันที่มี 3 สายพันธุ์**โดยมีการเก็บคอลัมน์ดังนี้
- วันที่เก็บแอปเปิ้ล ( Date )
- ปริมาณของแอปเปิ้ลสายพันธุ์ Envi ( Number of Envi apples)
- ปริมาณของแอปเปิ้ลสายพันธุ์ Fuji ( Number of Fuji apples )
- ปริมาณของแอปเปิ้ลสายพันธุ์ Gala ( Number of Gala apples )
- ภูมิภาค/ประเทศ ( Region )  

ในกาทดลองนี้ผู้ทดลองได้เลือกชุดข้อมูลตัวอย่างของประเทศอังกฤษในการสร้างโมเดลด้วย AI Algorithm (Pefer apple dataset in UK for making models)

## การสร้างโมเดลด้วย AI Algorithm (How to make model by AI Algorithm)
ผู้ทดลองได้เลือก AI Algorithm มา 3 วิธีการได้แก่ (Using 3 Algorithm)
- BaseLine Algorithm
- Linear Regression Algorithm
- Gradient Boosting Regression Algorithm

## การวัดหาค่าประสิทธิภาพของแต่ละโมเดล (Using Performances)
- Mean Absolute Error : MAE ( ใช้ค่าดังกล่าวเป็นหลักเนื่องจากชุดข้อมูลตัวอย่างมีค่าที่ต่างกันมาก )
- Mean Square Error : MSE
- Mean Absolute Percentage Error : MAPE
- R2 Score

## โครงสร้างของไฟล์ (File Structure)
 RegressionMiniProject (เก็บข้อมูลเกี่ยวกับ project)
  - DataSet (เก็บข้อมูลไฟล์แอปเปิ้ลและจำแนกสายพันธุ์ | store information about kinds of apples in Dataset)
     - Envi ( แฟ้มที่เก็บการสร้างชุดข้อมูลตัวอย่างของ Envi )
     - Fuji ( แฟ้มที่เก็บการสร้างชุดข้อมูลตัวอย่างของ Fuji )
     - Gala ( แฟ้มที่เก็บการสร้างชุดข้อมูลตัวอย่างของ Gala )
  - algorithm
      - Envi ( แฟ้มที่เก็บโมเดลแต่ละชุดข้อมูลตัวอย่างของ Envi และสรุปผลของค่าประสิทธิภาพทั้งหมด )
          - 1_predict_1 ( แฟ้มที่เก็บโมเดลและค่าประสิทธิภาพจากการใช้ทำนายวันถัดไปโดยใช้วันก่อนหน้า )
          - sequence_predict_1 ( แฟ้มที่เก็บโมเดลและค่าประสิทธิภาพจากการใช้ทำนายวันถัดไปโดยใช้วันก่อนหน้า 5 วันเรียงกัน )
      - Fuji ( แฟ้มที่เก็บโมเดลแต่ละชุดข้อมูลตัวอย่างของ Fuji และสรุปผลของค่าประสิทธิภาพทั้งหมด )
          - 1_predict_1
          - sequence_predict_1
      - Gala ( แฟ้มที่เก็บโมเดลแต่ละชุดข้อมูลตัวอย่างของ Gala และสรุปผลของค่าประสิทธิภาพทั้งหมด )
          - 1_predict_1
          - sequence_predict_1
