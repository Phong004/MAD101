```mermaid
graph TD
    A[Cha] --> B[Con 1]
    A --> C[Con 2]
    B --> D[Cháu 1]
    B --> E[Cháu 2]
    C --> F[Cháu 3]
    C --> G[Cháu 4]

    
### Giải thích
- `graph TD`: Khai báo loại đồ thị (ở đây là **Top-Down**, từ trên xuống).
- `A --> B`: Mũi tên từ `A` (Cha) đến `B` (Con 1).
- `A --> C`: Mũi tên từ `A` đến `C` (Con 2), tạo ra một nhánh khác cho `A`.
- Tương tự, các nhánh còn lại sẽ kết nối các thành phần khác trong sơ đồ cây.

Bạn có thể mở rộng và tùy chỉnh các node hoặc thêm các nhánh khác nếu cần. Để hiển thị sơ đồ này, cần sử dụng trình hỗ trợ Mermaid (nhiều nền tảng như GitHub, GitLab hay Visual Studio Code đều hỗ trợ).

Root
├── Child 1
│   ├── Grandchild 1
│   └── Grandchild 2
├── Child 2
│   ├── Grandchild 3
│   └── Grandchild 4
└── Child 3
    └── Grandchild 5

