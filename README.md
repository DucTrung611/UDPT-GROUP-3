### 1. **Thuật giải nhân hai ma trận \(C[n,n] = A[n,n] \cdot B[n,n]\)**

#### a) **Thuật giải tuần tự:**
- **Mô tả:**
  - Tính mỗi phần tử \(C[i][j]\) của ma trận \(C\) bằng cách nhân từng hàng của \(A\) với từng cột của \(B\).
- **Độ phức tạp:** \(O(n^3)\), vì cần \(n^2\) phép tính với mỗi phép tính gồm \(n\) phép nhân.

#### b) **Thuật giải song song:**
- **Mô tả:**
  - Phân chia công việc tính các phần tử của ma trận \(C\) cho nhiều bộ xử lý. Mỗi bộ xử lý tính một tập hợp con của \(C\).
- **Độ phức tạp:** \(O(n^3/P + n)\), với \(P\) là số bộ xử lý. Thời gian giảm đi khi \(P\) tăng.

---

### 2. **Thuật giải sắp xếp dãy số nguyên \(a[n]\) bằng Merge Sort**

#### a) **Thuật giải tuần tự:**
- **Mô tả:**
  - Chia dãy thành hai nửa nhỏ hơn, đệ quy sắp xếp từng nửa, sau đó gộp hai nửa đã sắp xếp lại thành dãy hoàn chỉnh.
- **Độ phức tạp:** \(O(n \log n)\), vì có \(O(\log n)\) bước chia nhỏ và \(O(n)\) bước gộp dãy.

#### b) **Thuật giải song song:**
- **Mô tả:**
  - Phân chia dãy \(a\) thành các phần nhỏ và giao cho các bộ xử lý. Mỗi bộ xử lý sắp xếp một phần, sau đó các phần đã sắp xếp được gộp lại song song.
- **Độ phức tạp:** \(O((n/P) + (\log n / \log P))\), với \(P\) là số bộ xử lý. Nếu \(P\) gần bằng \(n\), độ phức tạp gần \(O(\log n)\).
