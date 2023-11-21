# config git
git config --global user.name "..."
git config --global user.email ".."
# Khởi tạo repository ở local (máy tính)
git init -b main
# Kiểm tra thay đổi code 
git status
# Đưa code thay đổi vào stage changes để chuẩn bị đưa lên remote repository 
git add <tên file>
git add . (Đưa toàn bộ file đang thay đổi vào stage change, ngoại trừ vừa vào mới vào stage change)
git add -A (Đưa những file đã thay đổi vào stage change)
# add commit
git commit -m "nội dung commit"
(chạy git add trước khi commit)
# Connect local repo to remote repo
git remote add origin https://github.com/khoatd2828/demoBC63.git
# push code từ local repo lên remote repo
git push -u origin main (chạy lệnh git commit trước)

git push

git reset . => đưa toàn bộ file đang ở stage change => change
git reset <tên file> => chỉ đưa file ở staged change => change
# git checkout <tên file> => đưa file về trạng thái ban đầu
# git checkout . => đưa tất cả file về trạng thái ban đầu
# xem lịch sử commit :
git log 
git log --oneline
=> để exit: q
# branch
git branch => liệt kê branch đang có

git branch <tên branch> => tạo 1 branch mới

git switch <tên brand> => chuyển qua branch <tên branch>

git checkout -b <tên branch> => tạo 1 branch mới và nhảy qua branch đó

git branch -m <tên branch mới> => đổi tên branch

git branch -D <tên branch> => đứng ở branch khác mới xóa được