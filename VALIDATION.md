# Kết quả kiểm tra — 01/10/2026

- Đã kiểm tra đủ 73 file thư viện nguồn trong lib_altium.LibPkg.
- Đã biên dịch bằng Altium Designer Professional 25.6.2.
- Đã tạo Project Outputs/lib_altium.IntLib (289935872 bytes).
- File nguồn giữ nguyên nội dung; việc gộp không tự sửa chân hay hình học footprint.

## Các vấn đề còn tồn tại trong dữ liệu nguồn

Bản build hiện có **9 lỗi và 17 cảnh báo compiler**. Không coi đây là bộ thư viện đã được xác minh đầy đủ về điện hoặc footprint.

- ICM20948 trong Dlib: model QFN-24_L3.0-W3.0-P0.40-BL-EP không tìm thấy pad 1, 6, 7, 12, 13, 18, 19, 24.
- SLW05A-12 trong Dlib: footprint không tìm thấy pad 4.
- Thiếu model cho CONN 5569 AW 8P, XH2.54 4P RA SMD, MOC3063M, MOC3083M, Screw Vit m3.
- 12 cảnh báo chân trùng ở một số IC và module; có thể là chân dùng chung giữa các phần, cần xem từng linh kiện trước khi sửa.

Chi tiết chính xác trong COMPILE_MESSAGES.txt. Kiểm tra các linh kiện này theo datasheet và footprint thực tế trước khi sử dụng. Không thay đổi số chân chỉ để bỏ lỗi compiler.

## Phạm vi

Gộp đúng các tài liệu của project RD Integrated_Library.LibPkg hiện có và hai file Dlib được cung cấp. Các thư viện rời khác nằm ngoài project gốc không tự động thêm vào.
Giữ kèm thư mục 3D của bộ RD. Các liên kết ngoài và model 3D của từng linh kiện chưa được kiểm tra toàn diện trên máy khác.


## USB 73725-0110BLF: embedded 3D update — 02/11/2026

- Embedded the manufacturer STEP model in USB_A_UPRIGHT_73725-0110BLF.
- Verified native Altium 3D display, embedded model bytes, four signal axes,
  original model dimensions and zero additional placement offset.
- Kept all 63 other Dlib footprints and all 35 existing embedded models unchanged.
- Rebuilt IntLib with the same existing 9 errors and 17 warnings; no new diagnostics.
- See Dlib/73725-0110BLF.md for model source, alignment and drawing revision notes.


## KCD1-104B / KCD117 rocker — 02/11/2026

- Added a 4-pin DPST symbol and embedded similar-shape STEP model to Dlib.
- Footprint is a visual reference only, per user request; no OEM interchangeability claim.
- Verified native symbol/pad counts, model placement and exact STEP bytes in PcbLib and compiled IntLib.
- Preserved all 64 previous Dlib footprints, existing symbol streams, and 36 embedded models.
- Existing Jack DC 5.5*2.1 / JACK_DC 5.5 mm already includes Jack DC.STEP; no duplicate created.
- Compiler diagnostics unchanged: 9 baseline errors and 17 warnings, no new diagnostics.
- See Dlib/KCD1-104B.md for source and limitations.

KCD1-104B symbol appearance revised: contact circles fixed, pin names hidden, labels aligned. Pin anchors/electrical properties and PcbLib unchanged; compiled symbol data matches source; no new compiler diagnostics.
