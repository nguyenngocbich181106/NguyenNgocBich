# NguyenNgocBich
-) Mỗi file cần có:
+ Tên file (string)
+ Kích thước (MB hoặc GB)
+ Thời gian tạo (timestamp hoặc int)
-) Dùng Linked List (Danh sách liên kết đơn):
  Node:
- file (data)
- next (con trỏ)
Thiết kế cấu trúc & hàm
1. Struct file
   struct File {
    char name[100];
    float size;     
    int time;       
};
2. Node
   struct Node {
    File data;
    Node* next;
};
3. Danh sách hàm cần có
   Tạo node:Node* createNode(File f);
   Chèn theo thứ tự thời gian: void insertSorted(Node*& head, File f);
   Hiển thị danh sách: void display(Node* head);
   Tính tổng dung lượng: float totalSize(Node* head);
   Xóa file nhỏ nhất: void removeSmallest(Node*& head);
   Xử lý copy vào USB 32GB( Nếu tổng > 32GB → xóa file nhỏ nhất cho đến khi đủ) : void fitToUSB(Node*& head, float limit);
   
