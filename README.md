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
