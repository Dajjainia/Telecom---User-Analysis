# Telecom---User-Analysis

# PHÂN TÍCH ĐỘNG LỰC CHUYỂN ĐỔI 4G - XÁC ĐỊNH NHÓM KHÁCH HÀNG TIỀM NĂNG CHO VIỆC ĐẨY MẠNH CHUYỂN ĐỔI 4G

**## Đặt vấn đề: 
Trong lĩnh vực viễn thông, việc khách hàng chuyển đổi sang 4g đóng một vai trò quan trọng, đây là bước đầu, là cơ sở trong phễu chuyển đổi khách hàng, giúp cải thiện trải nghiệm sử dụng dịch vụ, sử dụng data cũng như là là bước đầu cho các dịch vụ công nghệ số trong tương lai

**## Giả định: 
Công ty mong muốn đội ngũ marketing có 1 chiến dịch tiếp cận khách hàng qua điện thoại để có thể tăng khả năng chuyển đổi người dùng thuê bao cũ hoặc đã đủ điều kiện để chuyển đổi. Với một budget có hạn, team marketing phải tìm ra giải pháp tối ưu về mặt cá nhân hóa cho mỗi thuê bao nhận tin. 

## Mục tiêu dự án
Xác định các yếu tố thúc đẩy và rào cản khiến khách hàng chuyển đổi từ hạ tầng cũ (2G/3G) lên 4G, từ đó xây dựng chân dung khách hàng tiềm năng và đề xuất chiến lược tiếp thị tối ưu.

## Quy trình xử lý dữ liệu
*   **Làm sạch:** Xử lý giá trị âm trong cước phí, chuẩn hóa tên cột và định dạng ID người dùng.
*   **Xử lý trùng lặp:** Phân loại và xử lý hai kịch bản trùng lặp (Lỗi Pipeline - Gộp dữ liệu; SIM đổi chủ - Giữ bản ghi mới nhất).
*   **Biến đổi:** Chuyển đổi dữ liệu từ dạng bảng rộng (Wide) sang bảng dọc (Long) theo thời gian để theo dõi hành vi qua 10 tháng.
*   **Gán nhãn:** Tạo biến mục tiêu `thuc_4g_next` để dự báo khả năng chuyển đổi trong tháng kế tiếp.

## Các Insight quan trọng
*   **Rào cản hạ tầng:** 18% khách hàng dù đã có đủ SIM 4G và thiết bị 4G nhưng vẫn chưa chuyển đổi, trong đó gần 50% gặp rào cản về vùng phủ sóng (hạ tầng thực tế vẫn là 2G/3G).
*   **Điểm bùng phát (The Surging Point):** Nhóm chuyển đổi có xu hướng tăng đột biến lưu lượng Data và tần suất nạp tiền qua kênh số (Topup) ngay trong tháng sát thời điểm chuyển đổi.
*   **Nhu cầu thực tế:** Người dùng thoại nhiều (Voice-centric) có tỷ lệ chuyển đổi thấp. Ngược lại, nhóm sử dụng Data thường xuyên (ngay cả ở mức thấp) là nhóm sẵn sàng nâng cấp nhất.
*   **Phân khúc RFM:** 
    *   **Nhóm Potential (Tiềm năng):** Có tỷ lệ chuyển đổi cao nhất (66.6%). Đặc điểm: Chi tiêu thấp nhưng nhu cầu Data cao và là nhóm khách hàng trẻ (25-45 tuổi).
    *   **Nhóm Loyal (Trung thành):** Chi tiêu cao, sử dụng dịch vụ số tốt nhưng cần được kích cầu về nội dung để tiêu dùng Data nhiều hơn.

## Chiến lược hành động đề xuất
1.  **Ưu tiên nhóm Potential:** Tập trung các gói cước Data dung lượng lớn với giá cạnh tranh.
2.  **Giáo dục nhóm Loyal:** Tặng kèm các gói dịch vụ nội dung (Video/Social) để làm quen với trải nghiệm 4G.
3.  **Real-time Marketing:** Kích hoạt ưu đãi ngay khi hệ thống ghi nhận lượt nạp tiền qua kênh Topup tăng bất thường.
4.  **Tối ưu hạ tầng:** Tập trung chăm sóc nhóm đủ điều kiện thiết bị nhưng sóng yếu bằng các giải pháp cải thiện vùng phủ hoặc thiết bị kích sóng.
