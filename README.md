# Web_Scraping_Tiki
## **Overview**

Build a web-crawler to take in a Tiki URL and return a dataframe
- The final dataframe contains the following information:
  - Product Name
  - Price
  - URL of the product image/page
  - Discount infomation/ Badge information
  - Membership information

- Code can be found in `WEB_SCRAPING_TIKI.ipynb` file.

## **Process**
### Get URL for product categories on Tiki website
| Main Categories | URL |
| --------------- | ---- |
| Điện thoại - Tablets | https://tiki.vn/dien-thoai-may-tinh-bang/c1789?src=c.1789.hamburger_menu_fly_out_banner |
| Điện tử - Điện lạnh | https://tiki.vn/tivi-thiet-bi-nghe-nhin/c4221?src=c.4221.hamburger_menu_fly_out_banner |
| Phụ kiện - Thiết bị số | https://tiki.vn/thiet-bi-kts-phu-kien-so/c1815?src=c.1815.hamburger_menu_fly_out_banner |
| Laptop - Thiết bị IT | https://tiki.vn/laptop-may-vi-tinh/c1846?src=c.1846.hamburger_menu_fly_out_banner |
| Máy Ảnh - Quay Phim | https://tiki.vn/may-anh/c1801?src=c.1801.hamburger_menu_fly_out_banner |
| Điện Gia Dụng | https://tiki.vn/dien-gia-dung/c1882?src=c.1882.hamburger_menu_fly_out_banner |
| Nhà Cửa Đời Sống | https://tiki.vn/nha-cua-doi-song/c1883?src=c.1883.hamburger_menu_fly_out_banner |
| Hàng Tiêu Dùng - Thực Phẩm | https://tiki.vn/bach-hoa-online/c4384?src=c.4384.hamburger_menu_fly_out_banner |
| Đồ chơi, Mẹ & Bé | https://tiki.vn/me-va-be/c2549?src=c.2549.hamburger_menu_fly_out_banner |
| Làm Đẹp - Sức Khỏe | https://tiki.vn/lam-dep-suc-khoe/c1520?src=c.1520.hamburger_menu_fly_out_banner |
| Thể Thao - Dã Ngoại | https://tiki.vn/the-thao/c1975?src=c.1975.hamburger_menu_fly_out_banner |
| Xe Máy, Ô tô, Xe Đạp | https://tiki.vn/o-to-xe-may-xe-dap/c8594?src=c.8594.hamburger_menu_fly_out_banner |
| Hàng quốc tế | https://tiki.vn/hang-quoc-te/c17166?src=c.17166.hamburger_menu_fly_out_banner |
| Sách, VPP & Quà Tặng | https://tiki.vn/nha-sach-tiki/c8322?src=c.8322.hamburger_menu_fly_out_banner |
| Voucher - Dịch Vụ - Thẻ Cào | https://tiki.vn/voucher-dich-vu/c11312?src=c.11312.hamburger_menu_fly_out_banner |

### Create functions to scrape infor from one product -- then all product from a page -- then all pages
Information scrapped include:
| ID | Info |
| --------------- | ---- |
| 1 | Name |
| 2 | Price |
| 3 | Product_URL |
| 4 | Image_URL |
| 5 | Freeship |
| 6 | Average_Review |
| 7 | No_of_sales |
| 8 | On_sale |
| 9 | Tikinow |
| 10 | Tikinow_member_deal |
| 11 | Badge_ReHonHoanTien |
| 12 | Badge_TraGop |
| 13 | Badge_FreeGift |

### Scapped information stored in `tiki_products.csv`
