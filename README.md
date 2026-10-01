# lib_altium

Thu vien Altium gom nguon RD-Altium-Library va Dlib trong mot Integrated Library Package.

## Cau truc
- `lib_altium.LibPkg`: project thu vien; mo bang Altium Designer.
- `RD Intergrated Lib schematic/`: symbols cua bo RD.
- `RD Intergrated Lib pcb/`: footprints cua bo RD.
- `Dlib/`: Dlib.SchLib va Dlib.PcbLib bo sung.
- `3D/`: model 3D di kem bo RD.
- `Project Outputs/`: thu vien IntLib sau khi compile.

## Them linh kien
1. Mo lib_altium.LibPkg.
2. Them symbol vao SchLib va footprint vao PcbLib; gan dung model va so chan.
3. Neu tao file thu vien moi, dung Add Existing to Project.
4. Chon Project > Compile Integrated Library.
5. Doc Messages, xu ly loi model missing / ten trung / pin-pad mismatch.
6. Cai file IntLib moi trong Installed Libraries. Cap nhat linh kien da dat bang lenh Update From Libraries khi can.

## Git
File nguon va model duoc luu truc tiep trong Git. File IntLib lon duoc tai o GitHub Releases: https://github.com/dangdangduong2k2/lib_altium/releases. Tai IntLib vao thu muc Project Outputs, hoac compile lai tu LibPkg.
Commit ca LibPkg va file nguon sau moi lan thay doi. Khong sua truc tiep IntLib.

## Nguon
- RD-Altium-Library: https://github.com/Tran-Luyen/RD-Altium-Library
- Dlib.SchLib va Dlib.PcbLib: file nguoi dung cung cap.
Khong tu gan giay phep moi cho du lieu thu vien goc.

## Kiem tra
Tat ca 73 duong dan thu vien trong project da duoc kiem tra ton tai.
Ket qua compile va cac van de con lai duoc ghi trong VALIDATION.md.

