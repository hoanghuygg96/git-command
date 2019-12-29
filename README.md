# git-command
git command basic

*****************************************************************************************************************
//Lần đầu tiên config cho nó
git config --global user.name "name"
git config -- global user.emai "abc@gmail.com"

//sử dụng duy nhất lần đầu tiên khi clone source từ server về máy tính
git clone <đường dẫn thư mục git trên github>

//Kiểm tra trạng thái xem có sự thay đổi gì hay không
git status

//add tất cả các file mà có sự thay đổi có màu đỏ
git add .
//Sau khi add xong những file thay đổi có màu xanh.
//Code chuyển qua vùng Staging Area

//commit code
git commit -m "Upload source code"
//Sau khi commit code chuyển qua phân vùng Local Repository

//Đẩy code tại máy tính của mình lên server
git push origin master <nhánh> => nhập user & password

//Tạo Branch
git branch <ten branch>

//Kiểm tra branch
git branch

//kéo code mới nhất về
git pull

//merge code lai voi nhau
git merge

***************************************************************************************************************
git log : xem lich su commit

git show <commit-id> : xem chi tiet lich su cua mot commit

git diff : check sự khác nhau của file modifed

định nghĩa staging area : la ~ file modefied màu xanh
định nghĩa git repository: la ~ fỉle màu xanh sau khi commit

git restore / git checkout <ten file> : restore file khi con dang ở working directory
git reset HEAD <ten-file> : bo file ra khỏi staging area // có thể không cần HEAD

git checkout -b <ten-branch> : tạo nhánh mới và nhảy vào nhánh đó làm việc
git checkout <ten-branch> : checkout branch đó

git branch : kiem tra xem co bao nhieu branch va dang o branch nao

muốn merge B vào A
git checkout A
git merge B

git branch -D <ten-branch> : delete branch

git reset --soft <commit-id> : uncommit sau commit-id được chỉ định, file sau commit-id ở staging area
git reset --mixed <commit-id> : uncommit sau commit-id được chỉ định, file sau commit-id ở work directory
git reset --hard <commit-id> : xoa luon commit va nhung thay đổi của nó (danger)

git revert <commit-id> : xoa di tất cả những thay đổi trong commit đó (những là xóa đi tất những dòng có dấu +)

git clone <url> : tai sourse ve may lan dau
git pull : dong bo source khi da co source


// pull request
git checkout -b <ten-branch> : tao 1 brach moi, ve lam viec tren branch do
git push origin <ten-brach> : push len 1 branch moi
pull request tren github
git fetch origin <ten-branch>


// resolve conflict
c1
ở branch conflict
git rebase master
git add . 
git rebases -continue
git push origin <ten-branch> -f

c1
git merge
...
