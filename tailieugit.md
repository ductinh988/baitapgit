# **Tìm hiểu Git**
## **Git là gì?**
+ **git** là hệ thống quản lý phiên bản phân tán: (distributed version control system- DVCS) là một trong những hệ thống quản quản lý phiên bản phân tán phổ biến nhất hiện nay.

			 - giúp pc lưu trữ nhiều phiên bản khác nhau của 1 bộ mã nguồn (clone) từ một kho chứa mã nguồn (repository).

             - giúp lưu trữ các thay đổi trên mã nguồn sẽ được commit rồi đưa lên server nơi đặt kho chứa chính,
             - các pc khác (có quyền truy cập ) cũng có thể clone lại ãm nguồn để lấy phiên bản mới nhất.

			 
+ **source control**: là 1 ctrinh để quản lý source code
- **repo**: có thể là một dự án chứa nhiều source code
- **commit**: mỗi lần sửa code thêm file xóa file sửa file thay đổi code sẽ là 1 commit rồi lưu trên repo từ đó sẽ biết ai làm, ai sửa, ai thêm, 
- **repo có 2 loại**: local và remote 

		- local là repo bố trí trên máy của bản thân mình, dành cho 1 ng sử dụng
		- remote là repo được chia sẻ và bố trí trên server chuyên dụng.
- **branch**: là nhánh của master
- xóa nhánh (branch): *git branch -d tên branch*

- ***git init**: tạo ra repository trong máy 
- **git clone** lấy trên mạng về .
- **git pull:**pull code từ trên mạng về để đồng bộ với máy
- **git add:**hêm các file thêm mới hoặc được chỉnh sửa vào repo trong máy
- **git commit**: commit lên
- **git push:** đồng bộ code từ máy lên mạng
- **git log:** kiểm tra lịch sử commit
- **git status**: kiểm tra trạng thái của file.
- **git branch**: chia nhánh
- **git checkout**: chuyển sang nhánh khác
- **git merge** trộn nhánh
- **git rebase**: trộn nhánh : trộn nhánh 
- **git cherypick**:
- **.gitignore** : là file do git quy định. nhiệm vụ của nó là liệt kê nhwuxng file ma fminfh k mong muốn cho vào git.
- **git fetch**: được sử dụng để tải xuống các nội dung từ remote repo mà không làm thay đổi trạng thái của local repo(các dữ liệu như commit, các file, refs)
staging area: là khu vực theo dõi các file sẽ đc commit lần tiếp theo
 # sự khác nhau giữa clone , pull, fetch:
- **git clone**: sao chép toàn bộ dữ liệu trên repo và sao chép luôn các thiết lập về repo, tức là nó sẽ tự độngtạo một master branch trên máy tính

		** lưu ý**: Lệnh này chỉ nên sử dụng khi cần tạo mới Git repo trên máy tính với toàn bộ dữ liệu và thiết lập của một remote repository.

- **git pull**: tự động lấy toàn bộ dữ liệu từ remote repo và gộp vào branch hiện tại đang làm việc.
- **git fetch**: lấy toàn bộ dữ liệu từ remote repo nhưng sẽ cho phép gộp thủ công vào một branch nào đó trên thư mục git ở máy tính
		stage changes --> staging area --> commit changes --> local repo
 
- **index**: là nơi chuẩn bị ch việc commit

	** working --> edit --> add --> staging --> commit --> repo

-  **staging area**: khu vực theo dõi những file được thực hiện ở lần commit tiếp theo

         git restore --staged index2.css 

        git push --set-upstream origin  
