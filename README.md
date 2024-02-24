# Air quality prediction

Mục tiêu của nghiên cứu này là lấy dữ liệu thời tiết Bắc Kinh có sẵn công khai từ năm 2013 đến năm 2017 và áp dụng các kỹ thuật học máy để dự đoán lượng nồng độ PM2.5 trong không khí dựa trên các đặc điểm môi trường với độ chính xác cao và sai số bình phương trung bình thấp

# Thông tin dữ liệu:

Bộ dữ liệu này bao gồm dữ liệu về chất gây ô nhiễm không khí hàng giờ từ 12 địa điểm giám sát chất lượng không khí do toàn quốc kiểm soát. Dữ liệu chất lượng không khí được lấy từ Trung tâm giám sát môi trường thành phố Bắc Kinh. Dữ liệu khí tượng ở mỗi địa điểm chất lượng không khí được khớp với trạm thời tiết gần nhất của Cục Khí tượng Trung Quốc. Khoảng thời gian từ ngày 1 tháng 3 năm 2013 đến ngày 28 tháng 2 năm 2017. Dữ liệu thiếu được ký hiệu là NA.

# Thông tin thuộc tính:

- No: row number
- year: year of data in this row
- month: month of data in this row
- day: day of data in this row
- hour: hour of data in this row
- PM2.5: PM2.5 concentration (ug/m^3)
- PM10: PM10 concentration (ug/m^3)
- SO2: SO2 concentration (ug/m^3)
- NO2: NO2 concentration (ug/m^3)
- CO: CO concentration (ug/m^3)
- O3: O3 concentration (ug/m^3)
- TEMP: temperature (degree Celsius)
- PRES: pressure (hPa)
- DEWP: dew point temperature (degree Celsius)
- RAIN: precipitation (mm)
- wd: wind direction
- WSPM: wind speed (m/s)
- station: name of the air-quality monitoring site
  PM là viết tắt của hạt vật chất (còn gọi là ô nhiễm hạt): thuật ngữ chỉ hỗn hợp các hạt rắn và giọt chất lỏng được tìm thấy trong không khí. Một số hạt, chẳng hạn như bụi, chất bẩn, bồ hóng hoặc khói, có kích thước lớn hoặc tối đến mức có thể nhìn thấy bằng mắt thường. Một số khác thì nhỏ đến mức chỉ có thể được phát hiện bằng kính hiển vi điện tử.
  Ô nhiễm hạt bao gồm:
- PM10 : các hạt có thể hít phải, có đường kính thường từ 10 micromet trở xuống;
- PM2.5: các hạt mịn có thể hít vào, có đường kính thường từ 2,5 micromet trở xuống

# Nhiệm vụ ban đầu:

- Tiền xử lý dữ liệu
- Phân tích dữ liệu thăm dò: Đặt các câu hỏi về dữ liệu và trả lời chúng thông qua biểu đồ
- Đào tạo và đánh giá mô hình

# Mô hình

Tạm thời bắt đầu với mô hình đơn giản trước: Decision Tree Regressor, RandomForestRegressor, GradientBoostingRegressor để đào tạo và đánh giá trước.
