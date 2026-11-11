# Global Sales Performance Dashboard

Dashboard Power BI phân tích hiệu quả kinh doanh toàn cầu theo **thị trường**, **danh mục sản phẩm** và **thời gian**, từ đó đưa ra các khuyến nghị về mở rộng thị trường.

---

## 1. Tổng quan dự án

**Câu hỏi kinh doanh chính**
- Tổng quan kinh doanh hiện tại như thế nào?
- Tình hình kinh doanh của các thị trường ra sao?
- Tình hình kinh doanh của các nhóm sản phẩm như thế nào?

**Mô hình dữ liệu (Star Schema)**

| Loại | Bảng |
|---|---|
| Fact | `factOrder`, `Return` |
| Dimension | `dimDate`, `dimProduct`, `dimRegion`, `dimCustomer`, `People` |
| Hỗ trợ | `_Measures`, `Parameters` (Metric Selector) |

**Các measure chính:** Total Sales, Total Orders, Total Profit, Profit Margin, Average Order Value (AOV), Quantity Sold, Return Rate, Sales/Profit/AOV Growth, YoY Growth.

---

## 2. Cấu trúc Dashboard

| Trang | Nội dung |
|---|---|
| **Executive Summary** | KPI tổng quan và % thay đổi, xu hướng Sales & Profit theo thời gian, hiệu quả theo Sub-Category và Market, cơ cấu theo Segment, Top Sales Person, Top Customers |
| **Market Performance Analysis** | Best region, highest profit/margin/YoY growth market, scatter Sales vs. Profit Margin (Scale up / Cash cow / Invest / Reconsider), Return Rate theo thị trường, Decomposition Tree, bảng chi tiết theo Market → City |
| **Product Performance Analysis** | Top category theo Sales/Orders/Profit/Margin, Return Rate thấp nhất, treemap Sales Growth, scatter Sales vs. Margin theo Sub-Category, bảng chi tiết theo Category → Product |
| **Insights and Recommendations** | Tổng hợp insight và khuyến nghị cho Market, Product và tổng thể |

---

## 3. Main visualizations
- KPI chính
<img width="1026" height="86" alt="image" src="https://github.com/user-attachments/assets/d076fda7-4f6f-4dc9-8a54-9b3d8d9fb059" />
- Sales metrics by Time and Market
<img width="1018" height="574" alt="image" src="https://github.com/user-attachments/assets/256785b6-4505-4897-8be1-72ac28272e59" />

---

## 4. Main Findings

### Tổng thể
- Công ty tăng trưởng tốt: **Sales ~26%/năm**, **Profit ~24%/năm**, **Profit Margin ổn định trên 11%**.
- **APAC, EU và US** là 3 động lực doanh thu chính, luôn nằm trong top 3 ở Sales, Profit và Profit Margin. Tăng trưởng đã chậm lại, nhiều khả năng do thị trường đã trưởng thành chứ không phải suy giảm.

### Thị trường
- **APAC** có doanh số lớn nhất (**~$3.6M**) nhưng Profit Margin và AOV thấp, đặc biệt **Đông Nam Á (PM chỉ ~2.02%)**.
- **EU, US, Oceania, Central Asia** có lợi nhuận tốt (PM trung bình **~13.5%**) và tăng trưởng bền vững (**~24.22%**).
- **Trung Quốc, Nhật Bản, Hồng Kông, Anh, Phần Lan, Na Uy** có margin cao (trung bình **~22.7%**) nhưng **Return Rate cao (~13.31%)** và RCR thấp, đặc biệt Nhật Bản và Anh (~3%).
- **Canada, Nam Phi và Trung Đông** hiện đóng góp nhỏ (~$175.83K) nhưng **tăng trưởng doanh số rất mạnh (~70.28%)**, còn nhiều tiềm năng chưa khai thác.

### Sản phẩm
- **Technology** là category mạnh nhất, đứng đầu về Sales, Profit và Profit Margin.
- **Full-size Smartphones** có doanh số cao nhất, margin khá (**6.81% – 23.27%**) và tăng trưởng hai chữ số (**27.5% – 67.81%**), ngoại trừ Nokia.
- **Machines** có margin thấp (**7.56%**) và tăng trưởng thấp (**17.48%**). Một số sản phẩm Copier/Machine doanh số cao nhưng đang chậm lại hoặc tăng trưởng âm.
- **Furniture** nhìn chung kém hiệu quả hơn. **Tables** yếu nhất, nhiều sản phẩm margin âm, tăng trưởng âm và Return Rate **7.54%**. Ngược lại, Bookcases, Adjustable Leather Chairs và Furnishings tốt hơn (5 sản phẩm Adjustable Leather Chairs chiếm **~50% doanh số Furniture**, tăng trưởng **25.47%**).
- **Office Supplies** có margin lành mạnh dù doanh số thấp hơn. Paper và Envelopes có margin cao, còn một số sản phẩm Storage lỗ (Hoover Stove White, Hamilton Beach Stove Silver).
- **Accessories** có Return Rate tương đối cao. Các nhóm hay bị hoàn trả gồm Fasteners, Accessories, Appliances, Furnishings.

---

## 5. Main Recommendations

### Thị trường
1. **Giữ mức đầu tư ở APAC, EU, US và cải thiện lợi nhuận Đông Nam Á.** Chuyển product mix sang sản phẩm margin cao và triển khai gói bundle tại Indonesia, Philippines, Thái Lan, Việt Nam.
2. **Giảm tỷ lệ hoàn trả trước khi mở rộng ở Bắc Á và một số thị trường châu Âu.** Rà soát lý do hoàn trả, siết kiểm soát chất lượng sản phẩm hay bị trả, cải thiện dịch vụ hậu mãi.
3. **Mở rộng có chọn lọc vào các thị trường mới nổi (Canada, Nam Phi, Trung Đông).** Tăng đối tác phân phối và marketing bản địa hóa, đồng thời theo dõi sát lợi nhuận trước khi mở rộng quy mô lớn.

### Sản phẩm
1. **Ưu tiên danh mục smartphone cao cấp** (tăng tồn kho và khuyến mãi cho Full-size Smartphones). Rà soát chi phí Canon Advanced Copiers và các sản phẩm Machines kém hiệu quả.
2. **Tái phân bổ nguồn lực từ Tables sang các sản phẩm Furniture margin cao.** Giảm tồn kho và chi phí khuyến mãi cho Tables.
3. **Tối ưu product mix của Office Supplies.** Xem xét các sản phẩm Storage lỗ, đẩy mạnh Paper, Envelopes và một số Appliances có lợi nhuận tốt.

### Chiến lược chung
- **Ưu tiên chất lượng lợi nhuận hơn quy mô doanh thu:** tối ưu giá, hạn chế giảm giá quá mức, đẩy mạnh danh mục margin cao tại các thị trường doanh số lớn nhưng margin thấp.
- **Phân tích Return Rate ở cấp SKU**, đặc biệt với Accessories, kết hợp cải thiện chất lượng, thông tin sản phẩm và hậu mãi.
- **Đa dạng hóa doanh thu** bằng cách mở rộng dần mạng lưới phân phối tại Canada và EMEA.
- **Cân bằng lại Furniture:** chuyển tồn kho, marketing và khuyến mãi sang sản phẩm có margin và tăng trưởng bền vững, đồng thời rà soát giá và chi phí cho nhóm kém hiệu quả.

---

## 6. Hướng phát triển
- Bổ sung phân tích mức chiết khấu (discount) và ảnh hưởng đến margin.
- Phân tích lý do hoàn trả theo SKU.
- Thêm dự báo (forecast) doanh số và lợi nhuận theo thị trường.
