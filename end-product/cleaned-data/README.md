# Giải thích file

## I. Về cấu trúc dữ liệu
1. Sơ đồ DSD:
   
<p align="center" width="100%">
    <img width="75%" src="https://github.com/user-attachments/assets/63960f9c-040b-4333-9246-0ecb4aefeb23">
</p>
2. Sơ đồ DSD chi tiết <b>(giải thích tốt hơn, vẽ bởi tác giả):</b>
<br>
<br>
<p align="center" width="100%">
    <img width="75%" src="https://github.com/user-attachments/assets/b76fc54e-c228-4c26-9d01-8b39ee7cab03">
</p>

## II. Data Dictionary
Phía dưới sẽ là Data Dictionary của từng bảng đã xuất hiện trong sơ đồ trên.

1. <b> Bảng fact_BA_job (Fact - Business Analyst Jobs: Bảng chính của dữ liệu, chứa thông tin giá trị của các thuộc tính)</b>

| Tên cột      	| Ý nghĩa      	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| job_id        	| Giá trị định danh công việc tuyển dụng  |
| job_domain_id        	| Giá trị định danh lĩnh vực của công việc tuyển dụng  |
| job_level_id        	| Giá trị định danh trình độ yêu cầu công việc tuyển dụng  |
| job_salary        	| Mức lương offer của công việc tuyển dụng  |
| job_exp        	| Số năm kinh nghiệm yêu cầu của công việc tuyển dụng  |
| job_hiring_count        	| Số đầu nhân sự công việc tuyển dụng  |
| company_id        	| Giá trị định danh công ty tuyển dụng  |
| distance_to_work        	| Khoảng cách từ nhà tới nơi làm việc (khoảng cách tính từ bến xe Giáp Bát tới UBND các đơn vị hành chính ghi trong địa chỉ làm việc)  |
| is_work_Sat_id        	| Giá trị boolean nhưng mà cũng định danh cho trạng thái công việc có làm việc thứ 7 hay không, giá trị 1 là không, 0 là có |
| job_working_hour        	| Tổng thời gian làm việc trong tuần của công việc, lưu ý là tổng, đơn vị là tiếng  |
| has_ai        	| Công việc có liên quan tới AI hay không? 1 là có, 0 là không |
| has_DA_skills        	| Công việc có yếu tố DA hay không? 1 là có, 0 là không  |
| has_odoo        	| Công việc có liên quan tới Odoo hay không? 1 là có, 0 là không  |
| has_saas        	| Công việc có liên quan tới SaaS hay không? 1 là có, 0 là không  |
| has_scrum        	| Công việc có liên quan tới Scrum hay không? 1 là có, 0 là không  |
| has_sor        	| Công việc có liên quan tới SoR hay không? 1 là có, 0 là không  |

2. <b> Bảng dim_job_domain (Dimension - Job Domains: Bảng lĩnh vực công việc)
   
| Tên cột      	| Ý nghĩa      	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| job_domain_id        	| Giá trị định danh lĩnh vực của công việc tuyển dụng  |
| job_domain        	| Lĩnh vực của công việc tuyển dụng  |

3. <b> Bảng dim_level (Dimension - Job Level: Bảng trình độ yêu cầu cho công việc)
   
| Tên cột      	| Ý nghĩa      	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| level_id        	| Giá trị định danh trình độ yêu cầu công việc tuyển dụng  |
| level_name        	| Trình độ yêu cầu của công việc tuyển dụng  |

4. <b> Bảng dim_company (Dimension - Company: Bảng tên công ty tuyển dụng)
   
| Tên cột      	| Ý nghĩa      	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| company_id        	| Giá trị định danh công ty tuyển dụng  |
| company_name        	| Tên công ty tuyển dụng  |

5. <b> Bảng dim_work_Saturday (Dimension - Work on Saturday?: Bảng boolean đại diện cho công việc có yêu cầu làm thứ 7 hay không)
   
| Tên cột      	| Ý nghĩa      	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| is_work_Sat_id        	| Giá trị boolean định danh cho trạng thái công việc có làm việc thứ 7 hay không |
| statement        	| Trạng thái "có" và "không"  |
