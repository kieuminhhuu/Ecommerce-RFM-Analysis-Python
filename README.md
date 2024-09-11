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
![his_f](https://github.com/user-attachments/assets/b51ab355-cecd-47b2-99d0-5cbc462a0bf1)
![his_m](https://github.com/user-attachments/assets/4b58366b-a2ce-4f33-a347-a52b05dd2b42)
![his_recency](https://github.com/user-attachments/assets/aae364f6-d2a1-4951-9408-cc5e8d9cca96)
![revenue](https://github.com/user-attachments/assets/81c771d7-94aa-422e-9fcf-1677def11609)
![scat_f_m](https://github.com/user-attachments/assets/dd5aeb43-3312-4ab5-9c56-14bc05b63a3b)
![scat_r_f](https://github.com/user-attachments/assets/7ca6f384-cbfd-4b26-b76b-5de9ac36fb04)
![scat_r_m](https://github.com/user-attachments/assets/8bc5dc03-8bb9-4a28-80ab-32357b161a6c)
![treemap](https://github.com/user-attachments/assets/6f41e36f-4a89-4c2a-addb-c857fc5caffc)
