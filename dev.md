# mmkdir Homework1

	==> mkdir เป็นคำสั่งที่ใช้ในการสร้าง directory ใหม่ใน directory ปัจจุบัน
	==> ในข้อนี้จะสร้าง directory ใหม่ที่ชื่อว่า Homework1
# cd Homework1
	==> cd เป็นคำสั่งที่ใช้ในการย้าย  directory
	==> ในข้อนี้จะย้ายไปยัง directory ที่ชื่อ Homework1
# echo "# Homework1" >> README.md
	==> echo เป็นคำสั่งที่ใช้ในการแสดงผล
	==> ในข้อนี้จะแสดงข้อความ # Homework1 ในไฟล์ README.md 
# git init
	==> คำสั่ง git init เอาไว้เพื่อสร้าง git repository เปล่าๆขึ้นมา โดย Git จะทำการสร้างโฟลเดอร์  .git ขึ้นมาภายในโปรเจ็คของเรา (Hidden ไว้อยู่)
# git add README.md
	==> git add เป็นคำสั่งที่ใช้ในการติดตามการเปลี่ยนแปลงของไฟล์
	==> ในข้อนี้จะติดตามการเปลี่ยนแปลงของไฟล์ README.md 
# git status
	==> ในการตรวจสอบสถานะ
# git config --global user.email "....your email...."
	==> เป็นคำสั่งที่ใช้ในการกำหนดอีเมลล์ผู้ใช้
# git config --global user.name "....username...."
	==> เป็นคำสั่งที่ใช้ในการกำหนดชื่อผู้ใช้
# git commit -m "first commit"
	==> git commit -m เป็นคำสั่งที่ใช้ในการยืนยันบันทึก การเปลี่ยนแปลง ต่างๆที่เกิดขึ้นโดยจะมีการอธิบายการเปลี่ยนแปลงไว้ใน double quote
	==> ในข้อนี้จะบันทึกการเปลี่ยนแปลงและอธิบายการเปลี่ยนแปลงว่าเป็น first commit
# git remote add origin https://github.com/Montira009/Homework1.git
	==> เมื่อยังไม่มี remote repository ให้เพิ่มเข้าไปโดยบอกที่อยู่ url ของ repository
# git remote -v
	==> แสดง remote repository 
# git push -u origin master
	==> เป็นคำสั่งที่ใช้ในการส่งโค๊ดจากเครื่อง local ไปที่ Github

---------------------------------------------------------------------------------------------------------

New Commands
# File Undo
	$ git checkout test.txt
# การ undo ไฟล์ โดยที่ไฟล์นั้น ได้ add ไปแล้ว > จะได้สถานะ untrack
	$ git reset HEAD test.txt
# การยกเลิกการ Commit
	$ git reset --soft "HEAD^"  
# การดูรายละเอียด
	$ git log --oneline
# Delete file, After committed
	$ git rm test.txt
# Recovery
	$ git reset HEAD test.txt
	$ git checkout test.txt
# Hide your Update
	$ git add file
	$ git stash    
	$ git pull 
	$ git stash pop  #recovery data 
	$ git add > commit > push
# Branch
	$ git branch yourbranch 		// Create Branch
	$ git checkour yourbranch		//Move to branch yourbranch
	$ git checkout -b yourbranch 		//Create branch and move to new branch
	$ git branch -a 			// Status branch
	$ git branch -d yourbranch 		//Delete branch | Move to master first.
	$ git push -u origin yourbranch	

# -- Upload branch to master -- 
	$ git checkout master
	$ git merge --no-ff dev 		// merge dev to master | --no-ff 