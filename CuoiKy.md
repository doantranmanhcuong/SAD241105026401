# A wilderness weather station
## I.Mô tả tóm tắt bài toán:
### 1.Mục tiêu của bài toán:
Xây dựng hệ thống trạm thời tiết tự động hoạt động trong các khu vực vùng sâu, vùng xa, không có cơ sở hạ tầng hỗ trợ (điện, đường giao thông, mạng viễn thông). Hệ thống này có nhiệm vụ thu thập, xử lý và truyền dữ liệu thời tiết về trung tâm để phục vụ:
- Nghiên cứu và phân tích biến đổi khí hậu ở cả cấp địa phương và quốc gia.
- Nâng cao độ chính xác của dự báo thời tiết quốc gia.
- Hỗ trợ quản lý tài nguyên thiên nhiên và phòng chống thiên tai.
### 2.Các đặc điểm chính của hệ thống:
#### 2.1.Tự cấp nguồn năng lượng:
- Sử dụng năng lượng tái tạo (năng lượng mặt trời hoặc gió) để vận hành toàn bộ hệ thống, không phụ thuộc vào nguồn điện bên ngoài.
#### 2.2.Giao tiếp từ xa qua vệ tinh:
- Truyền dữ liệu thời tiết về hệ thống trung tâm và nhận cập nhật phần mềm hoặc cấu hình từ xa.
#### 2.3.Hoạt động tự động và đáng tin cậy:
- Hệ thống phải hoạt động độc lập trong thời gian dài, có khả năng tự xử lý lỗi cơ bản và tự khởi động lại khi cần.
#### 2.4.Tự cấu hình và nâng cấp từ xa:
- Cho phép thay đổi cấu hình hoặc cập nhật phần mềm từ xa mà không cần truy cập trực tiếp.
### 3.Sự cần thiết và lợi ích khi giải quyết bài toán:
Trạm thời tiết vùng hoang dã là một thành phần quan trọng trong hệ thống thu thập thông tin thời tiết quốc gia. Việc xây dựng và triển khai trạm thời tiết tự động ở những khu vực không có cơ sở hạ tầng (điện, mạng, đường xá, v.v.) mang lại những lợi ích sau:
- Hỗ trợ nghiên cứu biến đổi khí hậu: Dữ liệu từ các trạm thời tiết giúp phân tích biến đổi khí hậu cục bộ và quốc gia, hỗ trợ các nhà khoa học đưa ra các dự báo chính xác hơn về xu hướng thời tiết trong tương lai.
- Cung cấp thông tin dự báo thời tiết: Các trạm này đóng góp vào hệ thống dự báo thời tiết quốc gia, phục vụ cho các hoạt động dự báo và cảnh báo sớm, đặc biệt là trong những tình huống thiên tai như bão, lũ lụt, hay hạn hán.
- Quản lý tài nguyên tự nhiên và giảm thiểu rủi ro thiên tai: Dữ liệu thời tiết có thể giúp các nhà khoa học và cơ quan chính phủ quản lý nguồn tài nguyên hiệu quả và phản ứng nhanh với các sự kiện thời tiết cực đoan.
### 4.Các yêu cầu chức năng:
#### 4.1.Thu thập và xử lý dữ liệu thời tiết:
- Trạm cần có khả năng đo và lưu trữ các thông số thời tiết như nhiệt độ, độ ẩm, áp suất không khí, tốc độ và hướng gió, lượng mưa.
- Dữ liệu phải được xử lý sơ bộ trước khi gửi về hệ thống trung tâm qua vệ tinh.
#### 4.2.Lưu trữ và xử lý dữ liệu:
- Hệ thống cần khả năng lưu trữ dữ liệu thu thập được trong bộ nhớ tạm thời, và sau đó gửi dữ liệu này lên hệ thống trung tâm khi có kết nối.
#### 4.3.Kết nối và truyền tải dữ liệu:
- Khi có tín hiệu vệ tinh hoặc mạng không dây, trạm cần có khả năng truyền tải dữ liệu về trung tâm để phân tích và sử dụng cho các mục đích dự báo.
#### 4.4.Quản lý năng lượng:
- Trạm cần có khả năng tự tạo điện năng từ nguồn năng lượng tái tạo như tấm pin mặt trời hoặc năng lượng gió và có hệ thống quản lý năng lượng hiệu quả để đảm bảo hoạt động liên tục.
#### 4.5.Khả năng tự động điều chỉnh và cấu hình lại:
- Hệ thống phần mềm cần có khả năng tự cấu hình lại để đối phó với các lỗi thiết bị, thay đổi trong môi trường, hoặc nâng cấp phần mềm từ xa.
#### 4.6.Bảo mật và độ tin cậy:
- Đảm bảo rằng dữ liệu được thu thập và truyền tải một cách an toàn, không bị tấn công hoặc giả mạo.
### 5.Các Yêu Cầu Phi Chức Năng:
Các yêu cầu phi chức năng cho hệ thống trạm thời tiết hoang dã chủ yếu tập trung vào khả năng hoạt động độc lập và tính bền vững của hệ thống:
#### 5.1.Tính độc lập và tự chủ:
- Vì các trạm thời tiết được triển khai ở những khu vực xa xôi, không có cơ sở hạ tầng, hệ thống phải hoạt động hoàn toàn độc lập. Điều này bao gồm tự cung cấp năng lượng, tự duy trì và tự khởi động lại sau sự cố.
#### 5.2.Khả năng chống chịu môi trường khắc nghiệt:
- Trạm cần phải có thiết kế bền vững để chịu được các điều kiện môi trường khắc nghiệt như gió mạnh, mưa lớn, nhiệt độ cực đoan, và các yếu tố tự nhiên khác.
#### 5.3.Tiết kiệm năng lượng:
- Với nguồn năng lượng hạn chế từ năng lượng tái tạo, trạm phải có khả năng tối ưu hóa việc sử dụng năng lượng để duy trì hoạt động liên tục trong điều kiện ít ánh sáng mặt trời hoặc gió
#### 5.4.Khả năng mở rộng:
- Hệ thống cần có khả năng dễ dàng mở rộng và thêm mới các trạm thời tiết mà không cần thay đổi cấu trúc hoặc phần mềm hệ thống hiện tại.
#### 5.5.Bảo trì và sửa chữa dễ dàng:
- Dù khó tiếp cận, nhưng hệ thống phần cứng và phần mềm của trạm cần phải thiết kế sao cho dễ bảo trì và sửa chữa từ xa, chẳng hạn như khả năng tự chẩn đoán sự cố và cập nhật phần mềm từ xa.

## II.Phân tích các ca sử dụng:
### 1. Kiến trúc đề xuất:
Hệ thống được thiết kế theo kiến trúc hướng đối tượng (object-oriented architecture) với các thành phần chính sau:
- Lớp cảm biến (Sensors):
  - Thu thập dữ liệu thời tiết từ các cảm biến như nhiệt độ, độ ẩm, tốc độ gió, áp suất không khí, lượng mưa.
  - Gửi dữ liệu thô đến lớp xử lý.

- Lớp xử lý dữ liệu (Data Processor):
  - Xử lý dữ liệu thô từ cảm biến, bao gồm làm sạch dữ liệu, phát hiện lỗi, và chuẩn bị dữ liệu để gửi đi.
  - Phân loại và lưu trữ dữ liệu tạm thời trong bộ nhớ.

- Lớp quản lý năng lượng (Power Management):
  - Theo dõi và quản lý việc tiêu thụ năng lượng của hệ thống.
  - Điều phối hoạt động của các thành phần dựa trên mức năng lượng hiện có từ nguồn tái tạo.

- Lớp truyền thông (Communication):
  - Kết nối với hệ thống vệ tinh để truyền dữ liệu về trung tâm.
  - Nhận lệnh hoặc bản cập nhật phần mềm từ trung tâm.

- Lớp quản lý lỗi (Fault Management):
  - Phát hiện lỗi phần cứng hoặc phần mềm và kích hoạt cơ chế khắc phục (tự cấu hình lại hoặc thông báo lỗi).

- Lớp điều khiển chính (Main Controller):
  - Điều phối hoạt động của các lớp trên, đảm bảo hệ thống hoạt động liên tục và chính xác.

### Biểu đồ kiến trúc đơn giản:
![Login](https://www.planttext.com/plantuml/png/ZLGzRnD14ErFklymFR54xG854X4X9SWeAMZNvvDlbTjPixSB14GHKQIWmK88KL0aLgeeIb12SokKugpyZ_qdxAxlOj-79LoSvDityzxCUtkRcIH2AfQ6GNP8SK84OH2b9CkUIYdeKCduHSHndtw8uN4OX84_Wpr2SOkZ53nDOm4Vmm3ixn7ClrAZZnLC4gEd519kybC9ywdHFt6y19bync1ednoC_euUy0KJi5Kd85sjGtzQykt7c76HxPAZLRQ3H3bqVZc1aT5Na5ho4_zA_w8WgSdlP8NTCVgIDc35hMFExn2sYIG3mQCuipIUfKRVFbwAU6qRGrhyRVMk08Eai3j8t052QlGFMftitbzRg71rqYwAbShNItvVSPMojpXZ2cb49ENObZtWxsAnHv2COnQZR6qlvZ0g_b30-MSSGtf_RVHiQPFLVOQLazqGg_0RwyE1oSyPJ2XkW5IaDwG8OrhSRBXNhgOSigQjBNr5cL17DaPOc_sD8l3MvuDYKY5VElSH8fy1T7-aNQM-i8JAwfN56QknFYSgbMitiaCBQqBcxF8-DV9OYZFwDnnQggl8B-SygfkwS6rOd7A8t6FHoIe_RejgNADUxqazwVt6XUgiw0ZdVzLrfgCFhvIzb-XJrZIzeqc7ZKroD_R2JdShrlJfDARLwI7_vSR3eBQkjTlORbtD3jZQSLQhvzDYzY0Z33fbkqQD4Vlmh1u8ftqpnf7_ylu3)


### 2.Các cơ chế phân tích:
#### 2.1.Cơ chế làm sạch dữ liệu (Data Cleaning): Làm sạch dữ liệu thu thập từ các cảm biến, loại bỏ các giá trị nhiễu hoặc không hợp lệ.
##### Phân tích cơ chế:
- Các cảm biến thu thập dữ liệu có thể gặp sự cố hoặc bị nhiễu do môi trường (ví dụ: cảm biến nhiệt độ bị ảnh hưởng bởi ánh sáng mặt trời trực tiếp hoặc cảm biến gió bị ảnh hưởng bởi các vật cản).
- Data Cleaning đảm bảo rằng dữ liệu đầu vào là chính xác và có thể sử dụng cho các phân tích sau này.
- Lợi ích: Giúp đảm bảo chất lượng dữ liệu đầu vào, từ đó cải thiện độ chính xác của dự báo thời tiết và các nghiên cứu về biến đổi khí hậu.
##### Các hoạt động chính:
- Loại bỏ các giá trị cực trị hoặc không hợp lý (ví dụ: nhiệt độ cực cao hoặc thấp).
- Chuẩn hóa dữ liệu từ các cảm biến khác nhau (ví dụ: chuyển đổi đơn vị đo lường nếu cần).

#### 2.2.Cơ chế phát hiện lỗi (Error Detection): Phát hiện các lỗi phần cứng hoặc lỗi dữ liệu bất thường trong hệ thống.
##### Phân tích cơ chế:
-Trạm thời tiết làm việc trong môi trường khắc nghiệt và xa xôi, vì vậy việc phát hiện lỗi kịp thời là rất quan trọng.
- Error Detection đảm bảo hệ thống có thể xác định các vấn đề như:
    - Lỗi phần cứng (ví dụ: cảm biến không hoạt động).
    - Dữ liệu bất thường hoặc bị lỗi (ví dụ: cảm biến bị hỏng hoặc gặp sự cố truyền thông).
- Lợi ích: Phát hiện lỗi sớm sẽ giúp tiết kiệm thời gian và chi phí sửa chữa, đồng thời duy trì tính ổn định của hệ thống.
##### Các hoạt động chính:
- Giám sát trạng thái các cảm biến và các thành phần hệ thống.
- So sánh dữ liệu thu thập được với các mô hình dự đoán (như mô hình khí hậu cơ bản) để phát hiện sự bất thường.

#### 2.3.Cơ chế giám sát năng lượng (Energy Monitoring): Theo dõi và quản lý mức năng lượng sử dụng của hệ thống.
##### Phân tích cơ chế:
- Trạm thời tiết cần hoạt động hoàn toàn tự động và không phụ thuộc vào nguồn năng lượng từ bên ngoài. Do đó, Energy Monitoring đóng vai trò quan trọng trong việc đảm bảo nguồn năng lượng luôn đủ để duy trì hoạt động của các cảm biến, bộ xử lý và hệ thống truyền thông.
- Lợi ích: Đảm bảo rằng hệ thống có đủ năng lượng để hoạt động liên tục, đặc biệt trong các điều kiện khắc nghiệt (ví dụ: thời tiết xấu, không có ánh sáng mặt trời).
- Các yếu tố năng lượng như tấm pin mặt trời, tua-bin gió và pin lưu trữ phải được theo dõi và điều phối để tối ưu hóa hiệu suất.
##### Các hoạt động chính:
- Theo dõi mức năng lượng từ các nguồn cung cấp (năng lượng mặt trời, gió, pin).
- Ước tính mức tiêu thụ năng lượng và cảnh báo khi mức năng lượng giảm xuống dưới ngưỡng tối thiểu.

#### 2.4.Cơ chế tự động cấu hình lại (Auto Reconfiguration): Khôi phục hoạt động của hệ thống khi phát hiện lỗi nhỏ hoặc sự cố.
##### Phân tích cơ chế:
- Hệ thống trạm thời tiết hoạt động ở những khu vực xa xôi, khó tiếp cận, do đó, việc sửa chữa hoặc can thiệp trực tiếp sẽ rất khó khăn.
- Auto Reconfiguration giúp hệ thống tự động khôi phục hoặc tái cấu hình khi gặp sự cố nhỏ (ví dụ: cảm biến bị hỏng, hoặc phần mềm gặp lỗi).
- Lợi ích: Tiết kiệm chi phí và thời gian, duy trì hoạt động của hệ thống mà không cần phải sửa chữa trực tiếp.
##### Các hoạt động chính:
- Cấu hình lại các thành phần hệ thống khi phát hiện lỗi nhỏ.
- Khởi động lại các cảm biến hoặc bộ phận bị lỗi mà không cần can thiệp từ xa.

#### 2.5.Cơ chế truyền thông qua vệ tinh (Satellite Communication): Đảm bảo việc truyền tải dữ liệu từ hệ thống trạm thời tiết đến trung tâm điều hành và nhận cập nhật từ trung tâm.
##### Phân tích cơ chế:
- Hệ thống cần truyền tải dữ liệu thời tiết thu thập được đến các trung tâm điều hành qua vệ tinh, vì khu vực lắp đặt không có cơ sở hạ tầng truyền thông.
- Satellite Communication cung cấp kênh truyền thông cần thiết cho hệ thống, giúp dữ liệu được truyền tải an toàn và hiệu quả.
- Lợi ích: Giúp hệ thống duy trì kết nối liên tục dù ở khu vực xa xôi, giúp cập nhật thông tin kịp thời và nhận các bản cập nhật hoặc lệnh từ trung tâm.
##### Các hoạt động chính:
- Truyền dữ liệu thu thập về trung tâm.
- Nhận các lệnh hoặc bản cập nhật phần mềm từ trung tâm.

#### 2.6.Cơ chế lưu trữ tạm thời (Temporary Storage): Lưu trữ tạm thời dữ liệu trước khi xử lý hoặc gửi đi.
##### Phân tích cơ chế:
- Dữ liệu từ các cảm biến cần được lưu trữ tạm thời để xử lý trước khi gửi đi hoặc khi cần thực hiện các phép tính phân tích.
- Temporary Storage giúp lưu trữ và giữ dữ liệu an toàn cho đến khi được xử lý hoặc truyền đi.
- Lợi ích: Đảm bảo rằng dữ liệu không bị mất trong trường hợp có sự cố và có thể được truy xuất lại khi cần thiết.
##### Các hoạt động chính:
- Lưu trữ dữ liệu trong bộ nhớ tạm thời trước khi gửi đi.
- Quản lý dung lượng bộ nhớ để tối ưu hóa việc lưu trữ.

### Biểu đồ quan hệ của các cơ chế:
![Login](https://www.planttext.com/plantuml/png/VLJBRjD05DrRyZ_SFQh4EWlKaY90F8H85smdpk0PrPunanc9WbXLA0iM9Ik4K0MXYX2Fg4M8ZKU8XQFyn_m9Tvn7FKbA5exjkVUSUyyvoMvV4wLDdiLH_v2BWYYIGvAHVdzFQyMxHjExYHGT_eB2zJYAe_eCzeacxOmImKKAB-C8y7CDxajNZZXqdJs1dhFda75d1mO4m-_NPbdMPiQLNmMmwXTfriNHgqk6Mqf9jKyrJJINufBZ4Qj66ZpWG43cx3iEYIlFSkXoL_uL_obhJjHrvLY3PhCBPqz56Z8BgjAZ1r9mBLMmtm6Z4dhLRmvYUem7cMy_mvi5Z_RhBujdvyv-I41N4y7MwpMllXcaTtOSKEyPBHzJrFifJuqYuUO7plw4wT3PzuY0EuyDAlW3mRDQTGGRr913F3vaVB6rm3SdIuXx-F2Hhq3cZPfLdn2bOAxy8hnvR-QjmMGTeccMSKtRCi-DuCdQSBUTdOGI8mdw0LePlt3rEL-MFaIYYV0RJ0e_NZb19vpz7fGsg0zeNaX5r547_I0fRUHjTc42Jcz0NejmklBX3kw2q2WyF3FL26zhqPxZm91LVxO4C0ZtpiwDzIosuCcoMIjlAThi1IysCXT7QwqURPl9BRXPZUJ2Cc_FyQR32BQUpAlXfc_dFmgyoetqAOdNfXXRkAumt3Dk6DBQuaHJcBGEntI8i1kz7Z0Gl0LjimXu4K0cJAvSypRjKj6h_xZ-0G00)
