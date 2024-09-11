# Python_RFM_Analysis
## I. Introduction
### 1. RFM Analysis
- **RFM (Recency – Frequency – Monetary)**: là một phần của Marketing Analysis và được sử dụng để phân tích giá trị khách hàng (Customer Value), từ đó giúp doanh nghiệp có thể phân tích ra từng nhóm khách hàng mà mình đang có để có những chiến dịch marketing hoặc chăm sóc đặc biệt
  - Recency: Khoảng cách từ lần cuối cùng mua hàng tới ngày chỉ định
  - Frequency: Tần suất mua hàng trong một khoảng thời gian chỉ định
  - Monetary: Số tiền đã chi tiêu trong một khoảng thời gian chỉ
- **Phương pháp Ngũ phân vị (quintiles)** là một phương pháp thống kê chia dữ liệu thành năm nhóm (hoặc phân vị) bằng nhau, mỗi nhóm chiếm 20% tổng số quan sát
- **Cách chấm điểm cho mỗi chỉ số**: gán điểm từ 1 đến 5 cho các chỉ số R, F, M, các chỉ số này sẽ được chia theo phương pháp **ngũ phân vị**:
  - Recency: Khách hàng mua gần đây hơn sẽ có điểm cao hơn
  - Frequency: Khách hàng mua hàng thường xuyên sẽ có điểm cao hơn
  - Monetary: Khách hàng chi tiêu nhiều hơn sẽ nhận được điểm cao hơn
- Kết hợp điểm của từng chỉ số RFM để tạo ra điểm tổng thể cho mỗi khách hàng từ đó phân vào nhóm khách hàng tương ứng
### 2. Dataset
- Là một tập dữ liệu của một công ty bán lẻ trực tuyến đa quốc gia chứa tất cả các giao dịch diễn ra trong khoảng thời gian từ 01/12/2010 đến 09/12/2011. Công ty chủ yếu bán các loại quà tặng cho các dịp đặc biệt. Nhiều khách hàng của công ty là người bán buôn
### 3. Data Description
![ds](https://github.com/user-attachments/assets/2b786299-b2ea-4e15-adc3-22fe2f2a85d3)
### 4. Business Question
- Phòng Marketing muốn chạy các chiến dịch marketing để tri ân khách hàng đã ủng hộ công ty suốt thời gian qua cũng như khai thác các khách có tiềm năng trở thành khách hàng trung thành vì vậy phòng Marketing cần phần nhóm khách hàng. Giám đốc Marketing đề xuất với team phương án sử dụng mô hình RFM được triển khai bằng Python để có thể xử lý lượng data lớn hiện có của công ty tư đó thực hiện phân tích và đưa ra khuyến nghị 
## II. Data Visualization bằng Python
- Phân bố của giá trị R <br />
<img src="https://github.com/user-attachments/assets/aae364f6-d2a1-4951-9408-cc5e8d9cca96" alt="..." width="600" /><br />
- Phân bố của giá trị F <br />
<img src="https://github.com/user-attachments/assets/b51ab355-cecd-47b2-99d0-5cbc462a0bf1" alt="..." width="600" /><br />
- Phân bố của giá trị M <br />
<img src="https://github.com/user-attachments/assets/4b58366b-a2ce-4f33-a347-a52b05dd2b42" alt="..." width="600" /><br />
- Phân bố của giá trị R và F <br />
<img src="https://github.com/user-attachments/assets/7ca6f384-cbfd-4b26-b76b-5de9ac36fb04" alt="..." width="600" /><br />
- Phân bố của giá trị R và M <br />
<img src="https://github.com/user-attachments/assets/8bc5dc03-8bb9-4a28-80ab-32357b161a6c" alt="..." width="600" /><br />
- Phân bố của giá trị F và M <br />
<img src="https://github.com/user-attachments/assets/dd5aeb43-3312-4ab5-9c56-14bc05b63a3b" alt="..." width="600" /><br />
- Treemap của các Segment <br />
<img src="https://github.com/user-attachments/assets/6f41e36f-4a89-4c2a-addb-c857fc5caffc" alt="..." width="600" /><br />
- Doanh thu từ các Segment <br />
<img src="https://github.com/user-attachments/assets/81c771d7-94aa-422e-9fcf-1677def11609" alt="..." width="600" /><br />
## Insight
- Từ biểu đồ doanh thu theo các segment ta thấy nhóm champions đóng góp doanh thu rất lớn cho doanh nghiệp -> đặc điểm của nhóm này là thường xuyên mua hàng với giá trị đơn hàng cao -> cần có những biện pháp giữa chân nhóm khách hàng này
- Nhìn vào biểu đồ TreeMap ta thấy 4 nhóm Lost, New Customer, Hibernating Customer, Promissing chiếm tỷ lệ phần trăm thứ 1,3,4,5 trong nhóm khách hàng. Hành vi của từng nhóm này như sau:
  - Lost là nhóm khách hàng lâu rồi không quay trở lại, giá trị đơn hàng nhóm này không cao
  - New Customers là nhóm khách hàng mới mua hàng gần đây, tần suất mua và giá trị đơn hàng không cao
  - Hibernating Customer là nhóm khách hàng đã lâu rồi không quay trở lại, sức mua yếu và giá trị giỏ hàng không cao
  - Promissing là nhóm khách hàng mới mua gần đây, giá trị đơn hàng lớn nhưng chưa mua thường xuyên
- Cả 4 nhóm này chiếm tỷ lệ lớn trong nhóm khách hàng nhưng lại đem lại doanh thu rất thấp, kết hợp với các biểu đồ scatter có thể thấy doanh nghiệp chưa có biến pháp thu hút khách hàng quay trở lại mua hàng và chưa có biện pháp tăng tần suất và giá trị mua hàng từ đó dẫn tới nhóm khách hàng trung thành và khách hàng tiềm năng chiếm tỷ lệ rất thấp
## Recomendation
- Đối với nhóm Champions cần có ra những chương trình riêng dành cho khách hàng trung thành ví dụ như chương trình tích điểm, các quyền lợi mà chỉ khách hàng VIP mới có hoặc cung cấp dịch vụ chăm sóc khách hàng tốt hơn để giữ chân nhóm khách hàng này
- Cần có biện pháp thu hút lại những khách hàng lâu rồi không quay trở lại như nhóm Lost, Hibernating, Needing Attension. Một số biện pháp:
  - Gửi email giới thiệu các loại sản phẩm mới dựa trên các sản phẩm đã mua hoặc các sản phẩm mà khách hàng quan tâm
  - Tặng phiếu giảm giá khi quay trở lại mua hàng
- Để tăng tần suất mua hàng hoặc giá trị đơn hàng đối với các nhóm New Customers, Promising có thể sử dụng các cách sau:
  - Gửi thông tin giới thiệu các sản phẩm tương tự với những sản phẩm khác hàng đã mua nhưng loại sản phẩm chất lượng hơn
  - Gửi thông tin giới thiệu các sản phẩm đi kèm với sản phẩm khách hàng đã mua
