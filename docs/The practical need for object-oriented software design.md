## 💡 1. Nhu cầu thực tế là gì?

Đây là những vấn đề xảy ra trong cuộc sống, công việc hoặc học tập mà con người muốn giải quyết bằng công nghệ.

### 👉 Ví dụ:

Thư viện của trường đang quản lý sách bằng giấy. Việc kiểm tra ai đang mượn sách, sách còn hay không, hay sách nào đã quá hạn rất mất thời gian và dễ sai sót.

### ✅ Nhu cầu: Cần một phần mềm quản lý thư viện để:

- Tra cứu sách nhanh

- Quản lý ai mượn sách

- Theo dõi hạn trả

## 🧠 2. Phần mềm giải quyết nhu cầu thực tế như thế nào?

Từ nhu cầu đó, ta viết phần mềm để mô phỏng và xử lý các tình huống thực tế. Phần mềm cần có các chức năng tương ứng với nhu cầu:

### 👉 Ví dụ chức năng trong phần mềm quản lý thư viện:

- Thêm/xóa/sửa thông tin sách

- Cho người dùng mượn/trả sách

- Thống kê số lượt mượn

- Kiểm tra hạn trả

### ➡️ Để làm được điều này, ta cần phân tích các đối tượng (thành phần) thực tế xuất hiện trong bài toán.

## 🧱 3. Lớp (Class) và Đối tượng (Object)

Trong lập trình hướng đối tượng (OOP), chúng ta mô hình hóa thế giới thực bằng class và object:

🔸 Lớp (Class):
Là khuôn mẫu mô tả một kiểu đối tượng.

Nó định nghĩa thuộc tính (dữ liệu) và phương thức (hành động).

🔸 Đối tượng (Object):
Là thực thể cụ thể được tạo ra từ class.

Ví dụ: lớp **Book** → tạo ra các đối tượng **book1**, **book2**...

### 👉 Ví dụ lớp và đối tượng:

```
public class Book {
    String title;
    String author;
    boolean isAvailable;

    void borrow() {
        isAvailable = false;
    }

    void returnBook() {
        isAvailable = true;
    }
}
```

- Lớp **Book** có 3 thuộc tính và 2 phương thức.

- Đối tượng:

```
Book b1 = new Book();
b1.title = "Lập trình Java";
b1.author = "Nguyễn Văn A";
b1.borrow(); // b1 đang được mượn
```

## 🔎 4. Thuộc tính và Phương thức là gì?

### ✅ Thuộc tính (Attributes):

- Là đặc điểm, trạng thái của một đối tượng

- Ví dụ: tên sách, tác giả, tình trạng còn hay đã mượn

### ✅ Phương thức (Methods):

- Là hành động mà đối tượng có thể thực hiện

- Ví dụ: mượn sách, trả sách, kiểm tra sách còn không

### 📌 Trong lớp **Book** ở trên:

- **title**, **author**, **isAvailable** là thuộc tính

- **borrow()**, **returnBook()** là phương thức

### 🔁 Chuỗi logic đầy đủ

| Bước | Diễn giải                                                            |
| ---- | -------------------------------------------------------------------- |
| 1️⃣   | Có một vấn đề thực tế (VD: quản lý thư viện thủ công)                |
| 2️⃣   | Ta cần viết phần mềm để giải quyết vấn đề đó                         |
| 3️⃣   | Dựa vào phân tích, ta xác định các lớp (VD: Book, User, Loan)        |
| 4️⃣   | Mỗi lớp mô tả một đối tượng với thuộc tính và phương thức            |
| 5️⃣   | Từ các lớp, ta tạo ra các đối tượng thực tế để vận hành chương trình |

### ✅ Tóm gọn:

> Nhu cầu thực tế → Tạo phần mềm → Phân tích thành Lớp → Mỗi lớp có Thuộc tính & Phương thức → Tạo ra các Đối tượng để chạy chương trình.
