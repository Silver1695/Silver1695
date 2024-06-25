use QuanLyThuoc;
CREATE TABLE NhaPhanPhoi (
	MaNPP NVARCHAR(50) PRIMARY KEY,
    Ten NVARCHAR(50) NOT NULL,
    DiaChi NVARCHAR(50) NOT NULL,
    Email NVARCHAR(50) NOT NULL,
    SDT NVARCHAR(10) NOT NULL
);

CREATE TABLE HoaDon (
    MaHD NVARCHAR(50) PRIMARY KEY,
    SoLuong INT NOT NULL,
    ThanhTien FLOAT NOT NULL,
    NgayThang DATETIME NOT NULL,
    MaNV NVARCHAR(50) NOT NULL,
    MaKH NVARCHAR(50) NOT NULL
);

select * from NhaPhanPhoi;
select * from HoaDon;


INSERT INTO NhaPhanPhoi (MaNPP, Ten, DiaChi, Email, SDT)
VALUES 
('NPP001', 'Nhà phân phối A', '123 Đường A, Quận 1', 'npp_a@example.com', '0123456789'),
('NPP002', 'Nhà phân phối B', '456 Đường B, Quận 2', 'npp_b@example.com', '0987654321'),
('NPP003', 'Nhà phân phối C', '789 Đường C, Quận 3', 'npp_c@example.com', '0912345678'),
('NPP004', 'Nhà phân phối D', '321 Đường D, Quận 4', 'npp_d@example.com', '0908765432'),
('NPP005', 'Nhà phân phối E', '654 Đường E, Quận 5', 'npp_e@example.com', '0934567890');
go

INSERT INTO HoaDon (MaHD, SoLuong, ThanhTien, NgayThang, MaNV, MaKH)
VALUES 
('HD001', 10, 1500000.50, '2024-06-25 10:00:00', 'NV001', 'KH001'),
('HD002', 5, 750000.00, '2024-06-26 11:30:00', 'NV002', 'KH002'),
('HD003', 3, 450000.00, '2024-06-27 09:45:00', 'NV001', 'KH003'),
('HD004', 8, 1200000.00, '2024-06-28 14:20:00', 'NV003', 'KH004'),
('HD005', 2, 300000.00, '2024-06-29 15:10:00', 'NV002', 'KH005');
go
