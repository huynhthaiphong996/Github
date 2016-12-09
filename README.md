# Github
# 1.Cách thức hoạt động của Github
* Làm việc với GitHub nói riêng hay hệ thống GIT nói chung có 2 workflow chính là local workflow và server workflow.  

* Bạn có thể làm mọi chuyện thay đổi source code ở local, sau khi đã thay đổi xong, bạn sẽ commit những thay đổi đó lên server và bản lên server phải là bản hoàn chỉnh một tính năng nào đó, hoặc fix bug xong, test xong hoặc ít nhất bản đó phải chạy được. Không được commit code dở dang, chưa qua test lên repository server sẽ làm ảnh hưởng đến các thành viên khác, ngược lại bạn có thể làm điều đó ở repository local (Bạn cũng có thể tạo một branch ở server cho việc commit code dở dang hay tính năng chưa hoàn thành như từng làm với SVN, nó sẽ chiếm space ở server cũng như làm mất thời gian của bạn vào việc tương tác kết nối với server, vậy tại sao không commit nó lên repository local nhỉ, vừa nhanh thao tác lại không mất space của server.  

# 2.Các khái niệm: Add, Remove, Commit, Push, Pull, Fetch, Clone, Fork, Star, Watch
* **Add** : soạn thảo thêm mới file đoạn code  
* **Commit** : update bản save hiện tại  
* **Push** : đẩy file từ máy trạm lên server(Overwrite)  
* **Pull** : kéo file từ server về máy trạm(Overwrite)  
* **Fetch** :hủy tất cả thay đổi và commit cục bộ, lấy về (fetch) lịch sử gần đây nhất từ máy chủ và trỏ nhánh master cục bộ vào nó  
* **Clone**: sao chép một repository  
* **Fork** : Lấy repo của người khác về trang cá nhân  
* **Star** : Gắn sao , tiện xem lại  
* **Watch** : Theo dõi Repo, nhận thông báo  

# 3.Tìm hiểu các bước để Setting up Git, Generate and add SSH key, Caching -your GitHub password in Git.  
## a/ Setting up Git (Windows)
Download tại địa chỉ: https://windows.github.com/  

Cài đặt bình thường, yêu cầu phải có .NET 4.5  

Giao diện của chương trình  
<img src="http://i.imgur.com/skKYQ2A.png">  
**Thêm tài khoản Github:**  
* Click vào tool and options (hình bánh răng cạnh biểu tượng Sync) chọn options, Add account. Khai báo username và password trên github.  
<img src="http://i.imgur.com/5IOsWvI.png">  

## b/ Generate and add SSH key

* Mở Git Bash  

* Nhập email của bạn: $ ssh-keygen -t rsa -b 4096 -C"your_email@example.com"  

* Enter a file in which to save the key (/Users/you/.ssh/id_sra): Pres Enter  

* Nếu nhập passphrase thì nhớ pass  

* Truy cập vào đường dẫn: https://github.com/settings/ssh

* Sau đó đặt tên cho file là Title và dán nội dung vừa copy vào ô Key

* Lúc này có thể commit mà không cần username hay password.


