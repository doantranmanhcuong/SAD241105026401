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

### 3.Kết quả các ca phân tích:
#### Ca sử dụng 1: Thu thập dữ liệu thời tiết
##### Mục tiêu: Thu thập dữ liệu về các yếu tố khí hậu (nhiệt độ, độ ẩm, áp suất không khí, tốc độ gió) từ các cảm biến trong khu vực.
- Mô tả:
  - Người tham gia: Cảm biến (sensors), hệ thống giám sát.
- Tiến trình:
  - Cảm biến đo lường các yếu tố khí hậu.
  - Dữ liệu thu thập được sẽ được chuyển tiếp đến DataProcessorLayer để làm sạch và xử lý.
- Kết quả: Dữ liệu thời tiết chính xác được thu thập và chuyển đến lớp xử lý.

#### Ca sử dụng 2: Xử lý dữ liệu và phát hiện lỗi
##### Mục tiêu: Xử lý dữ liệu thu thập được từ các cảm biến, đồng thời phát hiện lỗi trong quá trình thu thập.
- Mô tả:
  - Người tham gia: DataProcessorLayer, ErrorDetection.
- Tiến trình:
  - Dữ liệu thô được gửi đến DataProcessorLayer để làm sạch và xử lý.
  - ErrorDetection phát hiện lỗi dữ liệu hoặc phần cứng.
  - Nếu phát hiện lỗi, hệ thống sẽ gửi cảnh báo về FaultManagementLayer.
- Kết quả: Dữ liệu được xử lý và lỗi (nếu có) sẽ được phát hiện và báo cáo.
  
#### Ca sử dụng 3: Quản lý năng lượng
##### Mục tiêu: Quản lý nguồn năng lượng của hệ thống để đảm bảo hoạt động liên tục.
- Mô tả:
  - Người tham gia: PowerManagementLayer.
- Tiến trình:
  - EnergyMonitoring theo dõi tình trạng năng lượng của hệ thống.
  - Kiểm tra mức năng lượng từ các nguồn (pin mặt trời, tua-bin gió, pin lưu trữ).
  - Nếu mức năng lượng quá thấp, hệ thống sẽ kích hoạt chế độ tiết kiệm năng lượng hoặc gửi cảnh báo về trung tâm.
-Kết quả: Đảm bảo hệ thống luôn có đủ năng lượng hoạt động và không bị gián đoạn.

#### Ca sử dụng 4: Truyền tải dữ liệu qua vệ tinh
##### Mục tiêu: Truyền tải dữ liệu về trung tâm điều khiển để phân tích và lưu trữ.
- Mô tả:
  - Người tham gia: CommunicationLayer, SatelliteCommunication.
- Tiến trình:
  - Dữ liệu đã được xử lý sẽ được gửi qua vệ tinh đến trung tâm điều khiển.
  - Dữ liệu có thể là các thông tin thời tiết, báo cáo sự cố hoặc cập nhật từ hệ thống.
  - Trung tâm điều khiển sẽ nhận dữ liệu và đưa ra quyết định dựa trên thông tin nhận được.
- Kết quả: Dữ liệu được truyền đi thành công, đảm bảo việc theo dõi và phân tích từ xa.

#### Ca sử dụng 5: Phát hiện và xử lý lỗi tự động
##### Mục tiêu: Phát hiện lỗi trong hệ thống và tự động tái cấu hình để tiếp tục hoạt động.
- Mô tả:
  - Người tham gia: FaultManagementLayer, AutoReconfiguration.
- Tiến trình:
  - FaultManagementLayer giám sát và phát hiện các lỗi hệ thống (cảm biến không hoạt động, mất kết nối, lỗi dữ liệu).
  - AutoReconfiguration tự động khôi phục hệ thống khi có lỗi nhỏ, chẳng hạn như tái khởi động lại cảm biến hoặc hệ thống.
  - Nếu lỗi không thể tự động xử lý, hệ thống sẽ gửi cảnh báo về trung tâm điều khiển.
- Kết quả: Hệ thống khôi phục hoạt động hoặc cảnh báo về lỗi nghiêm trọng.

#### Ca sử dụng 6: Lưu trữ tạm thời dữ liệu
##### Mục tiêu: Lưu trữ dữ liệu tạm thời trước khi xử lý hoặc truyền tải.
- Mô tả:
  - Người tham gia: TemporaryStorage, DataCleaning.
- Tiến trình:
  - Dữ liệu thu thập được từ cảm biến được lưu trữ tạm thời trong bộ nhớ.
  - Sau đó, dữ liệu này sẽ được xử lý bởi DataCleaning và ErrorDetection để làm sạch và phát hiện lỗi.
- Kết quả: Dữ liệu được lưu trữ an toàn và có thể truy xuất lại khi cần thiết.

### Biểu đồ kết quả các ca sử dụng:
![Login](https://www.planttext.com/plantuml/png/ZLJ1RjD04Br7oZ-CUk-1j6ah3gZ2792Agg0cWglZM5chphhOkuKUKG-vaXFYW4HQ8GvjHP4uUOKuEEf_x9ymit7YtIIkk3Yoi-_DU_DczZ0JVYhaA6us_40aAMnrKvrFHz1bMdsDe1lf_A_O0Z-3Dw4lM9YU25z42RVEIpw4Rd4rWjcdIAkF4euO_bvoW_8IBj8aza8kmdG9ydH-FOBdH3u_TXBoBAd-VwdLs4YO8FVnx1AVhnxkjRhcGtEyaxn79HUP24VDHhCXip3min35C0c2wVpk30PQ_OGOXOpD9p8ZAZCzxua5UwlL7SJ57mTqNdo3CrPC1P2TCOTOgyzHYMvPwDSItN23vqPgR4ljUJksm5HUO8yu2CH4JhrtqeTpyYqYpahehWNjs5f8t8U5QYCC6TKlc4sq-hAitBRWs3ziH4e5XKcuR8ebeKJjRKPjzBPldJsYr94tzOsyFZfCyAsuXS34tQ_Yxda7b9ixKh2z_Oo2WQTGbwDMDmvP3KKBAPQPafRJIfh5LuFUGRJbHT12e7E1_OzMkb33q4Q6pjhe03FfpgUw1hc7oFz8YfhdR5O9tqNuCVLjFY53xC4ZGxQPerrneENVwBPVJ9FI0h5Y0DybiEAMC_oQJrUDDHlpRRRozEYE89oRfnkbjTHM4XRKxJq4B5cflCwmx_PpXM7mS6_0Dpwf9gdL_BnmTVxWrRvbleHJXXktd582jwm8ry6pYIaQKF6DwIv85rM8ibrI7hWJ-SXs6OhrMuli7OPyO2xwVm00)

## Xác định các phần tử thiết kế:
## 1. Xác định các lớp và các hệ thống con

**1. Các lớp chính trong hệ thống:**

**1.1. Lớp WeatherStation (Trạm thời tiết)**

#### Thuộc tính:

- stationID: ID duy nhất của trạm.
- location: Vị trí địa lý (kinh độ, vĩ độ).
- powerStatus: Trạng thái nguồn (mức pin, năng lượng mặt trời/wind generator hoạt động).
- communicationStatus: Trạng thái kết nối vệ tinh.
- sensorData: Bộ dữ liệu thu thập từ các cảm biến (tốc độ gió, hướng gió, nhiệt độ, áp suất, lượng mưa...).
- localStorage: Bộ nhớ cục bộ lưu dữ liệu khi mất kết nối.
  
#### Phương thức:

- collectData(): Thu thập dữ liệu từ các cảm biến.
- processData(): Xử lý và tổng hợp dữ liệu trước khi truyền.
- transmitData(): Truyền dữ liệu đã xử lý đến hệ thống quản lý.
- storeDataLocally(): Lưu dữ liệu cục bộ khi không thể truyền đi.
- monitorHardware(): Giám sát trạng thái phần cứng (cảm biến, truyền thông).
- managePower(): Quản lý nguồn năng lượng và sạc pin.
- reconfigureSystem(): Cấu hình lại hệ thống khi có thay đổi phần mềm hoặc lỗi phần cứng.

**1.2. Lớp Sensor (Cảm biến)**

#### Thuộc tính:

- sensorType: Loại cảm biến (nhiệt độ, áp suất, gió, mưa...).
- sensorID: ID duy nhất của cảm biến.
- dataFrequency: Tần suất đo lường.
- status: Trạng thái hoạt động của cảm biến.
  
#### Phương thức:

- readData(): Đọc dữ liệu thời tiết từ cảm biến.
- calibrate(): Hiệu chỉnh cảm biến.
- selfCheck(): Tự kiểm tra trạng thái hoạt động.
  
**1.3. Lớp PowerManagement (Quản lý nguồn)**

#### Thuộc tính:

- batteryLevel: Mức pin hiện tại.
- solarPanelStatus: Trạng thái tấm năng lượng mặt trời.
- windGeneratorStatus: Trạng thái máy phát gió.
  
#### Phương thức:

- chargeBattery(): Sạc pin từ nguồn năng lượng tái tạo.
- shutDownInStorm(): Tắt hệ thống khi điều kiện thời tiết nguy hiểm.
- optimizePowerUsage(): Tối ưu hóa tiêu thụ năng lượng.
  
**1.4. Lớp Communication (Truyền thông)**

#### Thuộc tính:

- satelliteLinkStatus: Trạng thái liên kết vệ tinh.
- bandwidth: Băng thông vệ tinh hiện có.
  
#### Phương thức:

- establishConnection(): Kết nối với vệ tinh.
- transmit(): Truyền dữ liệu đến hệ thống quản lý.
- retryTransmission(): Thử lại khi truyền thất bại.
  
**1.5. Lớp DataManagement (Quản lý dữ liệu)**

#### Thuộc tính:

- rawData: Dữ liệu thô từ cảm biến.
- processedData: Dữ liệu đã được xử lý.
- storageCapacity: Dung lượng lưu trữ cục bộ.
  
#### Phương thức:

- aggregateData(): Tổng hợp dữ liệu theo khoảng thời gian.
- compressData(): Nén dữ liệu để tối ưu truyền tải.
- clearOldData(): Xóa dữ liệu cũ để giải phóng dung lượng.
  
**1.6. Lớp Maintenance (Bảo trì)**

#### Thuộc tính:

- hardwareStatus: Tình trạng phần cứng.
- errorLogs: Nhật ký lỗi.
- softwareVersion: Phiên bản phần mềm hiện tại.
  
#### Phương thức:

- sendStatusReport(): Gửi báo cáo tình trạng đến hệ thống bảo trì.
- updateSoftware(): Cập nhật phần mềm.
- performDiagnostics(): Chạy chẩn đoán lỗi.
  
## **2. Quan hệ giữa các lớp:**

#### WeatherStation liên kết với nhiều Sensor:

- Mỗi trạm thời tiết bao gồm nhiều cảm biến để đo các thông số khác nhau.
  
#### WeatherStation sử dụng PowerManagement:

- Quản lý nguồn là một phần quan trọng của trạm thời tiết.
  
#### WeatherStation liên kết với Communication:

- Để giao tiếp với hệ thống quản lý và bảo trì qua vệ tinh.
  
#### WeatherStation liên kết với DataManagement: 

- Để xử lý, lưu trữ và truyền tải dữ liệu.
  
#### Maintenance liên kết với WeatherStation:

- Để theo dõi trạng thái và thực hiện các hoạt động bảo trì.

##  **3. Ánh xạ từ lớp phân tích đến các phần tử thiết kế**

 ### 1. Lớp WeatherStation
 
**Phân tích:**
- Trạm thời tiết là lớp chính, chịu trách nhiệm tổng hợp dữ liệu từ các cảm biến, xử lý dữ liệu, và quản lý giao tiếp với các hệ thống khác.
  
**Thiết kế:**
  
- Đảm bảo rằng lớp này hoạt động như bộ điều phối chính (Coordinator Class), tương tác với các lớp phụ trợ như Sensor, PowerManagement, Communication, và DataManagement.
  
- Sử dụng các mẫu thiết kế như Facade Pattern để cung cấp một giao diện thống nhất cho các chức năng của trạm.
  
**Chi tiết thiết kế:**
**Thuộc tính:**
- stationID: String
- location: Coordinates (Lớp con đại diện cho kinh độ/vĩ độ).
- powerManagement: PowerManagement
- communication: Communication
- sensors: List<Sensor>
- dataManager: DataManagement
  
**Phương thức:**
- collectData(): Điều phối việc lấy dữ liệu từ các cảm biến.
- transmitData(): Sử dụng Communication để gửi dữ liệu đã xử lý.
- handleFault(): Quản lý lỗi thông qua các phương thức của Maintenance.
  
### 2. Lớp Sensor
**Phân tích:**
- Các cảm biến đo các thông số thời tiết và cung cấp dữ liệu thô.
  
**Thiết kế:**
- Triển khai lớp trừu tượng (Abstract Class) Sensor để đại diện cho các loại cảm biến khác nhau, sau đó kế thừa để cụ thể hóa từng loại cảm biến.
- Mẫu thiết kế Strategy Pattern có thể được áp dụng nếu các cảm biến có cách xử lý dữ liệu khác nhau.

**Chi tiết thiết kế:**

**Lớp trừu tượng Sensor:**

**Thuộc tính:**

- sensorID: String
- sensorType: SensorType (Enum gồm: TEMPERATURE, PRESSURE, WIND_SPEED, v.v.).
- dataFrequency: int (Tần suất đo lường).
  
**Phương thức:**

- readData(): WeatherData (Phương thức trừu tượng).
- selfCheck(): Boolean (Phương thức trừu tượng).
- Lớp cụ thể (VD: TemperatureSensor, WindSensor):
- Cài đặt readData() và selfCheck() dựa trên loại cảm biến.
  
### 3. Lớp PowerManagement

**Phân tích:**
- Lớp này quản lý nguồn pin và các cơ chế sạc năng lượng tái tạo.
  
**Thiết kế:**
- Phân tách quản lý năng lượng thành các mô-đun nhỏ hơn:
- BatteryManager: Quản lý pin.
- EnergyHarvesting: Quản lý năng lượng mặt trời và gió.
- Áp dụng Observer Pattern để giám sát mức năng lượng và kích hoạt hành động khi năng lượng thấp.
  
**Chi tiết thiết kế:**
  
**Thuộc tính:**
- batteryLevel: int
- solarPanelStatus: Boolean
- windGeneratorStatus: Boolean
**Phương thức:**
- chargeBattery(): Kích hoạt sạc.
- shutDownInStorm(): Ngắt hoạt động trong điều kiện thời tiết khắc nghiệt.
- optimizePowerUsage(): Tối ưu hóa sử dụng năng lượng.
### 4. Lớp Communication

**Phân tích:**

- Quản lý giao tiếp giữa trạm và hệ thống quản lý qua vệ tinh.
  
**Thiết kế:**
- Đưa thêm các chiến lược dự phòng như lưu dữ liệu cục bộ khi mất kết nối.
- Áp dụng Command Pattern để đảm bảo việc truyền dữ liệu được thực hiện tuần tự và có thể thử lại nếu thất bại.
  
**Chi tiết thiết kế:**
**Thuộc tính:**
- satelliteLinkStatus: Boolean
- bandwidth: int
- Phương thức:
- establishConnection(): Boolean
- transmit(data: ProcessedData): Boolean
- retryTransmission(data: ProcessedData): Boolean
### 5. Lớp DataManagement
**Phân tích:**
- Xử lý, tổng hợp và lưu trữ dữ liệu thu thập từ các cảm biến.
  
**Thiết kế:**
- Tối ưu hóa dữ liệu trước khi truyền để giảm băng thông qua Compression Algorithms.
- Áp dụng Singleton Pattern để đảm bảo chỉ có một bộ quản lý dữ liệu cho mỗi trạm.
  
**Chi tiết thiết kế:**
**Thuộc tính:**
- rawData: List<WeatherData>
- processedData: ProcessedData
- storageCapacity: int
  
**Phương thức:**
- aggregateData(): ProcessedData
- compressData(data: ProcessedData): CompressedData
- clearOldData(): Giải phóng dung lượng lưu trữ.
### 6. Lớp Maintenance
**Phân tích:**

- Hệ thống bảo trì theo dõi trạng thái phần cứng và thực hiện cập nhật từ xa.
  
**Thiết kế:**
- Tích hợp Remote Update System và cơ chế chẩn đoán lỗi tự động.
- Sử dụng Template Method Pattern để đảm bảo các quy trình bảo trì diễn ra theo một trình tự chuẩn.
  
**Chi tiết thiết kế:**

**Thuộc tính:**
- hardwareStatus: Map<Component, Status>
- errorLogs: List<ErrorLog>
- softwareVersion: String
  
**Phương thức:**
- sendStatusReport(): StatusReport
- updateSoftware(version: String): Boolean
- performDiagnostics(): DiagnosticReport

 ## 4.Nhóm các lớp thiết kế vào package
**Package weatherstation**

- Chứa lớp trung tâm WeatherStation.
  
**Package sensor**

**Chứa các lớp liên quan đến cảm biến:**
- Sensor (lớp cơ sở).
- TemperatureSensor.
- PressureSensor.
- WindSensor.
- RainSensor.
- Package power

**Chứa lớp PowerManagement.**
- Package communication

**Chứa lớp Communication.**
- Package data

**Chứa lớp DataManagement**
- Package maintenance

**Chứa lớp Maintenance.**
#### Biểu đồ Package
![Diagram](https://www.planttext.com/plantuml/png/X5R1Rjim3BtdAuITEc3v0QCeYYNhK235WgPRpupCEa9bogFePjdMBzjXdxHV66JBjfouxIcX-4JfFP4l-VVdxwKNOAbBEwj0FqA1wjqUGNR8Na2CetVgrqmfRS5xTTzcDcscIIWrLn5vlSpKHjXG4TUjqqqYKmldE3S4WZxcAhT7lW620aiaoTHwl11XsfLbJMQeauJTwKZUiS_KodWvtpJHHSpb8D3Mv4mj-o0ve0H3WWIaCLCtGz2cvys7KjfPYrf2XRFtcNfo9eyPOI1VcgdK3YYtU0MrbIJpF7kU3LgtbsyrXgqN1YrHx9R9878JdcZSBjyTAipYZl0zeN_5-Br6qeTCcPvrUB7QPshhd4MWCLb6o3iwySL3s4a1rcmP18_OUhGFYntgnx0-r7sUzTrpXsM5358pHcxuGv3oZceFN3Dw_oRgtb3-Ek8M34qZqYUeGkEbNNxKYVqBR444-R329xGZCPq5NWEXtKp9glQ6yiz8WRfhPkT5vVKEkC2FxJb7-hfAJ6b-OdExhnwAamVOrR9qUxgcZJWkNsovqKYbl4V3DVGT25fh15U67gS9Re7olSbbbwZIKK8liBN6xnQE27KeFMwGT8ZEGiDcQirEe_VOTE49c57uSDVky3xKUslNc7z0fxJ7jj3pPjY7JBILP0uwRwdIyuwExyVCCHIuW0gqaSE4F50KZ0K8TWDtMYQuJrc5aMWmqsGN4JBUPn7uY-s7UR8T4WDCLKcii9Ta1vplWR7hWXkepiF1Zf3aWsgNEtcGsV7A5PqnVufnb_VkGKAnRyZX4SUsridZaVAsx2rMZXiVJUC8gwiS13UnujdJkEH91rN83uxBfO62d1UZVQWxX7tjHgcZ7xtv_AApvanfHmA6lBgOWgsFZ2HJjSSNiEFXUmrvrA-lGTD7x77nykU_v_DJInvbnpuyIWtcEreU77TsYPI7lnN_0G00__y30000)

### Giải thích biểu đồ Package:

- Các lớp được nhóm theo chức năng trong hệ thống.
- Lớp **WeatherStation** nằm ở package trung tâm và liên kết với tất cả các package con.
- Package **sensor** chứa lớp cơ sở Sensor và các lớp cụ thể như **TemperatureSensor**, **PressureSensor.**
- Package **power**, **communication**, **data**, và **maintenance** độc lập, nhưng được sử dụng bởi lớp WeatherStation.

## 5.Xác định giao diện của hệ thống con

**1. Hệ thống trạm thời tiết (WeatherStationSubsystem)**

**Giao diện:** IWeatherStation
- Giao diện cung cấp các chức năng để thu thập và quản lý dữ liệu thời tiết từ các cảm biến.
  
**Phương thức:**
- collectData(): WeatherData
→ Thu thập dữ liệu từ các cảm biến trên trạm.
- getStationStatus(): StationStatus
→ Lấy thông tin trạng thái của trạm (năng lượng, cảm biến, kết nối...).
- transmitData(): void
→ Truyền dữ liệu đã xử lý đến hệ thống quản lý.
- storeDataLocally(): void
→ Lưu dữ liệu cục bộ khi không thể truyền tải.
- configure(newConfig: StationConfig): boolean
→ Cập nhật cấu hình hoạt động của trạm thời tiết.

**2. Hệ thống quản lý và lưu trữ dữ liệu (DataManagementSubsystem)**

 **Giao diện:** IDataManagement
- Giao diện xử lý và lưu trữ dữ liệu từ các trạm thời tiết.
  
 **Phương thức:**
- receiveData(data: WeatherData): boolean
→ Nhận dữ liệu thời tiết từ trạm.
- processData(rawData: WeatherData): ProcessedData
→ Xử lý dữ liệu thô thành dạng tổng hợp.
- storeData(data: ProcessedData): boolean
→ Lưu trữ dữ liệu đã xử lý vào hệ thống cơ sở dữ liệu.
- retrieveData(query: Query): DataResult
→ Truy xuất dữ liệu dựa trên các truy vấn.

**3. Hệ thống bảo trì trạm (MaintenanceSubsystem)**

**Giao diện:** IMaintenance
- Giao diện giám sát, bảo trì, và cập nhật phần mềm trạm thời tiết.
  
**Phương thức:**
- getHardwareStatus(stationID: String): HardwareStatus
→ Lấy thông tin trạng thái phần cứng của trạm.
- sendUpdate(stationID: String, updatePackage: Update): boolean
→ Gửi gói cập nhật phần mềm tới trạm.
- runDiagnostics(stationID: String): DiagnosticReport
→ Chạy chẩn đoán lỗi trên trạm từ xa.
- resetStation(stationID: String): boolean
→ Khởi động lại trạm khi cần thiết.
- scheduleMaintenance(stationID: String, time: DateTime): boolean
→ Lập kế hoạch bảo trì trạm.

**4. Hệ thống giao tiếp vệ tinh (SatelliteCommunicationSubsystem)**

**Giao diện:** ICommunication
- Giao diện quản lý giao tiếp giữa trạm thời tiết và hệ thống quản lý qua vệ tinh.
  
**Phương thức:**
- establishConnection(stationID: String): boolean
→ Thiết lập kết nối với một trạm thời tiết.
- sendData(data: CompressedData, stationID: String): boolean
→ Truyền dữ liệu từ hệ thống đến trạm qua vệ tinh.
- receiveData(stationID: String): CompressedData
→ Nhận dữ liệu từ trạm qua vệ tinh.
- checkConnectionStatus(stationID: String): boolean
→ Kiểm tra trạng thái kết nối vệ tinh của một trạm.

**5. Hệ thống dự báo thời tiết (WeatherForecastingSubsystem)**

**Giao diện:** IForecasting
- Giao diện xử lý và dự báo thời tiết dựa trên dữ liệu đã thu thập.
  
**Phương thức:**
- getWeatherData(query: Query): DataResult
→ Lấy dữ liệu thời tiết đã xử lý từ hệ thống lưu trữ.
- generateForecast(region: String, timeRange: TimeRange): ForecastResult
→ Tạo dự báo thời tiết cho một khu vực cụ thể.
- updateModel(modelConfig: ModelConfig): boolean
→ Cập nhật mô hình dự báo thời tiết.

### Biểu đồ thiết kế giao diện của hệ thống con 

![Diagram](https://www.planttext.com/plantuml/png/Z5LBRjim4Dth54HMCf1SG0iZW8sY0M8WjLDqFQOcCc5ow9936qQHatNH8_KA1VMpQCb9jP1CyitlyStux-y_Zvx1SJ0wEu3SGuNYxWS2xz1j65XPseIjFtj6SoT-PK8eOdHl854yfRZwD3xIQesIby2GpmhHekAo1LJ8dMy63ZwYaeqMnmx86zLxEbfLjaUUhSEu_smbQ7s-EfQMtbGL7EQ4fqMzw4CqoraXjjPg1Cg4UC_UiqlvqUqA22eqI7ox_1JNb-zGeZhMoUKbC2GC967ZSt1MelSrsi5fEM7mqa2m753Orz-6I32Z80xPAMnp-XdGdGlnBNvcXOXxQ_H1yuY85SHg2KZYRHO6e9w22lahkF843jiRzWttJyju3KvHv3-5T8KXbTyF9J2ERUv5g4zUcWGBqG37vGPQAgZ8UbPoElRbV8q7wxWdolVQdBHB0tcvmp9e770mbJKhWpNH-AfCccvA-0OOjLQC2sjC82K_QS04rhEFdc6hbTyjB17A_wq5gHm8Qc7DmVMAkXUVEnZgVWgTUkmQTOToVydp0xNSugpjbI_MeGJFYghRV0r0GwqEskt3xcZWX0uOErUvmqfPIYzx3HJb-Thzd1MYmoVE6ZclR8awD_7TZQhLPJ4k_NhkFZpCHyEew8Ud5_52nJoxXjHcGqQAE8oEgiIBoR2vQ_nLw48OIugjyxL0Wez6K-cbIYr4yEY5x-GkjAAzc6UFI6Ny9_e7003__mC0)

### Giải thích biểu đồ:
- Hệ thống trạm thời tiết giao tiếp trực tiếp với hệ thống quản lý dữ liệu **(IDataManagement)** để truyền dữ liệu thời tiết.
- Hệ thống bảo trì sử dụng **IMaintenance** để giám sát, bảo trì, và cập nhật các trạm thời tiết từ xa.
- Hệ thống giao tiếp vệ tinh **(ICommunication)** là trung gian truyền dữ liệu giữa các hệ thống trạm và hệ thống quản lý/lưu trữ.
- Hệ thống dự báo thời tiết sử dụng dữ liệu từ hệ thống quản lý và cung cấp dự báo thời tiết qua **IForecasting.**
