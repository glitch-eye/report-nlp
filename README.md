# NLP Course Assistant Report

Báo cáo LaTeX cho bài tập lớn Course Assistant (CO3085).

## Cấu trúc

- `main.tex`: file gốc, mục lục, danh sách hình/bảng và các chương.
- `template/cover.tex`: bìa theo phong cách mẫu `newbranch`, đã đổi nội dung sang NLP.
- `template/header-footer.tex`: header/footer và logo trường.
- `assets/hcmut.png`: logo sử dụng ở bìa và header.
- `sections/`: nội dung sáu chương của báo cáo.

## Biên dịch

Yêu cầu XeLaTeX (do sử dụng `fontspec` và `polyglossia`):

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
```

Hoặc chạy hai lượt để cập nhật mục lục và tham chiếu:

```bash
xelatex -interaction=nonstopmode -halt-on-error main.tex
xelatex -interaction=nonstopmode -halt-on-error main.tex
```

## Trước khi nộp

1. Điền mã nhóm, tên giảng viên, danh sách thành viên và MSSV trong `template/cover.tex`.
2. Kiểm tra lại học kỳ/ngày tháng theo lịch nộp thực tế.
3. Đối chiếu các số liệu ở Chương 5 với đúng artifact/dataset được dùng.
4. Chạy biên dịch XeLaTeX trên máy cá nhân và kiểm tra danh sách hình, bảng, mục lục, số trang.
5. Không xem hình sơ đồ kiến trúc là bằng chứng thực nghiệm; đây là sơ đồ mô tả thiết kế.